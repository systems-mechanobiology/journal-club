# GitHub setup and maintenance

## Live repository

The public repository is [systems-mechanobiology/journal-club](https://github.com/systems-mechanobiology/journal-club). The local folder is `systembio-journal-club`; the default branch is `main`.

Display name: **SystemBio Journal Club**

Repository description:

> A journal club for biology, health, medicine, and neuroscience, with curated Nature Portfolio papers and open scientific discussion.

The package contains 12 citation-checked candidates, four topic views, a Time Series collection, forum forms, an actionable issue form, a PR template, and a label manifest.

**Configuration applied on 2026-10-29:** Discussions and Issues are enabled; the four categories below and the 16 labels in `.github/labels.json` are configured. Unused default categories and labels were removed. The wiki is disabled because the repository files and discussions provide the reading record.

## Maintain the configuration

1. Propose changes to the catalog, guides, and forms through pull requests.
2. Keep category slugs aligned with the filenames in `.github/DISCUSSION_TEMPLATE/`.
3. Keep hosted labels aligned with `.github/labels.json`. The file is a manifest, not an automatically applied GitHub configuration.
4. Check the rendered new-discussion form after changing its YAML template.
5. When a paper discussion is opened, copy its real URL into the catalog.
6. Create a Journal Club session only when its date and participants are known.
7. A welcome discussion may be published and pinned in Journal Club when the group is ready to introduce itself.

Repository creation, category creation, and publishing welcome or paper posts are separate hosted actions. Discussion forms become available only when the matching categories exist and the files are on the default branch.

## Discussion categories

| Name | Slug / template filename | Format | Purpose |
| --- | --- | --- | --- |
| Paper Discussions | `paper-discussions.yml` | Open-ended | One ongoing conversation per paper |
| Journal Club | `journal-club.yml` | Open-ended | Agendas, paper links, and meeting notes |
| Cross-Paper Insights | `cross-paper-insights.yml` | Open-ended | Evidence-based comparisons across papers |
| Questions & Help | `questions-help.yml` | Question and answer | Focused questions and explanations |

The live slug for **Questions & Help** is `questions-help`, matching the template filename. The four categories were verified against GitHub's repository configuration.

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

## Maintenance checks

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
