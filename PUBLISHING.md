# Publishing Guide

End-to-end steps for publishing this repo to `github.com/jukkablomberg/finnish-bitcoin-reserve` and producing the v0.2 release. Reuse for future versions.

Total time: ~30 minutes including CI wait.

---

## 0. Pre-flight (one-time, 5 min)

Verify your environment in Terminal:

```bash
git --version              # any modern git is fine
gh --version               # optional but helpful; install via `brew install gh`
gh auth status             # if installed, confirm you're logged in as jukkablomberg
```

If `gh` is not installed, you can do every step via the GitHub web UI instead — the CLI just saves clicks. Install with `brew install gh && gh auth login` if you want it.

---

## 1. Initialize git in the local folder (3 min)

```bash
cd "/Users/jukka/Second Brain/finnish-bitcoin-reserve"

# Initialize the repo with main as default branch
git init -b main

# Sanity-check what git sees
git status

# Stage everything
git add .

# First commit
git commit -m "Initial publication: v0.2 — Finland's Path to a Sovereign Bitcoin Reserve"
```

You should see a commit with all the files (README, LICENSE, CITATION.cff, the whitepaper, distribution kit, the workflow, etc.).

---

## 2. Create the GitHub repo (2 min)

**Option A — via `gh` CLI (recommended):**

```bash
gh repo create jukkablomberg/finnish-bitcoin-reserve \
  --private \
  --description "Policy whitepaper: Finland's Path to a Sovereign Bitcoin Reserve. Operating model, custody, political sequencing. CC-BY 4.0." \
  --homepage "https://northpoint.fi/whitepapers/finnish-bitcoin-reserve" \
  --source=. \
  --remote=origin \
  --push
```

This creates the repo *as private*, sets the remote, and pushes in one shot. We'll flip to public in step 7, after verifying the PDF build works.

**Option B — via the GitHub web UI:**

1. Go to https://github.com/new
2. Repository name: `finnish-bitcoin-reserve`
3. Description: *"Policy whitepaper: Finland's Path to a Sovereign Bitcoin Reserve. Operating model, custody, political sequencing. CC-BY 4.0."*
4. Visibility: **Private** for now
5. Leave "Initialize this repository with…" unchecked (we already have files locally)
6. Click *Create repository*
7. Back in Terminal:
   ```bash
   git remote add origin https://github.com/jukkablomberg/finnish-bitcoin-reserve.git
   git push -u origin main
   ```

---

## 3. Watch the first Actions run (5 min)

The first push to `main` triggers the PDF build workflow.

```bash
# CLI way: watch the run in your terminal
gh run watch
```

Or open https://github.com/jukkablomberg/finnish-bitcoin-reserve/actions in a browser.

The build installs pandoc + xelatex and renders `en/whitepaper.md` → PDF. Expect ~3-5 minutes.

When it completes:

```bash
# Download the PDF artifact to inspect it locally
gh run download --name whitepaper-pdf -D /tmp/wp-check
open /tmp/wp-check/finnish-bitcoin-reserve-en.pdf
```

**This is the quality check.** Open the PDF. Look for:
- TOC renders correctly
- Footnotes render correctly
- Section numbering matches what's in the markdown
- No obviously broken layouts
- Font (Noto Serif) renders cleanly
- A4 page size

If anything is wrong, fix it in the markdown, commit, push — the workflow re-runs automatically.

---

## 4. Create the v0.2 release (2 min)

Once the PDF looks good, tag a release. This triggers the same workflow but attaches the PDF to the release automatically.

```bash
git tag -a v0.2 -m "v0.2 — Restructured opening around Sweden's naming of Finland; Section 2 folded into Track A"
git push origin v0.2
```

Then create the release itself:

**Option A — via `gh`:**
```bash
gh release create v0.2 \
  --title "v0.2 — Initial public release" \
  --notes "First public release of the whitepaper. Three-track operating model (governance framework / legal mechanism / strategic allocation), three-tier custody architecture, political sequencing across Finnish parties, replies to five counter-arguments, and three concrete 2026 moves. Published under CC-BY 4.0." \
  --latest
```

**Option B — via GitHub UI:**
1. https://github.com/jukkablomberg/finnish-bitcoin-reserve/releases/new
2. Tag: `v0.2`
3. Title: `v0.2 — Initial public release`
4. Description: paste the same notes as above
5. Tick "Set as the latest release"
6. Click *Publish release*

The workflow re-runs on the release event and attaches `finnish-bitcoin-reserve-en.pdf` to the release within ~5 minutes.

After it completes, this URL will work permanently:
```
https://github.com/jukkablomberg/finnish-bitcoin-reserve/releases/latest/download/finnish-bitcoin-reserve-en.pdf
```

This is the URL you put on the northpoint.fi landing page.

---

## 5. Repo polish (5 min)

In the GitHub web UI, on the repo's main page:

**About box (top-right):**
- Description: *"Policy whitepaper: Finland's Path to a Sovereign Bitcoin Reserve. Operating model, custody, political sequencing. CC-BY 4.0."*
- Website: `https://northpoint.fi/whitepapers/finnish-bitcoin-reserve`
- Topics (tag-style keywords for discoverability): `bitcoin`, `finland`, `monetary-policy`, `sovereign-reserves`, `cryptocurrency`, `eduskunta`, `nordic-policy`, `whitepaper`, `policy`, `mica`
- Tick: *Releases*, *Packages*
- Untick: *Deployments* (not relevant)

**Social preview image (optional but worth doing):**
- Settings → General → scroll to *Social preview*
- Upload a 1280×640 PNG. If you don't have one, GitHub generates a default from the README. You can produce one in 60 seconds with Canva or Figma — title + author + the URL on a clean background.

**Branch protection (optional but professional):**
- Settings → Branches → Add rule for `main`
- Tick *Require a pull request before merging* — this means anyone else (or you, in a fork) cannot push directly to main. PRs only. Optional for solo work.

---

## 6. Verify the workflow attached the PDF (1 min)

Visit https://github.com/jukkablomberg/finnish-bitcoin-reserve/releases/latest

You should see a "Assets" section with `finnish-bitcoin-reserve-en.pdf` listed. Click it once to verify it downloads. If it's not there yet, wait — the release workflow may still be running.

Confirm the permanent URL works:
```bash
curl -ILs "https://github.com/jukkablomberg/finnish-bitcoin-reserve/releases/latest/download/finnish-bitcoin-reserve-en.pdf" | head -5
```

You want a `200` or `302 → 200` response, not `404`.

---

## 7. Flip to public (10 seconds)

When everything looks right:

```bash
gh repo edit --visibility public --accept-visibility-change-consequences
```

Or in UI: Settings → General → scroll all the way down → *Change visibility* → Make public → confirm.

**Once public**, the repo URL is the canonical citation target everywhere.

---

## 8. Wire the landing page (5 min — separate from the repo work)

In `landing-page/index.html`, three placeholders need to be resolved when you deploy this onto northpoint.fi:

- `{{LATEST_PDF_URL}}` → `https://github.com/jukkablomberg/finnish-bitcoin-reserve/releases/latest/download/finnish-bitcoin-reserve-en.pdf`
- `{{REPO_URL}}` → `https://github.com/jukkablomberg/finnish-bitcoin-reserve`
- `{{EMAIL_ENDPOINT}}` → your existing NorthPoint newsletter form handler (Buttondown, ConvertKit, whatever you currently use for the Substack signups, or just point at the existing NorthPoint newsletter signup page)

After deploying, smoke-test by clicking *Download the PDF* on the landing page and confirming it pulls from the GitHub release.

---

## 9. You're live

After step 7 + 8, the publication is technically complete. The order to launch publicly is then:

1. Send embargoed press pitch (`distribution/press-pitch-email.md`) to ~12 journalists 48h before the public launch
2. Send Eduskunta + Suomen Pankki cover emails individually
3. Public-launch day, 09:00 Helsinki: tweet thread (`distribution/tweet-thread.md`) goes live, pinned to profile
4. 09:30 Helsinki: LinkedIn essay (`distribution/linkedin-post.md`)
5. Cross-post via the 4-channel routine: NorthPoint Substack + Medium + Dev.to + LinkedIn
6. Reply to first 10 comments / quote-tweets within 2 hours

The 7-day decision gate after public launch: ≥100 GitHub stars, ≥500 PDF downloads, ≥1 press mention, ≥1 contact from Eduskunta/Suomen Pankki → operationalize. Less → permanent citable artifact.

---

## For future versions (v0.3, v0.4, …)

Same flow, shorter:

```bash
cd "/Users/jukka/Second Brain/finnish-bitcoin-reserve"
# … make your edits in en/whitepaper.md and elsewhere …
git add .
git commit -m "v0.3 — what changed"
git push
git tag -a v0.3 -m "v0.3 — what changed"
git push origin v0.3
gh release create v0.3 --title "v0.3" --notes "What changed in this version." --latest
```

The PDF auto-builds and attaches. Bump the `version` field in CITATION.cff and the metadata at the top/bottom of `en/whitepaper.md` to match.
