# Project 2: Game Development and Evaluation
**Participants:** This project is to be completed in groups of 3-4 people.

**Marks:** This project counts towards 60% of your marks for this subject.

**Due date:** Multiple submissions required; see the [schedule](#schedule) below.

## Schedule

This project is split into a number of milestones, each with its own deadline.
The milestones are split into two categories: team and individual. Team
milestones are submitted by the team leader on behalf of the team, while
individual milestones are submitted by each team member individually.

#### Team submissions

- [Milestone 1 | Evaluation Demo](#milestone-1-evaluation-demo) ... due **Sunday 8 October, 11.59pm AEST**
- [Milestone 2 | Gameplay Video](#milestone-2-gameplay-video) ... due **Sunday 15 October, 11.59pm AEST**
- [Milestone 3 | Final Submission](#milestone-3-final-submission) ... due **Tuesday 31 October, 11.59pm AEST**

#### Individual submissions

- [Milestone 4 | Team Member Evaluation](#milestone-4-team-member-evaluation) ... due **Thursday 2 November, 11.59pm AEST**
- [Milestone 5 | Team Feedback Reflection](#milestone-5-team-feedback-reflection) ... due **Sunday 5 November, 11.59pm AEST**

## Table of Contents
- [Assignment Brief](#assignment-brief)
  - [Overview](#overview)
  - [Requirements](#requirements)
  - [Development Tools](#development-tools)
  - [Accepting the Assignment](#accepting-the-assignment)
- [Milestone 1: Evaluation Demo](#milestone-1-evaluation-demo)
- [Milestone 2: Gameplay Video](#milestone-2-gameplay-video)
- [Milestone 3: Final Submission](#milestone-3-final-submission)
- [Milestone 4: Team Member Evaluation](#milestone-4-team-member-evaluation)
- [Milestone 5: Team Feedback Reflection](#milestone-5-team-feedback-reflection)
- [Assessment](#assessment)
- [Report](#report)
  - [Evaluation plan](#evaluation-plan)
  - [Evaluation report](#evaluation-report)
  - [Shaders and Special Effects](#shaders-and-special-effects)
  - [Summary of Contributions](#summary-of-contributions)
  - [References and External Resources](#references-and-external-resources)
  - [Other Details](#other-details)
- [WebGL Builds](#webgl-builds)
- [Gradescope Submissions](#gradescope-submissions)
- [Late Submission Policy](#late-submission-policy)
    - [Team submissions](#team-submissions-1)
    - [Individual submissions](#individual-submissions-1)
- [Academic Honesty](#academic-honesty)
  - [Use of AI Tools (e.g., ChatGPT)](#use-of-ai-tools-eg-chatgpt)
  - [Unity Asset Store](#unity-asset-store)
  - [Credit where credit is due ...](#credit-where-credit-is-due-)
- [Resources and Help](#resources-and-help)


## Assignment Brief

### Overview

In this project you will enter the full development phase of the game you
designed and prototyped in Project 1. You will be required to develop the game
in its entirety, evaluate it with end users, and improve it based on their
feedback. There will also be a focus on low-level graphics techniques, and you
will be required to implement a number of shader effects in your game to help
bring it to life.

### Requirements

Here's a high level overview of the requirements for this project:

- The game must be a continuation of the game you designed in Project 1,
  following the same GDD and "time survival" mechanic (all design requirements
  from Project 1 still apply unless otherwise stated). 
- The game must be playable in a computer web browser (as a WebGL build),
  including a full-screen mode.
- The game must be developed using [Unity 2022
  LTS](https://unity.com/releases/lts) and tracked on GitHub (see [Development
  Tools](#development-tools) below).

You will be working in the same team of people as you did in Project 1, and
will again be required to submit a number of milestones. The first three
milestones are team-based, and will be submitted by the team leader on behalf
of the team. The final two milestones are individual, and will be submitted by
each team member individually. Be sure to read the [Assessment](#assessment)
section below carefully, as it provides details on our full set of expectations
for this project. 

> **Note**<br>
> You'll again be asked to evaluate your team members at the end of both
> projects in this subject. See the [Team Member
> Evaluation](#milestone-4-team-member-evaluation) milestone for more details.
> We expect that any issues raised in the Project 1 evaluation will be
> addressed in this project, so every member of the team should take the time
> to read their feedback and reflect on it.

### Development Tools

You'll again be collaborating with your team via GitHub Classroom. We will
provide you with a **new** private repository for this project, which will be
pre-populated with a Unity project template. See the [Accepting the
Assignment](#accepting-the-assignment) section below for more details.

Your game must be developed using [Unity 2022
LTS](https://unity.com/releases/lts). All team members are expected to
regularly commit and push their changes to GitHub. Based on experiences and
feedback for Project 1, you should continue refining strategies as a team for
avoiding and resolving merge conflicts, as these can be a major source of
frustration and wasted time. This will be increasingly important as the project
progresses, and changes become more complex.

### Accepting the Assignment

A **new** private template repository will be created for your team via GitHub
Classroom. You should not be updating the Project 1 repository going forwards.

> **Warning**<br>
> Follow _all_ of the instructions below very carefully! Do not blindly
> overwrite the new template with your entire repository from Project 1. If you
> change critical files in the new template, it is probable that online WebGL
> builds will fail in some way. We will be less lenient in this project than we
> were in Project 1 regarding last-minute failed builds, especially if it is
> due to careless overwriting of template configuration files.

Together as a team, accept the assignment by following these steps:

1. The **team leader** should create the new repository by accepting the
   assignment on the [LMS assignment
   page](https://canvas.lms.unimelb.edu.au/courses/154322/assignments/420267?module_item_id=5127103).
   (Teams previously created will be preserved, so you should be able to accept the
   assignment and create the repository without any issues.)
2. **All other team members** should then join the repository via the same link. 
3. **Everybody** should clone the new repository to their local machine and open
   the template project in Unity. It might be necessary to download the latest
   LTS version of Unity first, if you don't already have it installed.
4. The **team leader** should open and update (not overwrite) the template
  `metadata.yml` file in the root of the repository. Follow the instructions
   within the comments carefully.
5. The **team leader** should copy content from the Project 1 GDD into the
   `GDD.md` file in new the template repository, along with any needed
   attachments. Your team is expected to update the GDD here to reflect any
   refinements to the game going forwards. Notice that there is a _separate_
   `README.md` that will house the [report](#report) for this project. Keep the
   template for this file **as-is** for now.
6. The **team leader** should commit and push all of the above changes to the
   `main` branch.
7. **All other team members** should then pull these changes to their local
   repository and verify that they can see the updated `metadata.yml` and
   `GDD.md` files.

**Finally, after once again heeding the above warning**, you may systematically
copy over files in the `Assets` folder from Project 1 as needed. Your team
is strongly encouraged to be selective and incremental (with regular testing)
when doing so. Take lessons from Project 1 on board as you do, and
ensure that your team is working in a way that minimises the risk of merge
conflicts. The same 250MB limit applies to the `Assets` folder, so be mindful
of this as you copy over files.


## Milestone 1: Evaluation Demo
**Due: Sunday 8 October, 11.59pm AEST (team submission)**

By this milestone deadline your game should be developed to a point where your
team can begin evaluating it with end users. This means that the core gameplay
should be implemented, and the game should be playable in a web browser (as a
WebGL build). The game does not need to be polished at this stage, but it
should be playable from start to finish. In the `README.md` template there is a
section titled **Evaluation Plan** that should be filled out by your team by
this milestone deadline. See the [Evaluation](#evaluation) section below for
more details.

After this point, design changes should primarily be based on feedback from end
users in your evaluation, and your team should be focusing on improving the
game's polish and overall quality. Major changes should only be made if the
evaluation reveals a significant issue with the game's design.

> **Note**<br>
> Your team should also be actively maintaining the same GDD from Project 1 in
> your repository. It should have the name `GDD.md`, and be situated in the top
> level directory of the repository alongside the new `README.md`. Ensure that
> it reflects the current state of the game at each milestone deadline,
> including this one.

### Submission

Update the repository `metadata.yml` by filling in the following entries:

```yaml
GameTitle: <your game title>
GameBlurb: <a short description of your game (max 200 words)>
```

Then, make sure the latest changes to your project are in the `main` branch, and submit the project repository on Gradescope as per the instructions under the
[Gradescope Submissions](#gradescope-submissions) section below. **Every member
of the team must verify that:**

- The submission on Gradescope is visible to them and that all validation tests
  are passing.
- The evaluation demo can be played in a (modern) web browser via the link on
  Gradescope, including full-screen mode.

## Milestone 2: Gameplay Video
**Due: Sunday 15 October, 11.59pm AEST (team submission)**

The final two lectures will be dedicated to showing everyone's games in action!
In order to do so, your team will upload a short gameplay video to YouTube
demonstrating the key features of your game (1 to 2 minutes long), by the
deadline above. You may make the video unlisted if you wish to prevent it from
being viewed publicly, but please ensure that we can access it from the
provided link without requiring any special permissions. Your video should be of a high quality, and don't forget to make it stand out from the crowd with some creative flair!


### Submission

Update the repository `metadata.yml` by filling in the following entry:

```yaml
GameplayVideo: <a link to your YouTube video>
```

Then, make sure the latest changes to your project are in the `main` branch, and once again submit the project repository on Gradescope as per the
instructions under the [Gradescope Submissions](#gradescope-submissions)
section below. The validation tests will now also check that the new
`metadata.yml` entry points to a real video. Every member of the team is again
responsible for verifying that the submission on Gradescope is visible to them,
all test cases pass, and that the video can be viewed via the link.

## Milestone 3: Final Submission
**Due: Tuesday 31 October, 11.59pm AEST (team submission)**

By this milestone deadline your game should be fully completed. You should have
completed your evaluation, summarised it in a final report (`README.md`) and
made changes to the game based on the feedback you received. The game should be
polished to the extent that it would be ready to be played by your target
audience as a published game.


> **Warning**<br>
> The `Assets` folder should be kept organised, and **must not exceed 250MB**.
> The game should run at a reasonable framerate (30fps or higher) on a typical
> laptop/desktop computer web browser. Remember to regularly build and test
> your Unity project as outlined in the [WebGL Builds](#webgl-builds) section
> below. 

As already discussed, your team’s final submission must open and run in Unity
2022 LTS without modification. The entry point should be
`Assets/StartScene.unity` (the marker will open this scene and play it from here
if they open the project in Unity). 


### Submission

This final team submission is the most important one to get right. It is
strongly recommended that you submit (and check the online WebGL build) at
least a couple of times _comfortably before_ this deadline, as it is the
version of the game that will be marked. Unlike in Project 1, we won't be as
lenient regarding last-minute issues with the submission, especially if they
could have been avoided by submitting and verifying earlier.

> **Note**<br>
> Double (and triple!) check that the latest changes to your project are in the `main` branch, and make sure this branch is being submitted on Gradescope. We will not be looking at other branches when marking.

Once again, follow the instructions under the [Gradescope
Submissions](#gradescope-submissions) section below in order to submit your
final work. Remember that the submission on Gradescope is what will be marked,
so ensure that you submit early and often to avoid any nasty surprises right
before the deadline. 

Every member of your team is expected to verify that the submission on
Gradescope is visible to them, that all validation test cases pass, and that
the **final version** of the game (i.e. the one you want marked) can be played
in a browser via the link in the submission confirmation page. 

## Milestone 4: Team Member Evaluation
**Due: Thursday 2 November, 11.59pm AEST (individual submission)**

Teamwork is an essential part of the project, and it is possible for individual
group members to receive a different mark to that of the group. Most
importantly, **each person is expected to contribute to the project equally.**
We also expect that there is effort to include all group members in the project
discussions and decision-making process. Therefore, we will be asking you to
evaluate your team members' contributions to the project, as well as provide a
self-evaluation of your own contributions.

After your team submits your final work, you are individually required to
submit a group member evaluation form for each of your team members. This is
conducted via a tool called FeedbackFruits, which you can access [via the
LMS](https://canvas.lms.unimelb.edu.au/courses/154322/assignments/420272).

> **Warning**<br>
> The group member evaluation is compulsory, and must be submitted by the
> deadline. Failing to do so will be taken to be an indication that you have
> not contributed to the project, resulting in you receiving an individual mark
> of zero.

The evaluation form will ask you to rate each team member on a rubric (scale of
1 to 5) using the following criteria:

- **Communication:** Refers to the quality of the group member's input in
  project discussions and their ability to facilitate effective communication.
  A good communicator provides meaningful input and contributes constructively
  to project discussions, be that in person or online.
- **Collaboration:** Refers to a group member's ability to work with others,
  respect their ideas, and promote balanced participation in discussions. This
  does not mean that all team members must agree on everything, but there
  should be a willingness to compromise and work together to achieve a strong
  outcome.
- **Contribution:** All team members are expected to contribute equally and
  pull their weight. A good contributor completes assigned tasks on time, and
  shows overall commitment to the project.

Please take the time to provide thoughtful and constructive feedback for each
of your team members. In many cases all team members will receive the same
mark, but in some cases we may adjust individual marks based on the group
member evaluation.

## Milestone 5: Team Feedback Reflection

**Due: Sunday 5 November, 11.59pm AEST (individual submission)**

After you have completed the group member evaluation, you will be able to see
the feedback that your team members have provided for you. You are also given
the opportunity to reflect on this feedback. This task is technically optional,
but we nonetheless encourage you to take the time to write something, even if
brief.

If deemed necessary, we may look at individual reflections as part of our
decision-making process for adjusting marks. Importantly, if you feel that you
have been unfairly evaluated, you can provide a response here (if this is about
unequal contributions, please provide repository URLs to commits where you have
contributed to the project). In any case, please be respectful and constructive
in your responses.

## Assessment

This assignment is worth 60% of your final mark. It will be assessed based on the following criteria:

**Gameplay (16 marks):**
- Instructions should be well specified within the game and controls should
  respond as expected. The chosen control scheme should be intuitive and easy
  to use. The objective of the game should be clear, with the player being able to
  progress towards and achieve that objective as intended.
- The design requirements from Project 1 should continue to be met. The survival
  mechanic should be clear and well-integrated into the game.
- The game should be bug-free and operate at a reasonable frame rate on a
  modern laptop/desktop computer web browser as a WebGL deployment.
- The game should be polished to the level of being "release ready", and there
  should be no obvious "rough edges" (e.g., objects clipping through each
  other, poor collision detection, etc). 
- Audio should be used to enhance the gameplay experience, as appropriate for
  the game's genre and style.
- The gameplay video must effectively and creatively capture all of the key
  gameplay elements. It should be polished and of a high quality, including
  clear audio and visuals.

**Graphics and Interfaces (10 marks):**
- Objects and entities should be clearly visible, and clearly distinguishable.
- Objects, entities, textures, lighting and user interfaces should suit the
style of the game, and consistent aesthetics should be employed across the
game.
- Camera orientation, positioning and motion should be comfortable and
well-polished.
- The overall visual style should capture the original vision in the GDD, with
various graphical techniques being fine-tuned to enhance the game's visuals
accordingly.

**Shaders and Special Effects (16 marks):**
- Two non-trivial Cg/HLSL `.shader` programs should be custom-written to
appropriately enhance the game’s visuals and (potentially) reduce burden on the
CPU. Each should be involved in producing a **distinct** effect.
- Clear, concise descriptions and rationales for the shaders must be detailed
in the report, along with exact paths to the respective shader asset files
(these should be links in the `README.md` to files in the repository). If your
team writes more than two shaders, choose two that your team would like to be
marked and ensure that you make this clear in the report.
- At least one particle system should be custom-created to create or enhance a
special effect within your game. Clearly specify in your report which particle
system should be marked, and how to locate it in your Unity project. Detail the
particle system attributes that were varied, how randomness was utilised, and
provide rationales for such choices.

**Evaluation and Report (12 marks):**
- You should use at least one querying technique to evaluate and then improve
your game. You should recruit a minimum of 5 participants for this technique.
- You should use at least one observational method to evaluate and then improve
your game. You should recruit a minimum of 5 (different) participants for this
technique.
- The overall quality of the delivered report matters, and writing should be
clear and concise (see below for details). The report should be in the
`README.md`.

**Project Organisation (6 marks):**
- The project should be well-organised and easy to navigate, with
  `Assets/StartScene.unity` being the entry point. 
- The assets folder must not exceed 250MB in size.
- All autograder "validation" tests should pass by the deadline for each
  milestone. Workflow files provided in the template repository must not be
  modified (everything under `.github/workflows`).
- All team members must be committing to the GitHub classroom repository, and a
  workflow for avoiding/resolving merge conflicts should be in place.
- All milestone deadlines must be met, and the project must show evidence of
  iterative development (i.e., not just a few of commits at the end). The
  latest version of the project must be on the `main` branch by each milestone
  deadline.
- The GDD from Project 1 should be kept up to date in the **new** team
  repository, and must reflect the current state of the game at each milestone
  deadline. It should be named
  `GDD.md` and be located in the top level directory of the repository
  alongside the `README.md`.
- All guidelines in this specification must be followed with care, including
  those regarding the [submission process](#gradescope-submissions) and [late
  submissions](#late-submission-policy).

## Report

Your final `README.md` should include a report with the below subheadings. Like
the GDD, the report should be written in "GitHub Flavoured" markdown, and it
should be clear and concise. Make use of headings, lists, images, and other
formatting features to make it easy to read and navigate. The `README.md` file
should be located in the top-level directory of the repository alongside the
GDD, which should be maintained another file named `GDD.md`. This structure is
already in place in the template repository.

### Evaluation plan

An important part of this project is evaluating your game with end users. This
will help you to identify any issues with your game's design, and provide you
with an opportunity to make changes before the final submission. Don't
underestimate the value of this process! It is very difficult to design a game
that is fun and engaging without testing it with real people.

> **Note**<br>
> We expect that your team utilises at least one **querying** and one
> **observational** evaluation technique, as discussed in the lectures. At
> least 5 participants are required for each technique (i.e., a minimum of 10
> participants in total). 

By the [Milestone 1](#milestone-1-evaluation-demo) deadline, your team should
have a plan in place for how you will evaluate your game. Here's some important
questions to consider:

- **Evaluation techniques:** Which evaluation techniques will you use and why?
  What tasks will you ask participants to perform?
- **Participants:** How will you recruit participants? What qualifying criteria
  will you use to ensure that they are representative of your target audience?
- **Data collection:** What sort of data is being collected? How will you
  collect the data? What tools will you use?
- **Data analysis:** How will you analyse the data? What metrics will you use
  to evaluate your game, and provide a basis for making changes?
- **Timeline:** What is your timeline for completing the evaluation? When will
  you make changes to the game?
- **Responsibilities:** Who is responsible for each task? How will you ensure
  that everyone contributes equally?

These are just some of the questions that your team should be considering, and
it is important that you have some goals in mind for what you want to achieve
with your evaluation, and design it around these goals accordingly. Your team
should outline your evaluation plan in the `README.md` template under the
**Evaluation Plan** section.

### Evaluation report

By the [Milestone 3](#milestone-3-final-submission) deadline, your team should
have completed your evaluation and made changes to the game based on the
feedback received. You should then update the report to summarise your
evaluation, including the changes you made to the game as a result. This should
be outlined in the `README.md` template under the **Evaluation Report**
section. If you wish, you may merge the **Evaluation Plan** into this section
and reword it to make this a full (retrospective) report. In any case, make
sure participant demographics and the exact methodology you followed is clear
in the final report.

### Shaders and Special Effects

As per the [assessment criteria](#assessment), there should be discussion
around the two custom Cg/HLSL shaders you were required to write, as well as
the particle system that your team wishes to be marked. Be sure to include
direct links to two `.shader` files in the repository, in order to make it
clear what should be marked. Also include images/gifs that clearly demonstrate
the shaders (and particle system) in action.

We expect that you provide context showing how the shader effects fit into the
rendering pipeline/Unity engine, taking into account theory as discussed in the
workshops and lectures. For example, if shaders take uniform parameters that
must be set from a C# script, make sure you explain this and provide a link to
that script and discuss how and why the parameters are set in this way. Or if
you have a material(s) that parameterise a shader, show where these are applied
in the project and how they are used.

### Summary of Contributions

Your team should include a brief summary of the work that each team member did.
Each team member may wish to include direct links to files in the repository
that demonstrates their code contributions in this section (i.e., `.cs` and
`.shader` files). This level of detail is not a strict requirement, and isn't
directly marked, but it will help us to make decisions in the event that there
are disputes over contributions in the [team member
evaluation](#milestone-4-team-member-evaluation).

> **Warning**<br>
> All team members are expected to check that their contributions are well
> documented in the report before the final submission, and that they are happy
> with the summary of their contributions relative to the other team members. 

### References and External Resources

Your team should maintain a list of **all** external resources that were used
in the project, directly or indirectly (see the [Academic
Honesty](#academic-honesty) section below for details on our expectations
regarding external resources).

### Other Details

You may wish to include other sections in your report, such as a discussion of
interesting graphical/technical challenges that you faced, and how your team
solved these challenges. This is not a requirement, but you are welcome to
include such sections if you wish to highlight certain aspects of your team's
work for the marker to take on board. If you do this, please keep the report
concise and organised, and ensure that it is easy to navigate (maintaining a
table of contents at the top of the report is a preferable).

## WebGL Builds

Your game will be deployed and marked as a WebGL build (in a modern web
browser). This is the only deployment method that will be supported for this
project, and it won't be marked if it does not run in this environment. You
should regularly build the game locally, and at least periodically via
Gradescope as outlined [below](#gradescope-submissions).

> **Warning**<br>
> If your project works within the Unity editor, this does not necessarily mean
> that it will work as a WebGL build. Build your game on a regular basis to
> ensure that it works as expected, and that you're not dealing with unforeseen
> issues right before a deadline.

To build your game within Unity, go to `File > Build Settings > WebGL` (you
might need to "switch platform"), then click `Build and Run` and choose a
target folder. If the build is successful, Unity will create a simple local
webserver and open the game in your default web browser. For a detailed guide,
see [this page](https://docs.unity3d.com/Manual/webgl-building.html). 

**Avoid changing the WebGL build settings** that came with the template, as this
might lead to unexpected issues during marking. If you feel you must modify
something, ask the teaching team first. We will not be as lenient as we were in
Project 1 regarding last-minute failed builds, especially if it is due to
careless overwriting of such settings.

## Gradescope Submissions

A submission via Gradescope is required for every team-based submission
(milestones 1-3). To make a submission, complete the following steps:

1. Ensure that the GitHub repository is up-to-date, and that the latest changes
   are merged into the `main` branch (if your team is using branches). Remember that it is an expectation that the latest version of the project is on the `main` branch by each milestone deadline.
2. The **team leader** must submit the project repository on Gradescope, which
   can be opened via the [LMS assignment
   page](https://canvas.lms.unimelb.edu.au/courses/154322/assignments/420267?module_item_id=5127103).
   This will require linking their GitHub account to Gradescope, if they
   haven't already done so.
3. The **team leader** should wait for the autograder to validate the
   submission, and finish building the Unity project in your team's repository,
   as detailed below. 
4. Once the auto-grader has finished running, the **team leader** must add all
   team members to the Gradescope submission. See [this
   guide](https://help.gradescope.com/article/m5qz2xsnjy-student-add-group-members)
   if you are unsure how to do this.
5. **All team members** are expected to verify that they can see the submission
   on Gradescope, and that the correct version of the game is deployed (see
   below). If you're having issues, please contact the teaching team via a
   private post on the discussion board.

After you submit, the Gradescope autograder will perform some simple validation
tests. If these pass, it will trigger a build in your team's project repository
using the **most recent** commit on the `main` branch, and attempt to deploy the build to GitHub
pages (this process occurs within your repository via GitHub actions). There
will be a direct link to it on the Gradescope submission confirmation page,
once the autograder has finished running.

**The build accessed via this link is the build that will be marked, so verifying that this link on
Gradescope opens your game as expected is _essential_!** All team
members are expected to do a check of the final submission, and make sure that
they are happy with what has been submitted. As such, we will not be able to
consider any issues raised after the deadline.

> **Note**<br>
> Builds can take a long time to complete, especially if there are a lot of
> assets. Take care to manage resources appropriately, and avoid including
> unnecessary assets or scenes in your project. 

## Late Submission Policy

#### Team submissions

The deadline for the **final submission** ([milestone
3](#milestone-3-final-submission)) is strict, with write-access to the GitHub
repository locked at the deadline. You are not allowed to make any further
changes to your repository after this point. Please contact the subject staff
immediately if you wish to make a late submission, so that the repository can
be temporarily unlocked.

> **Warning**<br>
> The penalty for late submission of milestone 3 is 10% of the total available
> marks (6 marks) per day or part thereof, up to a maximum of 5 days. After
> this time, late submissions will not be accepted.

Penalties also apply for late completion of the earlier team milestones, but
these fall under the marking criteria outlined above. 

#### Individual submissions

The deadline for the **Team Member Evaluation** ([milestone
4](#milestone-4-team-member-evaluation)) is also strict, with late submissions
not being accepted (the peer review portal automatically shuts). Failure to
submit will be taken to be an indication that you have not contributed to the
project, and an individual mark of zero will be given.

While the deadline for the **Team Feedback Reflection** ([milestone
5](#milestone-5-team-feedback-reflection)) is again strict, this task is
optional. However, it is your only opportunity to respond to any issues raised
in the team member evaluation, so keep this in mind as we will not be able to
consider any responses made after the deadline.

## Academic Honesty

Every member of your team is expected to follow the University's [Academic
Honesty](https://academichonesty.unimelb.edu.au/) policies. To ensure that you
properly attribute work that is not your own, your team must:

- Include a "References" section at the end of your repository's `README.md`
  outlining all external resources used.
- For code or game logic, you must **also** include comments within the respective sourcecode files providing direct link(s) to the sources utilised. 

Submitting work that a member of your team has not authored, without proper
attribution, is considered academic misconduct. Also bear in mind that heavy
reliance on external resources may result in a lower mark, as it is difficult
to assess your own understanding of the concepts involved.

### Use of AI Tools (e.g., ChatGPT)

Please see the University's [stance on AI Tools](https://academicintegrity.unimelb.edu.au/plagiarism-and-collusion/artificial-intelligence-tools-and-technologies). In particular:

> If a student uses artificial intelligence software such as ChatGPT or
> QuillBot to generate material for assessment that they represent as their own
> ideas, research and/or analysis, they are NOT submitting their own work.
> Knowingly having a third party, including artificial intelligence
> technologies, write or produce any work (paid or unpaid) that a student
> submits as their own work for assessment is deliberate cheating and is
> academic misconduct.

If you use an AI tool to develop any component of the project, you **must**
cite it in your `README.md` file (under the "references" section), and outline
exactly how it was used. 

### Unity Asset Store

Use of the Unity asset store strictly limited to importing artistic assets. In
simple terms - images, models, animations, sounds and music tracks are fine,
but not code, components, game logic, or non-artistic prefabs. Note that it is
possible to get a great mark without using "flashy" external resources! You are
assessed based on what you create, and how well you address the criteria in
this specification. In other words, producing a fun and well polished game with
consistent visuals is much more important than sourcing "AAA game" assets.

### Credit where credit is due ...

Remember, we expect that a majority of your submission is your team's
regardless. Full credit will not be awarded where there is an over-reliance on
others' work, even if it is attributed. We will be checking for similarity
between submissions and with code available over the Internet.

## Resources and Help

Check out the following resources for help with this project:

- [FAQ (Ed Discussion)](https://edstem.org/au/courses/12266/discussion/1537508) - A list of frequently asked questions about the project, which will be
  updated throughout the duration of the project.
- [GitHub Markdown](https://guides.github.com/features/mastering-markdown/) - A
  comprehensive guide to "GitHub Flavoured" Markdown, the formatting language
  to be used in your `README.md`/`GDD.md` files.
- [Unity Learn](https://learn.unity.com/) - Unity's official learning platform,
  with tutorials and courses for all skill levels.
- [Unity Documentation](https://docs.unity3d.com/Manual/index.html) - Unity's
  official documentation, with detailed information on all aspects of the
  engine.

If you can't figure something out, or are unsure about something in the
specification, feel free to reach out to your tutor or post on the discussion
board (please also read the
[FAQ](https://edstem.org/au/courses/12266/discussion/1537508) before posting).
