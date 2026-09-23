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
| Active Repo | Checking recent commit dates | Pass if there is a commit in the last 60 days | Required |
| Not already taken | Issue body and comment thread | Pass if nobody has clearly said they are currently working on the issue | Required |
| Clear task | Issue title and issue body | Pass if the issue identifies a specific bug, missing behavior, or requested change, even if the description is brief. | required |
| Expected result is clear | Issue title and issue body | Pass if the desired result can be reasonably understood from the issue title and body, even if it is not written as a separate expected-result statement. | required |
| Helpful details | Issue body | Pass if the issue gives at least one useful detail such as an error message, example, file name, screenshot, etc | required |
| Maintainer activity | Repo-facts block: dates of the last 5 commits on the default branch; issue comment thread: dates of maintainer comments | Pass if the default branch has at least 1 commit within the last 90 days OR a maintainer has commented on the issue within the last 90 days | required |
| Repository in use | Repo-facts block: dates of the last 5 default-branch commits and recent issue/PR activity listed by the skill | Pass if there has been at least 1 default-branch commit within the last 180 days and at least 1 issue or pull request activity within the last 180 days. | required |
| Newcomer-sized scope | Issue title and issue body | Pass if the issue is centered on one bug or feature, even if the issue lists several possible causes or implementation ideas. Fail only if it requires multiple unrelated tasks, a repo-wide migration, or a broad redesign. | required |
| AI contribution policy | AI/contribution policy locations listed in references/evidence-guide.md | Pass if the repository does not prohibit AI-assisted contributions. Fail if the repository explicitly bans AI-assisted contributions. | required |



## Verdict rule

<!-- State how the grades above combine into accept or reject, and how
unclear is treated. Example shape (write your own): "accept if every
required check passes; preferred checks never change the verdict, they
rank accepted issues; unclear counts as fail." -->

Accept only if every required check passes. If a required check fails or is unclear, reject the issue.