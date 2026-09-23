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
https://github.com/codepath/pathreview-ai301-fa26-s3/issues/64

**Verdict output**
accept

**The verdict must record `accept` for this issue.** Choose an issue your own skill
accepts. If your skill rejects every candidate you try, that is a signal about your
rubric rather than about the issues: revise it and re-run — retries are unlimited and a
partial re-run costs about $0.20 — or run the skill on different candidates. Output
recording `reject` for the issue you chose earns no credit for this field.

```
Scope check — codepath/pathreview-ai301-fa26-s3 matches the repo named in
  scope.md:17. In field. House rule noted (classmates' claim comments don't
  block); no claims exist on this issue, so it never came into play.

  Rubric — 8 checks, all required, no preferred rows. Verdict rule: accept only
  if every required check passes; fail or unclear → reject.

  Evidence gathered live (gh isn't installed on this machine — I used the GitHub
  REST API via curl instead). All recency measured against today, 2026-09-23.

  ┌─────────────┬───────┬───────────────────────────────────────────────────┐
  │    Check    │ Grade │                     Evidence                      │
  ├─────────────┼───────┼───────────────────────────────────────────────────┤
  │ Active Repo │ pass  │ Last main commit 2026-09-16T21:42:18Z — 7 days    │
  │             │       │ ago, inside 60                                    │
  ├─────────────┼───────┼───────────────────────────────────────────────────┤
  │ Not       │       │ assignees: [], comments: 0, timeline holds 4        │
  │  taken      │ pass  │ labeled events and zero cross-references or       │
  │             │       │ linked PRs                                        │
  ├─────────────┼───────┼───────────────────────────────────────────────────┤
  │             │       │ Title + body name the exact defect: fixture "uses │
  │ Clear task  │ pass  │  query 'Python Django web framework' against a    │
  │             │       │ chunk containing all four query terms, then       │
  │             │       │ asserts the score is below 0.9"                   │
  ├─────────────┼───────┼───────────────────────────────────────────────────┤
  │ Expected       │       │ "Fix the fixture so the overlap is genuinely   │
  │ result is      │ pass  │ partial" — states the post-fix state, against  │
  │ clear          │       │ stated correct behavior ("scorer correctly     │
  │                │       │ returns 1.0 for full keyword coverage")        │
  ├────────────────┼───────┼────────────────────────────────────────────────┤
  │ Helpful        │       │ File tests/unit/test_relevance_scorer.py, test │
  │ details        │ pass  │  name, repro command pytest … -q, observed     │
  │                │       │ failure assert 1.0 < 0.9                       │
  ├────────────────┼───────┼────────────────────────────────────────────────┤
  │ Maintainer     │ pass  │ main commit 2026-09-16, 7 days ago — satisfies │
  │ activity       │       │  the ≥1-commit-in-90-days arm                  │
  ├────────────────┼───────┼────────────────────────────────────────────────┤
  │ Repository in  │ pass  │ Commit 2026-09-16 (7d) AND issue #53 updated   │
  │ use            │       │ 2026-09-22 (1d), both inside 180               │
  ├────────────────┼───────┼────────────────────────────────────────────────┤
  │ Newcomer-sized │ pass  │ One fixture in one test file; no refactor,     │
  │  scope         │       │ migration, or multi-subsystem change described │
  └────────────────┴───────┴────────────────────────────────────────────────┘

  8/8 required pass → accept. Labels bug, good first issue, tests, tier-1;
  opened 2026-09-10 by Aburke225 (author_association: COLLABORATOR).

  Two things your rubric didn't decide, flagged but not scored:

  - Your fit profile is still blank (scope.md:39). It only ranks accepted
  issues, and there's one candidate, so it changed nothing here. It will matter
  the moment you grade two URLs at once.
  - No check covers the fifth surface — the AI-contribution policy from
  references/evidence-guide.md. Your eight checks cover all four lecture
  families cleanly, but an outright AI ban is a documented fail condition your
  rubric currently can't see. Your workflow is AI-assisted, so that's a real gap
  in the rubric, not in this run.

  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/64",
    "checks": [
      {"name": "Active Repo", "grade": "pass", "evidence": "Last default-branch 
  commit 2026-09-16T21:42:18Z, 7 days before today (2026-09-23), within the 
  60-day threshold"},
      {"name": "Not already taken", "grade": "pass", "evidence": "assignees: [],
  comments: 0, and the issue timeline contains only 4 'labeled' events — no 
  linked PRs or claim comments"},
      {"name": "Clear task", "grade": "pass", "evidence": "Body: test 'uses 
  query \"Python Django web framework\" against a chunk containing all four 
  query terms, then asserts the score is below 0.9'"},
      {"name": "Expected result is clear", "grade": "pass", "evidence": "Body: 
  'Fix the fixture so the overlap is genuinely partial', against stated correct 
  behavior 'The scorer correctly returns 1.0 for full keyword coverage'"},
      {"name": "Helpful details", "grade": "pass", "evidence": "Body names file 
  tests/unit/test_relevance_scorer.py, test test_query_with_partial_overlap, 
  repro 'pytest tests/unit/test_relevance_scorer.py -q', and failure 'assert 1.0
  < 0.9'"},
      {"name": "Maintainer activity", "grade": "pass", "evidence": "Default 
  branch has a commit at 2026-09-16T21:42:18Z, 7 days ago, satisfying the 90-day
  commit arm"},
      {"name": "Repository in use", "grade": "pass", "evidence": "Default-branch
  commit 2026-09-16 (7d ago) and issue #53 updated 2026-09-22 (1d ago), both 
  within 180 days"},
      {"name": "Newcomer-sized scope", "grade": "pass", "evidence": "Scope is 
  one test fixture in one file; body describes no refactor, migration, or change
  spanning multiple subsystems"}
    ],
    "verdict": "accept"
  }

```

---

## Eval iterations

Quote source text directly in each field below. Paraphrase does not satisfy them.

**Run history**

1. Full run: "agreement: 15/20 scored items"
2. issue-12 re-run: "agreement: 1/1 scored items"
3. issue-01 re-run: "agreement: 0/1 scored items"
4. issue-01 re-run after changing the scope check: "agreement: 0/1 scored items"
5. issue-01 re-run after revising the scope check again: "agreement: 1/1 scored items"
6. issue-04 re-run: "agreement: 0/1 scored items"
7. issue-04 re-run after changing the clarity checks: "agreement: 1/1 scored items"
8. issue-16 re-run: "agreement: 1/1 scored items"
9. issue-19 re-run: "agreement: 0/1 scored items"
10. issue-19 re-run after changing the scope check: "agreement: 1/1 scored items"
11. Full run: "agreement: 19/20 scored items"
12. Final saved run: "agreement: 20/20 scored items"

**Issue analysis**

Issue: issue-01

My rubric's verdict: accept

Gold label: accept

The issue asks for one main documentation task, even though it affects several related documentation files. The issue says, "We should add a stable docs location for the GA workflow and update the existing pages that currently mention older or temporary guidance." My earlier scope check treated several files as too large, which caused the issue to be rejected. I changed the check so that several related files can still count as one focused task. With the revised check, the rubric accepted the issue, matching the gold label.

**Check rationale**

"Pass if the issue is centered on one bug or feature, even if the issue lists several possible causes or implementation ideas. Fail only if it requires multiple unrelated tasks, a repo-wide migration, or a broad redesign."

I changed this check because counting the number of files or possible fixes was too strict. A first issue can still be focused even if it affects several related files or lists more than one possible solution. I wanted the check to focus on whether the work is one main task instead of simply how many files or ideas are mentioned.

**Trade-offs**

This check may accept an issue that is technically difficult as long as all of the work is centered on one bug or feature. For example, issue-19 says, "There are two potential causes which should be fixed:" and then lists multiple implementation ideas. My earlier version rejected it because it looked too broad. The revised check accepts it because all of those ideas are related to the same UI-freezing bug. The trade-off is that the rubric is less strict about complexity in order to avoid rejecting focused issues just because they have several possible causes or fixes.

---

## Selection rationale

Graded on whether all three are answered, in your own words. Not on how good the
reasoning is, and not on length — a short honest answer to each earns the full marks.
This is also the basis for the claim comment you write in Unit 2.

**Selection rationale**

1. This issue fits my interests because it involves testing and a relevance-scoring bug, which is related to software and AI systems. It also looks manageable within the time available because the issue focuses on fixing one test fixture in one test file.

2. The verdict correctly identified that the repository is active, the task is clear, the expected result is understandable, the scope is focused, and there is no existing assignee or linked pull request. I also considered that the issue is labeled "good first issue" and "tier-1," which made it seem appropriate for a first contribution.

3. I expect the claiming process to be fairly straightforward because the issue currently has no assignee, no comments, and no linked pull request. The main difficulty will probably be understanding the existing test and making sure I reproduce the failure correctly before changing anything.

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
