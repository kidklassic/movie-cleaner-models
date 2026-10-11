# Movie Cleaner – speech models

Download copies of the speech-recognition models used by **Movie Cleaner**, a free app
from [Doctor Soni Apps](https://doctorsoni.ca) that mutes bad language in movies you own.

The app downloads its model from this repo's
[`models-v1` release](../../releases/tag/models-v1) the first time it's used, and falls back
to the original source on Hugging Face if this copy can't be reached. Every file is checked
against a SHA-256 fingerprint built into the app.

| App setting | Model | Original source (exact version) |
|---|---|---|
| Fast | base | [Systran/faster-whisper-base @ ebe41f7](https://huggingface.co/Systran/faster-whisper-base/tree/ebe41f70d5b6dfa9166e2c581c45c9c0cfc57b66) |
| Balanced | small | [Systran/faster-whisper-small @ 536b066](https://huggingface.co/Systran/faster-whisper-small/tree/536b0662742c02347bc0e980a01041f333bce120) |
| Best | medium | [Systran/faster-whisper-medium @ 08e178d](https://huggingface.co/Systran/faster-whisper-medium/tree/08e178d48790749d25932bbc082711ddcfdfbc4f) |

The files are unchanged copies, made by the
[`mirror.yml`](.github/workflows/mirror.yml) workflow, which also checks each model
against Hugging Face's own fingerprint before publishing.

## License

These are [OpenAI Whisper](https://github.com/openai/whisper) models converted to
CTranslate2 format by [SYSTRAN](https://huggingface.co/Systran), released under the
MIT License (see `LICENSE`).
