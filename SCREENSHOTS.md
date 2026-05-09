# Screenshots needed

Drop each PNG into `images/` with the **exact filename** below. The placeholder
in the page automatically swaps in the real image as soon as the file exists at
that path — no code edits required.

PNG preferred. ~1400px wide is plenty (page max is 980px).

## Perplexity (5)

| Filename | What to capture |
|---|---|
| `perp_01_home.png` | Perplexity homepage with the search bar centred. Show the focus pills (Web · Academic · Social) under the input. |
| `perp_02_search.png` | A normal Search Mode answer with 3-5 numbered citations next to facts. |
| `perp_03_deep.png` | The Deep Research toggle highlighted under the input box. |
| `perp_04_learn.png` | Learn Mode in a query — flashcards or step-by-step explanation. |
| `perp_05_deep_running.png` | "Deep Research running…" with the live list of sources being read. |

## Gemini · Music (3)

| Filename | What to capture |
|---|---|
| `gem_01_home.png` | Gemini home — "Hello — what should we create today?" + input box. |
| `gem_02_tools_menu.png` | Tools dropdown open, with "Create music" highlighted. |
| `gem_03_track_ready.png` | Generated track UI — play button, waveform, cover art, download icon. |

## Suno (3)

| Filename | What to capture |
|---|---|
| `suno_01_home.png` | Suno landing or signed-in home with the "Create" button visible. |
| `suno_02_custom.png` | Custom mode with Lyrics + Style + Title fields filled. Vocals toggle visible. |
| `suno_03_library.png` | Library showing the two newly-generated versions of your song. |

## Claude.ai (2)

| Filename | What to capture |
|---|---|
| `claude_01_chat.png` | Claude.ai chat home — input box + Projects sidebar on the left. |
| `claude_02_project.png` | A Project view with knowledge files uploaded + custom instructions filled. |

## Claude Code · landing-page flow (10)

This is the longest sequence — each shot covers one moment in the resume → landing-page flow.

| Filename | What to capture |
|---|---|
| `cc_01_new_session.png` | Claude Code on the web — chat on left, empty preview pane on right. |
| `cc_02_attach.png` | Resume PDF attached to the chat, ready to send. |
| `cc_03a_thinking.png` | Claude reading your resume — "Thinking…" or planning state in the chat. |
| `cc_03b_writing_code.png` | Claude actively writing the HTML — code streaming in the chat. |
| `cc_03c_preview.png` | Preview pane: hero with name + tagline + about visible. |
| `cc_03d_full_page.png` | Scrolled preview showing Experience, Skills, Projects, Contact. |
| `cc_04a_iteration.png` | A follow-up message ("make hero bigger…") + updated preview. |
| `cc_04b_download.png` | Download button (or "Copy code" on the code block) — the export action. |
| `cc_05a_saved_file.png` | The saved `index.html` in your Downloads folder / Desktop. Filename visible. |
| `cc_05b_local_preview.png` | The downloaded `index.html` opened locally in your browser (URL = `file:///…`). |

## GitHub (5)

| Filename | What to capture |
|---|---|
| `gh_01_signup.png` | GitHub signup page, or the signed-in dashboard with "+ New" top-right. |
| `gh_02_new_repo.png` | "Create a new repository" form — repo name filled, Public selected. |
| `gh_03a_upload_zone.png` | The empty drag-and-drop upload zone. |
| `gh_03b_file_added.png` | After dragging — `index.html` listed, commit button visible. |
| `gh_03c_committed.png` | Repo home with `index.html` in the file list + latest commit message. |

## GitHub Pages (3)

| Filename | What to capture |
|---|---|
| `pg_01_settings.png` | Repo Settings → Pages screen, before any source has been picked. |
| `pg_02_branch.png` | Branch picker showing `main` + `/(root)`, Save button highlighted. |
| `pg_03_live.png` | The green "Your site is live at https://username.github.io/repo/" banner. |

## Total — 31 screenshots

Capture order doesn't matter — placeholders are independent. Page works fine
with partial coverage (any not-yet-captured shots stay as visible placeholder
boxes so you can see exactly what's still pending).

## How the swap works

Every `<figure class="ph">` has both:
- a placeholder block (`.ph-info`) shown by default
- a hidden `<img class="ph-img" src="images/...">` with `onload`/`onerror` handlers

When the image loads, `.has-image` is added → placeholder hides, image shows.
When it fails (file missing) → placeholder stays. Pure HTML/CSS, no build step.
