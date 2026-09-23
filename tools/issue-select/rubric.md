# Rubric: is this a good first issue?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever checks
you define here. It ships empty on purpose: the judgment is your work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four columns:
   - Check: a short name (used in the output JSON).
   - Evidence: exactly what to look at, and where. Name the source
     (repo-facts block, issue body, comment thread, or the locations in
     references/evidence-guide.md). "The repo" is not a source; "the last
     5 default-branch commit dates" is.
   - Pass condition: a condition someone else could apply and get your
     answer. Prefer thresholds with numbers ("a maintainer commented
     within 30 days") over adjectives ("maintainer is responsive").
   - Weight: `required` (a fail here rejects the issue) or `preferred`
     (never changes the verdict; a nice-to-have that helps rank the
     issues you accept).

2. A verdict rule below the table: how the check grades combine into
   accept or reject, including how `unclear` is treated. The verdict
   space is binary. If you write no rule for `unclear`, the skill treats
   it as fail.

Cover what actually kills first contributions. The lecture named four
families: the maintainer is alive, the repo is in use, the scope fits a
newcomer, and nobody else is already on it. A rubric that ignores a family
will fail eval issues designed around that family.
-->

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| maintainer_alive | Date of the most recent commit on the default branch (repo-facts block / repo homepage) | There was a commit within the last 30 days | required |
| repo_in_use | Date of the last push to any branch (repo-facts block / repo homepage or Branches tab) | There was activity within the last 60 days | required |
| scope_fits_newcomer | Issue body (title + description) and the comment thread | The issue targets one cohesive outcome. It still passes when reaching that outcome needs several related edits, checklist items, or named examples (e.g., updating multiple doc pages for one feature, or listing several example cases under one bug/feature) — as long as those pieces are not independently assignable. It fails only when: (a) the issue is an explicit tracking list of several unrelated GitHub issue numbers or separate feature requests meant to be claimed independently, or (b) the thread shows the design is still being actively debated with no maintainer decision. | required |
| unclaimed | Issue's assignees field, and any linked PRs (Development box / repo-facts block) | No assignee is set, and no linked PR is open. (Per Path Review house rule in scope.md: classmates' "working on this" comments do not count as a claim.) | required |
| contribution_policy | CONTRIBUTING.md, AI_USAGE_POLICY.md, AGENTS.md, or the "contribution policy" line under Repo facts | The policy does not state an outright ban on AI-generated contributions. (Disclosure/testing/review conditions are fine and pass; silence also passes.) | required |

## Verdict rule

Accept only if all five required checks pass. If any check fails, or its evidence is unclear, the issue is rejected. `unclear` on a required check counts as fail.

<!-- State how the grades above combine into accept or reject, and how
unclear is treated. Example shape (write your own): "accept if every
required check passes; preferred checks never change the verdict, they
rank accepted issues; unclear counts as fail." -->