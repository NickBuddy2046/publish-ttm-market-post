# Publish TTM Market Post

A reusable Codex skill for researching, drafting, previewing, and publishing original market commentary on [To The Moon](https://ttm.financial/) in natural Hong Kong Cantonese.

## What it does

- Reads current TTM topics and the user's recent posts when relevant.
- Verifies market claims with primary or authoritative sources.
- Drafts a balanced Cantonese article with a clear thesis, counterargument, indicators, sources, hashtags, and disclaimer.
- Prepares and previews the article in the signed-in TTM editor.
- Requires explicit confirmation immediately before the final publish click.
- Verifies the published title and returns the canonical post URL.

## Requirements

- ChatGPT desktop or Codex with local skill support.
- Browser or Chrome-control capability.
- A TTM account signed in within the selected browser.
- Web access for time-sensitive market research.

The skill contains no credentials, cookies, account IDs, or private browsing data. Each user signs in to their own TTM account.

## Install

Ask Codex to install the skill from this GitHub repository:

```text
$skill-installer install the publish-ttm-market-post skill from
https://github.com/NickBuddy2046/publish-ttm-market-post/tree/main/skills/publish-ttm-market-post
```

Alternatively, copy `skills/publish-ttm-market-post` to:

```text
~/.agents/skills/publish-ttm-market-post
```

Restart Codex if the skill does not appear automatically.

## Use

Invoke it explicitly:

```text
$publish-ttm-market-post 幫我今日 upload 一篇
```

The skill may also trigger automatically for requests about drafting or publishing a current TTM market post.

## Safety

The workflow separates drafting from publishing. It will not publish a public post until the user confirms at action time after reviewing the account, title, and preview.

## License

MIT
