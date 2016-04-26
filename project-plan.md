# Project Plan

It is important that all agreements between us, the client and the coach
concerning the content, goals and methods of the project are set out in writing.
The purpose of this document therefore is to describe these items and to
formally agree upon how the project is realised. If anything changes over the
course of the project, these changes need to be documented in written form.
While an e-mail describing these changes is often sufficient, we propose that
this document is updated accordingly (perhaps simply by referring to said
emails) such that this document is the one document required to track our
progress.

# Project goal

From Spoofax's website:

> Spoofax is a platform for developing textual domain-specific languages with
> full-featured Eclipse editor plugins.

A feature that Spoofax is lacking is a Read-Eval-Print Loop (REPL) service
generator. A REPL is an interactive programming environment that takes single
expressions, evaluates them and prints the result(s). REPLs are a popular tool
for programming because they facilitate exploratory programming and debugging.
Common examples include command-line shells such as Bash and Python's REPL.

The deliverable for this project, then, is to create such a REPL generator for
the Spoofax Language Workbench.

# The final product
The final product will meet the following requirements and demands,
as specified following the MoSCoW method:

* Must-have
  * Interactive REPL
    * Generated from language definition
    * Should be language definition agnostic
    * Syntax checked expressions
  * Indication of errors
  * Integration with Eclipse
  * Syntax highlighting
* Should-have
  * Save and load shell state
* Could-have
  * Integration with other IDE's (IntelliJ)
  * Hover over variables to see value, type and others
  * GDB style interaction with context / environment
    * Ability to partially change or update environment
  * Literate programming
* Won't-have

If the above turns out to be (too) easy, the REPL can be extended into a
language playground such as the one offered by the Swift programming language.
If we decide to extend the project, new agreements will be made between us and
the client.

# Methodologies and tooling

During this project we will work using the SCRUM methodology with weekly
sprints. Our backlog, current and completed sprints will be managed using
[Trello](https://trello.com/b/u2aKQ12y/bachelor-project-spoofax-repl).
Trello will also be used to communicate documents to the client and the TU coach.
Sprints will end on friday, coinciding with most deadlines according to the
planning for this project as mandated by TU Delft.

Each sprint will start with a "sprint planning event", in which user stories
from the backlog will be assigned to project members, based on their
prioritization and their feasibility for this sprint.
Each sprint will end with a meeting in which we discuss to what degree
we have achieved our sprint planning and how we can improve on that.
A working demo should always be available at the time of the "sprint review".
During sprints, the team will hold a daily scrum every day, where
they will discuss their progress of the previous day and their planning for
today, as well as any issues that could be detrimental to the weekly sprint goal.

We will use a pull-based development model using GitHub in conjunction with
the SCRUM methodology. GitHub Issues will be used to
track issues (all of this will be linked to Trello in one way or another).
To facilitate this, we will use repositories from our GitHub organization
[spoofax-shell](https://github.com/spoofax-shell).
Each of us will then fork these repositories to our private GitHub
accounts. We will also use one repository to hold all the documents
(e.g. this document, the research project, et cetera) supporting our project.

A pull request will be designated a status tag WIP, RFC or RDY:

* WIP: Work in progress
* RFC: Request for comments
* RDY: Ready

A pull request can be changed from WIP to RFC as soon as it is "done",
which means it contains sufficient documentation and test coverage,
and that the pull request passes continuous integration testing.
Pull requests with status RFC should be reviewed by at least one other member
of the development team. Once reviewed, the pull request can be changed
to RDY, after which it can be merged.
This process ensures that all code has been reviewed and tested before
being merged into the final product, thereby always ensuring a working product.

Since Spoofax is an already existing project, we will reuse most tooling that is
already being used. This means that we will use:

* the Java programming language;
* Maven for the build environment;
* JUnit for unit tests;
* TravisCI for continous integration

# What TU Delft expects from us

This section's purpose is to document additional agreements between the TU coach
and us. For the regular project deadlines, please see the end of this section.

Weekly meetings with the TU coach will be held on mondays at 11.00 to discuss
the past and next week, and the overall progress of the project.
Documents (such as the meeting topics) that will be discussed will be emailed
to the TU coach at its latest the evening before the day of the meeting.

Minutes will be made of every meeting, whether with the client, the TU coach or both.
These minutes shall be sent to the TU coach as well.

Regular project deadlines:

* 19-04-2016: Project Plan
* 29-04-2016: Research Report
* 20-05-2016 - 27-05-2016: mid-project meeting (coordinator + team + client)
* 27-05-2016: SIG 1st submission
* 17-06-2016: Final Report
* 17-06-2016: BEP infosheet
* 17-06-2016: SIG 2nd submission
* 24-06-2016: Final presentation

# Quality assurance
