# Test repo E — Trail Journal

A valid, self-contained website with exactly one commit, testing the smallest supported history.

**Expected compatibility result: Accept · one version only.**

- Default-branch commits: **1**.
- Commit numbers below are **oldest first**, starting at 1.
- This is a synthetic Git Gallery fixture, not an organic production history.
- Expected outcomes below describe the application requirements, not a claim that Git Gallery integration tests have passed.

## Pages at the latest commit

`index.html`

## Test cases and expected results

### One version is enough

**Target page:** `index.html`  
**Commit numbers:** 1.

Compatibility passes. Select the only commit once. Capture produces Complete status and one viewable timeline entry with matching metadata.

### No invented comparison

**Target page:** `index.html`  
**Commit numbers:** 1.

Do not duplicate the single version, invent another commit, or enable a two-version comparison. Explain that two distinct successful captures are required.

## Important fixture rules

- Keep exactly one commit, including this README.
- This fixture does not test visual evolution; it tests the one-version workflow.

## Local preview

Serve this directory with `python3 -m http.server 8000`, then open http://localhost:8000. The site uses only local HTML, CSS, JavaScript, and original SVG assets. No build step, API, external font, account, or secret is needed.

## Preserve the test

Do not append setup or documentation commits casually: the default-branch count is part of this test. Count with `git rev-list --count main`. List the history oldest first with `git log --reverse --format="%h %s" main`.

The README contains test guidance and expected answers. AI evaluation using this repo is therefore not a blind benchmark; judge visual claims against screenshots and website changes, not this document alone.
