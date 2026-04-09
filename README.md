# Stained Glass Art Generator

Generate stunning stained glass style art and illustrations from text descriptions. Create luminous jewel-toned stained glass portraits, animals, landscapes, and decorative panels — perfect for wall art, print-on-demand, posters, church window designs, and mosaic-inspired artwork.

Powered by the Neta AI image generation API (api.talesofai.com) — the same service as neta.art/open.

## Install

```bash
npx skills add blammectrappora/stained-glass-art-generator
```

or

```bash
clawhub install stained-glass-art-generator
```

## Token Setup

This skill requires a Neta API token (free trial available at <https://www.neta.art/open/>).

Pass it via the `--token` flag:

```bash
node <script> "your prompt" --token YOUR_TOKEN
```

## Usage

Generate a stained glass art panel with default settings (portrait size):

```bash
node stainedglassartgenerator.js "a majestic lion in stained glass style with rich amber and gold tones" --token "$NETA_TOKEN"
```

Generate a landscape stained glass scene:

```bash
node stainedglassartgenerator.js "a serene mountain lake scene in stained glass, deep blues and greens" --token "$NETA_TOKEN" --size landscape
```

Generate a square stained glass design:

```bash
node stainedglassartgenerator.js "an intricate rose window cathedral design with ruby red and sapphire blue glass" --token "$NETA_TOKEN" --size square
```

Use a reference image UUID for style inheritance:

```bash
node stainedglassartgenerator.js "a peacock with jewel-toned feathers in stained glass" --token "$NETA_TOKEN" --ref YOUR_REFERENCE_UUID
```

Returns a direct image URL.

## Options

| Option | Description | Default |
|--------|-------------|---------|
| `--token` | Neta API token (required) | — |
| `--size` | Image dimensions: `portrait`, `landscape`, `square`, `tall` | `portrait` |
| `--ref` | Reference image UUID for style inheritance | — |

### Size Reference

| Size | Dimensions |
|------|-----------|
| `portrait` | 832 x 1216 |
| `landscape` | 1216 x 832 |
| `square` | 1024 x 1024 |
| `tall` | 704 x 1408 |

This skill requires a Neta API token (free trial available at https://www.neta.art/open/).

## Example Output

```bash
node stainedglassartgenerator.js "a beautiful stained glass art panel, luminous jewel-toned colors, bold dark lead lines separating glass segments, radiant light shining through translucent colored glass, intricate detailed glasswork pattern, cathedral window aesthetic"
```

![Example output](https://oss.talesofai.cn/picture/027e5a16-ce53-410d-9a09-350d89db93f8.webp)

> Prompt: *"a beautiful stained glass art panel, luminous jewel-toned colors, bold dark lead lines separating glass segments, radiant light shining through translucent colored glass, intricate detailed glasswork pattern, cathedral window aesthetic"*
