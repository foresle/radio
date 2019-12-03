# AutoRadio
> An easy way to have a 24/7 audio stream of music. 

## Requirements
- docker
- docker-compose
- Some music

## Install
- Copy `.env.example` to `.env` and edit it
- Put music inside `music/`
- Run `docker-compose up -d --build`
- Listen to `http://localhost:8000/live` (if you changed `ICECAST_PORT`, edit the port in the URL)

## Config
Everything is set in the `.env` file (or your shell environment).  
All settings are optional but please set the two passwords or it will stay to the default, `hackme`.

- `ICECAST_PORT`: The port to bind Icecast in the open.
- `ICECAST_SOURCE_PASSWORD`: The password to stream audio to Icecast.
- `ICECAST_ADMIN_PASSWORD`: The password for Icecast's administration.
- `STREAM_NAME`: A title for your stream.
- `STREAM_DESC`: A description for your stream.
- `STREAM_URL`: A URL (like your website) to show on the stream details.
