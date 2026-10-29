# GitHub setup

## Prepared locally

The local folder is `systembio-journal-club`. Suggested remote repository name: `journal-club`, under the intended SystemBio account or organization. Confirm the exact GitHub owner when creating the repository; this package does not assume an existing account URL.

Display name: **SystemBio Journal Club**

Suggested description:

> A journal club for biology, health, medicine, and neuroscience, with curated Nature Portfolio papers and open scientific discussion.

The package contains 12 citation-checked candidates, four topic views, a Time Series collection, forum forms, an actionable issue form, a PR template, and a label manifest.

**Remote state:** No repository, hosted discussion, label, or category has been created by preparing these files.

## Activate the repository

1. Create the repository under the intended owner with the chosen visibility. Upload or push only this folder's contents to the root of the default branch.
2. Enable **Discussions** and **Issues** in repository settings.
3. Create the four categories below. Use the exact category names and verify their slugs against the template filenames.
4. Create the labels in `.github/labels.json`. This file is a setup manifest, not an automatically applied GitHub configuration.
5. Open each category's new-discussion form and check that its fields render correctly.
6. Publish and pin a welcome discussion explaining the scope, English-language policy, and how to join.
7. Open an initial paper discussion from a catalog entry. Copy its real URL into the catalog.
8. Create a Journal Club session only when its date and participants are known.

Repository creation, category creation, and publishing welcome or paper posts are separate hosted actions. Discussion forms become available only when the matching categories exist and the files are on the default branch.

## Discussion categories

| Name | Slug / template filename | Format | Purpose |
| --- | --- | --- | --- |
| Paper Discussions | `paper-discussions.yml` | Open-ended | One ongoing conversation per paper |
| Journal Club | `journal-club.yml` | Open-ended | Agendas, paper links, and meeting notes |
| Cross-Paper Insights | `cross-paper-insights.yml` | Open-ended | Evidence-based comparisons across papers |
| Questions & Help | `questions-help.yml` | Question and answer | Focused questions and explanations |

Verify the generated slug for **Questions & Help** in GitHub before activation; rename its form file if GitHub produces a different slug. Pin the welcome post in Journal Club. Remove or repurpose unused default categories to keep navigation focused.

Scientific topics are labels and repository folders, not separate forum categories. A paper spanning health and neuroscience should still have one discussion.

## Labels

- Topics: `topic:biology`, `topic:health`, `topic:general-medicine`, `topic:neuroscience`.
- Collection: `collection:time-series`.
- Reading state: `reading:proposed`, `reading:scheduled`, `reading:discussed`. Use one current state per paper.
- Contribution: `contribution:method`, `contribution:discovery`, `contribution:resource`, `contribution:evaluation`, `contribution:association`, `contribution:prediction`, `contribution:theory`.
- Tasks: `task:follow-up`.

Form dropdowns record information in the post body; they do **not** dynamically apply topic labels. A maintainer applies those labels. Forms intentionally do not require pre-existing labels to render.

## Roles

- **Maintainers:** manage the catalog, labels, categories, and PR review.
- **Presenters:** provide reading context and lead the meeting.
- **Participants:** ask questions, reply, and contribute evidence.
- **Recorder:** summarize the session and preserve unresolved disagreements.

For public repositories, GitHub users can join accessible discussions without write access. For private repositories, invite participants with the needed repository access.

## Launch checks

- All community-facing content is in English.
- The four category forms render on GitHub.
- The issue form and PR template render.
- The 12 catalog entries retain working DOI links.
- Discussion URLs are added only after their threads exist.
- No parent-folder corpus, PDFs, datasets, or unrelated project files are included.

## GitHub documentation

- [About Discussions](https://docs.github.com/en/discussions/collaborating-with-your-community-using-discussions/about-discussions)
- [Category forms](https://docs.github.com/en/discussions/managing-discussions-for-your-community/syntax-for-discussion-category-forms)
- [Issue forms](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms)
