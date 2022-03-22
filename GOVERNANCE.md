# Gluecose Governance

The following document outlines Gluecose project governance.

## The Gluecose Project

The Gluecose project consists of several repositories known as sub-projects that enable community cohorts to experiment and implement solutions across the scope of the Gluecose project.

## Maintainers Structure

There are two types of maintainers in the Gluecose project organized hierarchically.
Gluecose org maintainers oversee the overall project and its health.
Sub-project maintainers focus on a single codebase or a group of related codebases.

Changes in maintainership must be announced via an [issue][issue].

### Maintainer Responsibility

Gluecose maintainers adhere to the requirements and responsibilities set forth in the respective [Gluecose Org Maintainers](#gluecose-org-maintainers) and [Sub-project Maintainers](#sub-project-maintainers).
They further pledge the following:

* To act in the best interest of the project and sub-projects at all times.
* To ensure that project and sub-project development and direction is a function of community needs.
* To never take any action while hesitant that it is the right action to take.
* To fulfill the responsibilities outlined in this document and its dependents.

### Gluecose Org Maintainers

The [Gluecose Org maintainers](./MAINTAINERS.toml) are responsible for:

* Maintaining the mission, vision, values, and scope of the project
* Refining the governance and charter as needed
* Making project level decisions
* Resolving escalated project decisions when the sub-project maintainers responsible are blocked
* Managing the Gluecose brand
* Controlling access to Gluecose assets such as source repositories, hosting, project calendars
* Deciding what sub-projects are part of the Gluecose project
* Deciding on the creation of new sub-projects
* Overseeing the resolution and disclosure of security issues
* Managing financial decisions related to the project

Changes to org maintainers use the following:

* Any sub-project maintainer is eligible for a position as an org maintainer
* No one company or organization can employ a [simple majority][simple-majority] of the org maintainers
* An org maintainer may step down by submitting an [issue][issue] stating their intent and they will be moved to emeritus.
* Org maintainers MUST remain active on the project. If they are unresponsive for > 3 months they will lose org maintainership unless a [super-majority][super-majority] of the other org maintainers agrees to extend the period to be greater than 3 months
* Any eligible person may stand as an org maintainer by opening a [PR][pr].
* When a PR is opened the project maintainers may vote
  * The voting period will be open for a minimum of three business days and will remain open until a super-majority of project maintainers has voted
  * Only current org maintainers are eligible to vote via casting a single vote each via a -1/+1 comment on the nomination issue or approving in GitHub.
  * Once a super-majority has been reached the maintainer elect must complete [onboarding](#onboarding-a-new-maintainer) prior to becoming an official Gluecose maintainer.
  * Once the maintainer onboarding has been completed a pull request is made on the repo adding the new maintainer to the [MAINTAINERS](MAINTAINERS.toml) file.
* When an org maintainer steps down, they become an emeritus maintainer

### Sub-Project Maintainers

Sub-project maintainers are responsible for activities surrounding the development and release of content (e.g., code, specifications, documentation) or the tasks needed to execute their sub-project (e.g., community management) within the designated repository, or repositories associated with the sub-project (e.g., community management).
Technical decisions for code resides with the sub-project maintainers unless there is a decision related to cross maintainer groups that cannot be resolved by those groups.
Those cases can be escalated to the org maintainers.

Sub-projects may be responsible for one or many repositories.

Sub-project maintainers do not need to be software developers.
No explicit role is placed upon them and they can be anyone appropriate for the work being produced.
For example, if a repository is for documentation it would be appropriate for maintainers to be technical writers.

Changes to maintainers use the following:

* A sub-project maintainer may step down by submitting an [issue][issue] stating their intent and they will be moved to emeritus.
* Maintainers MUST remain active. If they are unresponsive for > 6 months they will be automatically removed unless a super-majority of the other sub-project maintainers agrees to extend the period to be greater than 6 months
* Potential new maintainers should be ongoing active participants in the project
* New maintainers can be added to a sub-project by a super-majority vote of the existing sub-project maintainers
* When a sub-project has no maintainers the Gluecose org maintainers become responsible for it and may archive the sub-project or find new maintainers

## Sub-Project Release Managers

Sub-project release managers are granted a set of permissions which enable them to perform a set of release operations for the project or sub project.
The release managers MUST coordinate with the project or sub project MAINTAINERS as per the COMMUNITY and GOVERNANCE guidelines to provide a release as per the projects release criteria. Operations that the release managers are likely to perform include:

1. Publish artifacts which include binaries, libraries, containers, release notes, or other artifacts as per project requirements.
2. Configure CI/CD workflows and update repositories so as to facilitate the release of the project which ‘MAY’ produce the artifacts mentioned above.

The onboarding of a new release manager or change of an existing manager for the project SHOULD be in accordance with the governance model similar to that of an owner or a sub-project owner, depending on the scope of the release activities being performed.

### Onboarding a New Maintainer

New Gluecose maintainers participate in an onboarding period during which they fulfill all code review and issue management responsibilities that are required for their role.
The length of this onboarding period is variable, and is considered complete once both the existing maintainers and the candidate maintainer are comfortable with the candidate's competency in the responsibilities of maintainership.
This process MUST be completed prior to the candidate being named an official Gluecose maintainer.

The onboarding period is intended to ensure that the to-be-appointed maintainer is able/willing to take on the time requirements, familiar with core logic and concepts, understands the overall system architecture and interactions that comprise it, and is able to work well with both the existing maintainers and the community.

## Decision Making at the Gluecose org level

When maintainers need to make decisions there are two ways decisions are made, unless described elsewhere.

The default decision making process is [lazy-consensus][lazy-consensus].
This means that any decision is considered supported by the team making it as long as no one objects.
Silence on any consensus decision is implicit agreement and equivalent to explicit agreement.
Explicit agreement may be stated at will. In the case of security critical decisions more explicit consensus may be needed.

When a consensus cannot be found a maintainer can call for a [majority][majority] vote on a decision.

Many of the day-to-day project maintenance can be done by a lazy consensus model.
But the following items must be called to vote:

* Removing a maintainer for any reason other than inactivity (super majority)
* Changing the governance rules (this document) (super majority)
* Licensing and intellectual property changes (including new logos, wordmarks) (simple majority)
* Adding, archiving, or removing sub-projects (simple majority)
* Utilizing Gluecose/CCC money for anything CCC deems "not cheap and easy" (simple majority)

New sub-projects should be created (or added) with a well defined mission and goals, and significant changes should be voted on by both the sub-project maintainers and the org maintainers.

Other decisions may, but do not need to be, called out and put up for decision via creating an [issue][issue] at any time and by anyone.
By default, any decisions called to a vote will be for a _simple majority_ vote.

Meetings should be publicly documented ([Zulip chat][zulip-chat]), and recorded and notes kept.
Meetings should have a chair, this is a rotating role not restricted to maintainers.

## Code of Conduct

[Gluecose Contributor Covenant Code of Conduct][coc]

## Attributions

* This governance model was created using the [Veraison Project](https://github.com/veraison/community/blob/main/GOVERNANCE.md) governance documents as a template.

## DCO and Licenses

The following licenses and contributor agreements will be used for Gluecose projects:

* [Apache 2.0](https://opensource.org/licenses/Apache-2.0) for code
* [Developer Certificate of Origin](https://developercertificate.org/) for new contributions

[coc]:                ./CODE_OF_CONDUCT.md
[issue]:              https://github.com/gluecose/community/issues/new
[lazy-consensus]:     http://communitymgt.wikia.com/wiki/Lazy_consensus
[majority]:           https://en.wikipedia.org/wiki/Majority
[pr]:                 https://github.com/gluecose/community/pulls
[simple-majority]:    https://en.wikipedia.org/wiki/Simple_majority
[super-majority]:     https://en.wikipedia.org/wiki/Supermajority#Two-thirds_vote
[zulip-chat]:         https://veraison.zulipchat.com/#narrow/stream/315448-gluecose
