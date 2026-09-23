# Unit 1 — Issue Selection

Path: `beat-1-sandbox/unit-1/selection.md`

Record of the issue carried into Unit 2, and of the evaluation runs that produced
`eval-run.txt`. This file is graded at the path above; a copy kept anywhere else in
the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the
wrong label is not graded.

---

## Selected issue

**Issue link**

https://github.com/codepath/pathreview-ai301-fa26-s1/issues/72

**Verdict output**

**The verdict must record `accept` for this issue.**

````
Skill(issue-select)
Successfully loaded skill

I'll read the rubric and scope, then gather evidence on all three issues in parallel.

Read 2 files, ran 1 shell command

Now I'll fetch all three issues and repo metadata in parallel.

Ran 4 shell commands

No gh CLI. I'll use WebFetch via the GitHub API instead.

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1/issues/73)
Received 239KB (200 OK)

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1/issues/72)
Received 269KB (200 OK)

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1/issues/69)
Received 250KB (200 OK)

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1/commits/main)
Received 481.8KB (200 OK)

Now let me check the contribution policy files.

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1/blob/main/CONTRIBUTING.md)
Received 0 bytes (404 Not Found)

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1/blob/main/AI_USAGE_POLICY.md)
Received 0 bytes (404 Not Found)

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1)
Received 296.6KB (200 OK)

Fetch(https://github.com/codepath/pathreview-ai301-fa26-s1/blob/main/docs/CONTRIBUTING.md)
Received 292.3KB (200 OK)

I have all the evidence. Let me compile the grades for each issue.

---
Grading Summary

Repo health (applies to all three): Most recent commit Sep 16, 2026 (7 days ago) → maintainer_alive OK | repo_in_use OK. Policy: docs/CONTRIBUTING.md is silent on AI-generated contributions OK.

---
Issue #73 — README and .env.example disagree about which LLM API key to set

- maintainer_alive: pass — last commit Sep 16, 2026 (7 days ago)
- repo_in_use: pass — same
- scope_fits_newcomer: pass — single cohesive docs fix: align README and .env.example on OPENROUTER_API_KEY; no active design debate
- unclaimed: pass — no assignees, no linked PRs
- contribution_policy: pass — CONTRIBUTING.md silent on AI; silence passes

Verdict: ACCEPT

---
Issue #72 — verify_password raises UnknownHashError instead of returning False

- maintainer_alive: pass — last commit Sep 16, 2026 (7 days ago)
- repo_in_use: pass — same
- scope_fits_newcomer: pass — single fix: catch UnknownHashError in core/security.py, return False, remove one @pytest.mark.xfail marker from test_security.py; no debate
- unclaimed: pass — no assignees, no linked PRs
- contribution_policy: pass — CONTRIBUTING.md silent on AI

Verdict: ACCEPT

---
Issue #69 — Output parser crashes on a top-level JSON array fallback

- maintainer_alive: pass — last commit Sep 16, 2026 (7 days ago)
- repo_in_use: pass — same
- scope_fits_newcomer: pass — single fix: handle top-level JSON array in rag/generator/output_parser.py, remove one @pytest.mark.xfail marker from test_output_parser.py; no debate
- unclaimed: pass — no assignees, no linked PRs
- contribution_policy: pass — CONTRIBUTING.md silent on AI

Verdict: ACCEPT

---
Fit ranking (all three accepted)

Your profile: wants Python practice, avoid complexity

1. #72 (top pick) — Python exception handling in core/security.py, one file to change plus one test marker to remove. Builds Python skills with minimal risk of getting stuck.
2. #73 — Pure docs fix (README + .env.example), 1-2 hrs, easiest possible first touch but least Python practice.
3. #69 — Python output-parser bug, 2-4 hrs. Good Python practice but meaningfully more work and the RAG pipeline adds conceptual overhead.

[
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s1/issues/72",
    "checks": [
      {"name": "maintainer_alive", "grade": "pass", "evidence": "Most recent commit: Sep 16, 2026 (7 days ago), within 30-day window"},
      {"name": "repo_in_use", "grade": "pass", "evidence": "Last push Sep 16, 2026 (7 days ago), within 60-day window"},
      {"name": "scope_fits_newcomer", "grade": "pass", "evidence": "Single fix: catch UnknownHashError in core/security.py, return False, remove one xfail marker; no active design debate"},
      {"name": "unclaimed", "grade": "pass", "evidence": "Assignees: none; linked PRs: none"},
      {"name": "contribution_policy", "grade": "pass", "evidence": "docs/CONTRIBUTING.md makes no mention of AI-generated contributions; silence passes"}
    ],
    "verdict": "accept"
  },
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s1/issues/73",
    "checks": [
      {"name": "maintainer_alive", "grade": "pass", "evidence": "Most recent commit: Sep 16, 2026 (7 days ago), within 30-day window"},
      {"name": "repo_in_use", "grade": "pass", "evidence": "Last push Sep 16, 2026 (7 days ago), within 60-day window"},
      {"name": "scope_fits_newcomer", "grade": "pass", "evidence": "Single cohesive docs fix: align README.md and .env.example on OPENROUTER_API_KEY; no design debate"},
      {"name": "unclaimed", "grade": "pass", "evidence": "Assignees: none; linked PRs: none"},
      {"name": "contribution_policy", "grade": "pass", "evidence": "docs/CONTRIBUTING.md makes no mention of AI-generated contributions; silence passes"}
    ],
    "verdict": "accept"
  },
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s1/issues/69",
    "checks": [
      {"name": "maintainer_alive", "grade": "pass", "evidence": "Most recent commit: Sep 16, 2026 (7 days ago), within 30-day window"},
      {"name": "repo_in_use", "grade": "pass", "evidence": "Last push Sep 16, 2026 (7 days ago), within 60-day window"},
      {"name": "scope_fits_newcomer", "grade": "pass", "evidence": "Single fix: handle top-level JSON array in rag/generator/output_parser.py, remove one xfail marker; no active debate"},
      {"name": "unclaimed", "grade": "pass", "evidence": "Assignees: none; linked PRs: none"},
      {"name": "contribution_policy", "grade": "pass", "evidence": "docs/CONTRIBUTING.md makes no mention of AI-generated contributions; silence passes"}
    ],
    "verdict": "accept"
  }
]
````

---

## Eval iterations

**Run history**

1. Smoke run (--limit 3): 2/3 agreement
2. First full run (--save-run): 14/20 (category floor unmet — no match in `policy`)
3. After adding `contribution_policy` check + rewording `scope_fits_newcomer` (--only issue-01,04,06,12,15,19): 2/6
4. After refining `scope_fits_newcomer` again (--only issue-01,04,19,10,15): 4/5
5. Final full run (--save-run, committed as eval-run.txt): 17/20 — category floor met in all 5 categories, one below the 18/20 bar (issue-14 and issue-19 failed `maintainer_alive`; manual date-check confirmed both commits are well within the 30-day window, so this looks like a model misread rather than a rubric flaw)

**Issue analysis**

issue-15 (zulip/zulip#19589): gold label is `reject`, my rubric graded `accept`. The issue proposes separating Slack-webhook `command`/`text` fields — one coherent feature, but its 97-comment thread (open since 2021, multiple contributors claimed and abandoned it) shows the design was never settled by a maintainer. My `scope_fits_newcomer` check, after I broadened it to stop rejecting legitimate multi-part single-task issues, no longer reliably caught this "long-unsettled design" pattern.

**Check rationale**

`scope_fits_newcomer`: "The issue targets one cohesive outcome. It still passes when reaching that outcome needs several related edits, checklist items, or named examples... It fails only when: (a) the issue is an explicit tracking list of several unrelated GitHub issue numbers or separate feature requests meant to be claimed independently, or (b) the thread shows the design is still being actively debated with no maintainer decision." I wrote it this way after my first version wrongly rejected 3 valid issues (issue-01, issue-04, issue-19) for having multiple related parts under one task.

**Trade-offs**

Broadening clause (b) to allow multi-part-but-single-task issues traded false rejects for a false accept: it fixed issue-01, issue-04, and issue-19, but let issue-15 slip through, since its "still debated" signal is buried in a 97-comment thread rather than stated plainly. A version of (b) that weighs debate length/inconclusiveness, not just presence, would likely catch issue-15 without losing the other three — I didn't have time/budget to test that iteration.

---

## Selection rationale

**Selection rationale**

1. #72 is a bounded Python exception-handling fix (~1-2 hrs), matching my interest in practicing Python and my preference to avoid complex issues, and it fit the time I had tonight.
2. The verdict correctly confirmed no claims/assignees, an active maintainer, and a silent AI policy. Beyond the rubric, I weighed that #72 gives more Python practice than #73 (pure docs) without the added RAG-pipeline complexity of #69.
3. Low difficulty: a single-file fix in `core/security.py` plus removing one `@pytest.mark.xfail` marker, no competing claims or linked PRs to navigate.

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
