# whisper rs

> Port of OpenAI's Whisper model in Rust/Candle

## Usage

```
# download video and convert to output.wav
ffmpeg -i ~/input.mp4 -vn -ar 44100 -ac 2 -b:a 192k ~/output.wav
cargo run --features metal -- --timestamps --input ~/output.wav --model large-v3

# run release
cargo run --release --features metal -- --timestamps --input ~/output.wav --model large-v3

```

## Roadmap

## Credit

- https://github.com/huggingface/candle
- https://github.com/ggerganov/whisper.cpp
