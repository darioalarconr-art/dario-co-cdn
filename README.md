# Dario Co — Public CDN

Public asset hosting for Dario Co client pipelines. Used by Instagram Graph API (which requires public HTTPS image URLs) and any other workflow needing a stable public URL.

## Conventions

```
<client-slug>/<YYYY-MM-DD>/<asset-name>.<ext>
```

Raw URL pattern:
```
https://raw.githubusercontent.com/darioalarconr-art/dario-co-cdn/main/<client-slug>/<YYYY-MM-DD>/<asset-name>.<ext>
```

## Privacy

Public repository. Every asset committed here is universally readable — exactly the same exposure profile as the final published Instagram post. Do **not** commit:

- Drafts not yet approved by the client.
- Unredacted contracts, NDAs, internal handoffs.
- Anything that would still be private after the post goes live.

## Migration plan

Catbox/0x0.st-style anonymous hosts have either disabled uploads or hard-block AI-agent clients (2026). This repo is the legitimate `$0` stand-in. After 3 manual publishes per Dario Co `agency_rules.md` "manual-3-times" rule, evaluate migration to **Cloudflare R2** with a custom subdomain.
