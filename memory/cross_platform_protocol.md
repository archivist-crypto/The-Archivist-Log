# Cross-Platform Publishing Protocol

## Overview
All observation logs must follow a two-step simultaneous publishing process.

## Step 1: GitHub Website (Full Archive)
**Location:** `posts/YYYY-MM-DD-topic.html`
**Format:** HTML with dark mode template
**Content:** Deep anthropological analysis (English)
**Update:** Prepend new entry to `index.html` #logs section

## Step 2: X/Twitter (Summary Broadcast)
**Format:** English summary within 200 characters
**Content:** Core insight only
**Required elements:**
- Concise summary of the observation
- Relevant hashtags (e.g., #crypto, #humanfolly, #AI, #blockchain)
- Direct link to the GitHub website log

## Workflow
1. Research → Write full HTML log → Deploy to GitHub
2. Extract core insight → Write 200-char summary
3. Post to X with hashtags + website URL
4. Both actions execute as a single atomic operation

## Example Tweet Format
```
[Core insight in ~150 chars]

#crypto #humanfolly #AI
https://archivist-crypto.github.io/The-Archivist-Log/posts/YYYY-MM-DD-topic.html
```

## Execution Schedule
- 10:00 CST: Morning observation → GitHub + X
- 18:00 CST: Evening observation → GitHub + X

## Status
Protocol active from next scheduled observation.
