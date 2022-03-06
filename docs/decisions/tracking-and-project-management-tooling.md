# Tracking and project management tooling (#79)

## Who?

The task was delegated to:

- Michael @Gapodo
- Anja @CraazyTRex007

## Contenders

- [Jira Software](https://www.atlassian.com/software/jira)
- [Github Projects (beta)](https://docs.github.com/en/issues/trying-out-the-new-projects-experience/about-projects)
- [openProject](https://www.openproject.org/)
- [Trello](https://trello.com/)
- [WeKan](https://wekan.github.io/)
- [ClickUp](https://clickup.com/)

## Criteria

- pricing / limitations in free editions
- availability
- ease of use
- linking to the SCM (GitHub)
- setup effort

## Preferences

- already in use by a team member
- keeping tool count low
- while self hosting is no problem, using provided tooling is usually quicker

## Rating

### Jira Software

_Jira Software_ is available as a free edition up to _10 people_, the limitations imposed on free tier users are mostly non-intrusive to our project, but degrade the experience towards the functional level of _GitHub Projects_.

_Jira Software_ allows for blocking issues, multiple assigned persons and reviewers is possible using workarounds.

Integration with the _SCM_ ist possible, but requires addons.

Proper setup is relatively complex, but has been done before by Michael @Gapodo, Anja @CraazyTRex007 has some experience as a user.

### GitHub Projects (beta)

While the _GitHub Projects_ views are still in a beta phase, the _GitHub Projects_ boards are available as fallback, also all items on the project boards and lists are simple issues in the repos issue tracker.

Linking in between issues is possible, defining blockers, which actively block other issues is not possible.

Licensing wise, using _GitHub Projects_ is free within the general limitations of free _GitHub_ the limitations are:

- no multi assignment
- no multi reviewing

Huge plus would be complete integration with the _SCM_ as it's just a view on the repos issues (but could aggregate across repos).

### openProject

_openProject_ is available for free as a _self hosted_ community edition.

The amount of work needed to start initial work is substantial and integration with _SCMs_ tedious (feedback by work colleague of Michael @Gapodo).

### Trello

_Trello_ is a _commercial_ Kanban board, the product has been acquired by _Atlassian_ (mfg. of _Jira Software_).

_SCM_ Linking would be possible via manually entered links (no proper integration), the feature set does not surpass _Jira Software_ or _GitHub Projects_.

Issue blocking, multi assignment or reviews are not possible within _Trello_.

### WeKan

_WeKan_ is a open source, _self hosted_ Kanban board and a direct alternative to _Trello_ (with a migration tool from _Trello_ to _WeKan_). The feature set is OK, there are no limits on user count or similar.

### ClickUp

_ClickUp_ is a _commercial_ project management tool seemingly optimized for software development, the free edition has an extremely low storage allowance (200MB), when adding images to stories, this is most likely quickly surpassed.

## Decision

Ordering:

1. GitHub Projects
2. Jira Software
3. openProject
4. WeKan
5. ClickUp
6. Trello

- The _self hosted_ solutions are far down the list due to the setup times needed.
- _Trello_ lost out, since it provides the fewest features and has an open source alternative.
- _ClickUp_ has way to low of a size limit.
- The warning about the needed effort for setup and base config for _openProject_ disqualified it as a solution for this project.
- While _Jira Software_ provides many features the _SCM_ linking is only OK, proper setup is quite intricate and the licensing puts it only a bit above _GitHub Projects_.
- Since _GitHub_ will be the _SCM_ used for the project, integration with _GitHub Projects_ is good, there is no tool-switching, the missing features are not severe enough to warrant the effort associated with the usage of multiple software pieces.

According to the points mentioned above, **GitHub Projects** was chosen as the project management and issue tracking tool.
