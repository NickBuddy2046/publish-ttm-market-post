---
name: publish-ttm-market-post
description: Research, draft, illustrate, independently review, preview, and publish original market commentary on To The Moon (TTM/ttm.financial) in natural Hong Kong Cantonese. Use when the user asks for a daily TTM post, a program-trading or investment article based on current platform trends, relevant article images, or help publishing through their signed-in Chrome tab.
---

# Publish TTM Market Post

Create a timely, evidence-based TTM article in Hong Kong Cantonese. Keep drafting and publishing as separate stages: never publish a draft unless the user asks, and always obtain action-time confirmation immediately before the final publish click.

## Default editorial profile

- Write in Traditional Chinese with natural Hong Kong Cantonese phrasing.
- Sound informed and conversational, not like a sales pitch or a copied research report.
- Aim for roughly 900–1,400 Chinese characters unless the user requests another length.
- Use a clear personal thesis while separating verified facts, inference, and opinion.
- Avoid guaranteed-return language, direct trade commands, invented figures, and exaggerated claims.
- End with a discussion question, focused hashtags, source links, and a statement that the article is not investment advice.

If the author's profile focuses on program trading, make that identity visible in the thesis and execution framework. Convert market commentary into rules another person could implement or test:

- Define the observable inputs and reference time.
- State scenario thresholds and confirmation signals.
- Include an explicit no-trade condition.
- Define entry timing, fixed risk, stop logic, and re-entry logic.
- Label illustrative thresholds as a framework rather than backtest results.

## Workflow

### 1. Read the live platform context

If the request refers to the current page, current feed, or TTM trends, inspect the selected Chrome tab first. Use the available Chrome-control skill for interactive browser work and follow its instructions.

Scan the visible feed for repeated subjects, platform-promoted topics, heavily discussed stocks, market-moving events, and recent engagement. Check the user's recent posts when practical so the new angle does not duplicate an earlier article.

Verify the publishing identity from the visible profile or preview. Never infer the active account from an earlier session. If the user names an account, match both the visible account name and, when available, its profile URL before preparing the draft.

### 2. Select one defensible topic

Prefer a topic that has all of the following:

- Fresh platform interest.
- Material implications for investors.
- Verifiable primary or authoritative sources.
- Room for a specific thesis, counterargument, and measurable follow-up indicators.

Do not select a headline merely because it is sensational. If a platform claim cannot be independently verified, omit it or state the uncertainty explicitly.

### 3. Research current facts

Because market information changes quickly, research the current event before drafting. Prefer company investor relations or newsroom releases, regulatory filings, government data, exchange notices, and other primary sources. Use reputable financial reporting only when primary material does not establish the point.

Verify names, dates, amounts, market reactions, and whether a figure is a target, commitment, order, forecast, or completed transaction. Never convert a proposed or mobilizable amount into booked revenue or an order backlog.

### 4. Draft the article

Use this structure when it suits the subject:

1. A 5–25 character title with a concrete tension or contrarian hook.
2. A short opening that states what happened and why it matters.
3. The verified facts, with important qualifications.
4. The author's own interpretation in first person.
5. The strongest bullish case and the main risk or counterargument.
6. Three to five indicators that can confirm or disprove the thesis.
7. A concise conclusion and a question that invites comments.
8. Relevant hashtags, source links, and a non-investment-advice disclaimer.

Prefer expressions such as「我認為」「我會睇」「唔係」「而家」「對我嚟講」where natural. Avoid forced slang, Mainland promotional jargon, and repetitive emojis.

### 5. Prepare the TTM draft

For a publishing request:

1. Open the long-article editor from the signed-in TTM tab.
2. Fill the title and body without changing their meaning.
3. Add one genuinely relevant platform topic; do not attach an unrelated trending topic only for reach.
4. Leave any autosaved draft intact unless the user explicitly asks to delete it.

### 6. Add relevant images

Choose the thesis before choosing or generating images. Every image must support a specific paragraph, dataset, scenario, or causal chain in the article.

- Prefer an original first image that visually explains the article's core thesis and can serve as the automatic cover.
- When a second news or data image adds evidence, prefer a primary-source chart, filing excerpt, exchange notice, government chart, or other clearly reusable authoritative material.
- Verify reuse rights before uploading an external image. Government material may be reusable, but check the source's stated policy, retain its source line, and avoid protected seals, emblems, or third-party photographs.
- Do not reuse a media outlet's or another TTM author's cover merely because it looks newsworthy.
- Add a factual caption that explains why the image is present and credits the source.
- If the browser upload fails, follow the selected browser's file-upload troubleshooting instructions instead of bypassing its security controls.

After uploading, verify that each image has a hosted TTM URL, renders in preview, appears in the intended position without splitting a sentence, and has the correct caption. Keep the automatic cover when the first image is suitable; use a custom cover only when the user asks or the automatic choice is visibly wrong.

### 7. Preview and optionally run an independent review

Preview the complete article and verify:

- Exact title and visible publishing account.
- Natural Hong Kong Cantonese and a thesis consistent with the author's profile.
- Paragraph order, image placement, image count, captions, sources, topic, and disclaimer.
- Factual values, dates, expectations versus official releases, and any reuse-rights claim.
- For program-trading articles: inputs, thresholds, confirmation, no-trade logic, entry timing, risk, stop, and re-entry rules.

Use a subagent only when the user explicitly requests independent review. Give it read-only instructions, require a `PASS` or `BLOCK` result with concrete reasons, and forbid edits or publishing. Treat any blocking finding as requiring correction and a fresh preview. Treat suggestions as non-blocking unless they affect accuracy, rights, account identity, or the user's requested editorial positioning.

### 8. Confirm and publish safely

Immediately before clicking the final Publish button, tell the user which TTM account will publish the article and ask for explicit confirmation. This confirmation is required even if the earlier request already said to publish.

One narrow exception is allowed: if the user's latest instruction explicitly says to run a final independent review and publish automatically only if it passes, a `PASS` result is the condition that activates that authorization. Publish without another prompt only when the reviewer inspected the exact final preview and nobody changed the draft afterward. Any edit after review invalidates the `PASS` and requires another review or explicit confirmation.

After confirmation, click Publish once. If the page does not immediately navigate, inspect the current URL, open-tab state, notifications, and published-post count before clicking again. Do not create a duplicate post because of a delayed response.

Verify success in stages:

1. Observe the success toast or navigation; never click Publish a second time while the first action may still be processing.
2. Confirm the visible account's Published count increased.
3. If the list is temporarily empty, wait briefly and reload the profile once.
4. Locate the exact title and capture the canonical `/post/<id>` URL.
5. Open the canonical post and verify the title, author, expected image count, relevant topic, and disclaimer.
6. Leave the public post open in Chrome and return its link to the user.

## Boundaries

- If the user asks only for a sample or draft, stop after delivering the draft.
- Never publish, edit, react to, or delete a public post without the required user authorization.
- Do not disclose private browsing, account, or portfolio data in the article.
- Do not promise unattended daily execution. When asked for recurring automation, distinguish this reusable editorial workflow from any scheduler or login-session limitations.
