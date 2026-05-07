# Higgsfield AI

Higgsfield AI brings image and video generation workflows to Codex through the Higgsfield CLI. This plugin includes skills for general image/video generation, Soul Character training, product photoshoots, and marketplace-ready product cards.

## Skills

| Skill | Description |
|---|---|
| [higgsfield-generate](./skills/higgsfield-generate) | Image and video generation across Higgsfield models, including Marketing Studio for branded ads with avatars, products, hooks, and settings. |
| [higgsfield-soul-id](./skills/higgsfield-soul-id) | Train a reusable Soul Character for identity-faithful image and video generation. |
| [higgsfield-product-photoshoot](./skills/higgsfield-product-photoshoot) | Brand-quality product imagery with mode-specific prompt enhancement. |
| [higgsfield-marketplace-cards](./skills/higgsfield-marketplace-cards) | Marketplace listing visuals, compliant main images, secondary product images, and A+ style modules. |

## CLI Setup

The skills use the Higgsfield CLI. If it is not installed, Codex should install it with the official installer:

```bash
curl -fsSL https://raw.githubusercontent.com/higgsfield-ai/cli/main/install.sh | sh
```

After installation, authenticate once:

```bash
higgsfield auth login
```

Codex can verify authentication with:

```bash
higgsfield account status
```

## Common Workflows

- Generate an image or video: use `higgsfield-generate`.
- Train a face/identity model: use `higgsfield-soul-id`, then pass the returned reference id to `higgsfield-generate` with `--soul-id`.
- Create product campaign imagery: use `higgsfield-product-photoshoot`.
- Build marketplace listing images: use `higgsfield-marketplace-cards`.

## Links

- Website: https://higgsfield.ai
- Privacy Policy: https://higgsfield.ai/privacy-policy
- Terms of Use: https://higgsfield.ai/terms-of-use-agreement
- Source repository: https://github.com/higgsfield-ai/skills

## License

MIT. See [LICENSE](./LICENSE).
