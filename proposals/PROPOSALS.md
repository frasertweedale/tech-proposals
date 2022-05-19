An HFTP (*Haskell Foundation Technical Proposal*) is a proposal for a technical initiative that will be executed under the guidance of the Haskell Foundation (HF). Each HFTP goes through an iterative process in which it is discussed by the HF Technical Working Group (TWG), the broader community, and any and all interested stakeholders. As part of this process, resources are identified that could ease or make possible the implementation of the proposal.

The aim of the HFTP process is to apply the openness and collaboration that have shaped Haskell's documentation and implementation to a process of evolving the HF and the broader Haskell ecosystem. This document captures our guidelines, commitments and expectations regarding this process.

## Acceptance

Upon acceptance, an HFTP and its associated discussion are merged into this repository, and both serve as a historical document that details a specification and rationale for work detailed within the process. Acceptance of a proposal does not constitute a firm commitment by the Haskell Foundation to execute on the proposal, or to provide the necessary or helpful resources that were identified in the proposal. Fundamentally, acceptance indicates that the TWG believes that the Haskell ecosystem would be better off if the proposal were implemented, and that it is sufficiently well-considered.

That said, the Haskell Foundation is keenly interested in making the Haskell ecosystem better off. Within the constraints of the Foundation's resources and strategic plans, accepted proposals will be considered as good candidates for tasks to be executed on.


## Submission process summary

1. Submit a Pre-HFTP topic to [Discourse](https://discourse.haskell.org), soliciting informal feedback.
2. If the feedback is favorable, fork the Haskell Foundation tech-proposals repository, [https://github.com/haskellfoundation/tech-proposals](https://github.com/haskellfoundation/tech-proposals).
3. Create a new HFTP file in the `proposals/` directory. Use the [HFTP template](https://github.com/haskellfoundation/tech-proposals/blob/main/proposals/TEMPLATE.md)
 * Make sure the new file's name follows the format: `YYYY-MM-dd-{title}.md`. Use the current date for `YYYY-MM-dd`.
 * Use [Markdown Syntax](http://daringfireball.net/projects/markdown/syntax) to write your HFTP.
4. Commit your changes to your forked repository
5. Create a new [pull request](https://github.com/haskellfoundation/tech-proposals/pull/new).
6. Notify the TWG on Github using the team label `@haskellfoundation/tech-proposals`. Optionally, the address the `#tech-track` channel on the HF Slack instance or on Discourse (or both!).


## Why Write a Proposal?

HFTPs are key to making the HF and its initiatives better for the good of everyone. If you decide to invest the time and effort of putting a proposal forward and see it through, your time and efforts will shape and improve the Haskell ecosystem, which means that your proposal may impact the life of myriad developers all over the world, including those on your own team. For many, this aspect alone can be quite worthwhile; however, the proposal process itself offers several key benefits to the broader community:

1. **Concretizing ideas:** as ideas for proposals are fleshed out, so too are the resource requirements, timelines, stakeholders, and available approaches. In this sense, a proposal allows us to fully concretize a proposal idea in terms of the work needed to complete the task.
2. **Implementation guidance:**  the myriad of subject matter experts and stakeholders affected by a proposal can comment in a centralized place to form a consensus and guide the implementation strategy for a particular task.
3. **Resource requirements:** ideas are often discussed in the abstract, without the consideration for the cost of work required for their implementation. This process allows for discussion that reifies the resource requirements for proposals, and allows the community to more accurately weigh the cost and benefits of an implementation.

It's important to note that seeing a proposal through to its conclusion is an involved task. On the one hand, it takes time to convince people that your suggestions are a worthwhile change for hundreds of thousands of developers to accept. Particularly given the sheer volume of developers that could be affected by a proposal, its acceptance is conservative and carefully thought through. Typically, this includes many rounds of discussion with HF leaders, Haskell library maintainers, and the broader community, several iterations on the design of the proposal, and some effort at prototyping the proposed change. Often, it takes weeks to months of discussion, re-design, and prototyping for a proposal to be accepted. It is therefore important to note that seeing a proposal through to its conclusion can be time-consuming and not all proposals may end up accepted, although they may teach us all something!

If you’re motivated enough to go through this involved but rewarding process, go on with writing and keep on reading.

## What kind of proposals are appropriate for an HFTP?

Many people in Haskell donate a considerable amount of their time to improving Haskell and its ecosystem for free. However, sometimes the financial or human cost of a project is too great for the individual, or creates an undue out-of-pocket expense in order to support those contributions. This is where the HFTP process comes in, and what separates this process from the core libraries process, or a GHC proposal: the HF is capable of contributing time, money, and resources to make a proposal happen.

### Resourcing

Consider the following examples:

- A contributor needs computational resources for CI, or to produce stable Hackage subsets
- A contributor wants to write educational materials covering a yet-unwritten-about portion of Haskell, but requires an editor
- An open source project requires funding for volunteers engaged in Summer of Code-type work on core tooling for Haskell

In each of these cases, the author of the associated HFTP should detail the resource request for machines, an editor, or in terms of volunteer funding needed to meet their delivery goals. Throughout the HFTP process, these resource requests will be considered and weighed against the existing demand for HF resources. If accepted, these resource requests be honored by the HF to the extent possible.

### Proposal Size

There is no size floor or ceiling for project submissions. In particular, small quality of life proposals are as welcome as epic community-shifting proposals - we do not judge. However, this is why step 1 (informal discussion) is so important: often, it may be faster and easier to just make that Pull Request and find people who are free to do it with you! If, for some reason, the discovery and discussion phase does not catch these issues, it will be raised by TWG members when appropriate. When a proposal, big or small, is inappropriate for the venue, we will be sure to make it known.

## What's the process for submitting a HFTP?

There are four major steps in the HFTP process:

1. Initial informal discussion
2. Submission
3. Formal Review
4. Acceptance

### Initial Discussion

Before submitting a HFTP, please write about your idea on the [Haskell.org Discourse](https://discourse.haskell.org/) and publicize the post in relevant venues. Create a Discourse topic under the category "Haskell Foundation", that starts with "Pre-HFTP” and briefly describe what you would like to change and why you think it’s a good idea. This helps discover prior art and related projects that are already underway. In some exceptional cases where prior art and existing projects are extremely unlikely, this requirement may be waived - please check in with the TWG if this is the case.


### Submission

A HFTP is a Markdown document written in conformance with the [process template](https://github.com/haskellfoundation/tech-proposals/blob/main/proposals/TEMPLATE.md). When such changes significantly alter an existing library or tool, the author is invited to provide a proof of concept. Delivering a basic implementation can speed up the process dramatically. If your changes are big or somewhat controversial, don’t let people hypothesize about them and show results upfront. Additionally, the author of the proposal should reach out to any stakeholders (e.g. library authors, maintainers) affected by the proposal and bring them into the formal discussion at this point.

A HFTP is submitted as a pull request against [the official Haskell tech proposal repository](https://github.com/haskellfoundation/tech-proposals). Within a week of receiving the pull request, members of the TWG will acknowledge your submission, validate that it conforms to the proposal template guidelines (see: [TEMPLATE.md](TEMPLATE.md)) and provide feedback to improve the overall quality of the document (if necessary). When the document conforms to the template guidelines, it is ready for formal evaluation by the TWG members, as well as the broader community.

### Formal Review

While the majority of general technical commentary and feedback will occur on the proposal pull request and its associated issue, it's hard to tell when a particular proposal is finalized. This what we call "Formal Review".  The entire community is strongly encouraged to comment on, and help improve, a proposal. Ultimately, however, the Foundation needs a mechanism to make a decision, to accept, reject, or push back a proposal. This process is called "Formal Review", and is carried out by the TWG working group.

#### Formal Review

Formal Review of a proposal is done in iterations. These iterations take place in the TWG meetings and are usually monthly. However, they can last longer, in which case the author has more time to implement all the required changes.

The maximum number of iterations is five. At the fifth iteration, the TWG can only vote to Accept, Postpone, or Reject.

The TWG decides the duration of the next iteration depending upon the feedback and complexity of the HFTP. Consequently, authors have more time to prepare all the changes. If they finish their revision before the scheduled iteration, an TWG member will reschedule it for the next available meeting.

During every iteration, the TWG reviews the changes (updated design document, progress with the implementation, etc) to the proposal. Based on the feedback, the HFTP is either:

1. **Accepted**, in which case the TWG has accepted the proposal, and it will be merged by the TWG members.
2. **Rejected**, in which case the HFTP is closed and no longer evaluated in the future.
3. **Postponed**, in which case the TWG sets aside the HFTP under some conditions. When those conditions are met, the HFTP can be resubmitted.
4. **Under revision**, in which case the author needs to continue the formal evaluation and address all the TWG feedback. Thus, the follow-up discussion is scheduled for the next iteration.
5. **Dormant**,  in which case no changes have been made to a HFTP in two iterations, it’s marked as dormant and both the PR and issue are closed. Dormant HFTPs can be reopened by any person, be it the same or different authors, at which point it will start from the formal evaluation phase.

#### Involving Stakeholders

At this point where a proposal is being reviewed, if there are relevant stakeholders from industry or in the community (e.g. library authors and maintainers who are affected), they should be solicited by the proposal author for comment and brought into the discussion. Remember, proposals may sound good, but it's best to iron out as many details as possible prior to their acceptance. This means that any hesitations stakeholders have with the project should be factored into the proposal's details.

#### Updating Proposal Statuses

If the author of a particular proposal wants to update the status of their proposal, they should comment on the issue and alert the TWG using the GitHub team tag `@haskellfoundation/tech-proposals` with a note regarding what status they would like to update the proposal to. It is good to be redundant and raise the question in our other fora as well: Slack and Discourse. However, Github is required.

### Acceptance

Upon acceptance, an HFTP is merged into the repository by an TWG member, and the HFTP is assigned a shepherd from the TWG who will serve as a liason for the project, guiding its progress. Shepherds are required to report dutifully and accurately on the progress to the TWG. Project leaders are welcome to arrange alternative reporting schema (e.g. as their schedules allow, or if time off is required) upon request, as long as reports are given on a consistent basis.

## The Role of the TWG

Authors are responsible for building consensus within the community and documenting dissenting opinions before the HFTP is officially discussed by the TWG. Their goal is to convince the TWG that their proposal is useful and addresses pertinent problems in the Haskell ecosystem as well as interactions with already existing features. Authors can change over the life-cycle of the HFTP. For a formal charter, as well as a list of current TWG members, please see [CHARTER.md](CHARTER.md).

### Voting

When a HFTP is scheduled at an TWG meeting (i.e. it is in 'Under Review'), it can be held to a vote for one of the following outcomes (in case it makes a difference: the HFTP will be marked according to the first on this list to have a majority) using a ranked voting method described in [CHARTER.md](CHARTER.md).

- Accepted (needs 66% of the TWG to vote in favor, and the HFTP must specify a proposal lead, e.g. an implementor or project director, from the TWG who will represent the work done on the project.)
- Dormant (needs a simple majority, an TWG member that voted in favor will close the issue and PR and mark it as Dormant)
- Postponed (needs a simple majority, an TWG member that voted to postpone will close the issue and PR, and write clear conditions for reopening)
- Revision needed (needs a simple majority. This can only be the outcome of the vote four times, for a total of five rounds. An TWG member will write up what revisions are needed.)
- Rejected (needs 66% of the TWG to vote in favor)

### Guests

Experts in some fields may be invited to specific meetings as guests when discussing related HFTPs. Their input would be important to discuss the current state of the proposal, both its design and implementation.

### Joining the TWG

If you would like to join the TWG or would like to know how members are elected, please refer to [CHARTER.md](CHARTER.md).


