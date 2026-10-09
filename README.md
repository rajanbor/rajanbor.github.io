# rajanbor.github.io

Landing page for **AI Chat for Business**, served at <https://rajanbor.github.io>.

A static export of `apps/landing` from the product monorepo. The page itself is
three links and a word: the demo, the onboarding walkthrough, and sign-in. There
is nothing else to say yet that would not be a promise.

`.nojekyll` is not decoration — without it GitHub Pages skips `_next/`, because
Jekyll ignores directories that begin with an underscore, and the page loads
unstyled.

## Updating it

Rebuild the export in the monorepo and copy it over:

```bash
LANDING_STATIC_EXPORT=1 pnpm --filter @ai-chat/landing build
```

The output lands in `apps/landing/out`.
