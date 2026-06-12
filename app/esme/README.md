# Esme Background Assets

This collection contains calm 16:9 WebP backgrounds for the Esme app and installer.

## Main App Rotation

Path:

`app/esme/main/bg/<slot>/<slot>-NN.webp`

Slots:

- `morning`
- `day`
- `night`
- `night-owl`

Each slot currently contains six 3840x2160 WebP images. The intended app behavior is:

- show one background for about 30 minutes by default,
- fade to the next background,
- keep UI contrast overlays controlled in the app layer.

Suggested transition:

- `fade`
- 1800 ms
- future 15 or 30 minute rotations work without changing app code; add assets to the manifest and the app will cycle through them.

## Installer Backgrounds

Path:

`app/esme/install/bg/<step>.webp`

Current installer steps:

- `welcome-license`
- `email-account`
- `provider-permissions`
- `ai-provider`
- `mailbox-scan`
- `receipt-ocr`
- `setup-complete`

These are designed to be unique to the task being performed while staying in the same calm visual family.

## Usage Notes

- Images are AI-generated and released under this repository's CC-BY 4.0 license.
- No image should contain readable text, logos, provider marks, or UI.
- Treat provider mirroring and AI-provider setup backgrounds as trust moments: pair them with clear copy about what leaves the computer and what stays local.
- Keep final app overlays subtle; these backgrounds are intentionally quiet.
