# pagelock-voices

Model files for the offline read-aloud voice in the PageLock reading app.
The app downloads them only when the user asks for the built-in natural
voice, checks each file against `SHA256SUMS`, and runs them on the phone.
Nothing here is app code.

## Releases

| Tag | Voice | Files |
|---|---|---|
| `supertonic-3-int8-v1` | Supertonic 3, int8 | 7 model files, `SHA256SUMS`, both licences |

Files under an existing tag are never replaced or deleted. A new or updated
model gets a new tag, so every app version keeps downloading exactly the
files it was built for.

## Where the files come from

- **Supertonic 3** by Supertone Inc.
  ([Hugging Face](https://huggingface.co/Supertone/supertonic-3),
  [GitHub](https://github.com/supertone-inc/supertonic)).
- **int8 export** by k2-fsa sherpa-onnx: the files are unchanged copies from
  `sherpa-onnx-supertonic-3-tts-int8-2026-05-11.tar.bz2` in
  [sherpa-onnx's tts-models release](https://github.com/k2-fsa/sherpa-onnx/releases/tag/tts-models).

## Licences

- `LICENSE-code`: MIT licence (Supertone Inc.), shipped with the export.
- `LICENSE-model`: the model weights are under the BigScience Open RAIL-M
  licence, as published on Supertone's Hugging Face model card. Its use
  restrictions (Attachment A) apply to anyone who uses these files,
  including through PageLock.
