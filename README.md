# Multi-agent meeting example using local LiveKit server:

There's a bunch of instructions here, but it's all fairly straightforward. The agents are slightly modified from the [fast agent example](https://github.com/dsa/fast-voice-assistant/) to explicitly have separate names and run on different ports. This will be more automated in a future release, but for now the tweaks are to get things to work.

## Run LiveKit server
These commands will install [LiveKit server](https://github.com/livekit/livekit) on your machine and run it in dev mode. Dev mode uses a specific API key and secret pair.
1. `brew install livekit`
2. `livekit-server -dev`

## Meeting link
'Meet' interface from Livekit sandbox 

## Run first agent
1. `cd agent-1`
2. `python -m venv .venv`
3. `source .venv/bin/activate`
4. `pip install -r requirements.txt`
5. `cp .env.example .env`
6. add values for keys in `.env`
7. `python main.py dev` | `python main.py start`

