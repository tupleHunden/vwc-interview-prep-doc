# VetsWhoCode Mock Interview Design
* Customer: VetsWhoCode troops preparing for post-training job interview loops
* Authors: RJ Smith, [Others Here]

*Disclaimer: Opinions and thoughts in this document are my own and do not represent the view points or internal processes of my employer Amazon (Audible).

## Overview/Problem Statement

The VetsWhoCode (VWC) course curriculum is broken up into four phases
1. The Core Basics (Onboarding & Fundamentals)
2. Product Development with JavaScript (JavaScript)
3. Serverless DevOps & DivOps (JavaScript at Scale)
4. Becoming a Dev Advocate of You (mentoring, networking, social equity, and interview prep)

Currently interview prep for troops throughout the curriculum is done on an as-needed basis usually triggered by a real interview the troop has been scheduled for.  Interview prep at VWC should be a semi-standardized process with clear expectations & guidance for both the mentors leading the interviews and the troops participating in them.

One of the challenges of attempting to standardize interview prep is the lack of standardization across the industry for what the ideal interview should look like.  FAANG/Big Tech prioritizes good knowledge of algorithms and data structures while not stressing any domain or specific language knowledge for Juniors.  Product focused small to medium size businesses might prioritize domain & language knowledge over the best scaling data structure at all times.  Some companies don't do any technical rounds whatsoever, and others send out take home assessments before even talking to a recruiter. 

This document will aim to address these challenges in a way that will give troops the confidence they need to land their first job.

Assumptions:
1. Interviews with FAANG-level companies requiring the heavier DS&A knowledge is the minority of interviews troops will need to prepare for.
2. VWC can scale with enough mentors to give every troop in each cohort multiple mock interviews during & after training.
3. https://github.com/Vets-Who-Code/web-curriculum and https://vetswhocode.io/syllabus are fairly up to date.

## Goals/In-Scope

- Troops should be given the opportunity to do at least 1 mock interview for each phase of training relevant to what's been learned so far along with continued as-needed mocks until their first job.
- VWC interview program should cover the majority of interview scenarios that troops would realistically encounter.
- Finding enough interested mentors to scale the program to cover more interview scenarios.
- Program produces actionable results getting troops real job offers and doesn't just add complexity and stress to the learning process.

## Non-goals / Out-of-Scope

* System Design Rounds
	* These can be arranged on a case-by-case basis and are usually not included in junior level rounds at most companies
- Non-fullstack web engineering interviews
- Domain specific or language/stack specific interviews outside the normal experience of the mentorship team conducting the interviews
	- e.g. - Troop gets an interview for a position using ClojureScript or Elm, this document won't cover edge cases like these that should be handled on a case-by-case basis.

## Proposed Design

Technical interviewing should be considered a trainable skill prioritized throughout the curriculum and not a step to complete *after* training.

**Phase 1 Integration**

_Skills learned:_ Git, CLI, HTML, CSS, Accessibility, and UX.

_Knowledge technical:_ HTML & CSS questions

_"On-site" Practical:_ Re-build the VWC testimonials page with HTML/CSS

_Behavioral:_  How have you handled conflict with a manager?

**Phase 2 Integration**

_Skills learned:_ Data types, control flow, conditionals, arrays, modern-JS features

_Knowledge technical:_ Basic JS questions

_"On-site" DS&A:_ [Fizz Buzz](https://leetcode.com/problems/fizz-buzz/) & [Running Sum of 1d Array](https://leetcode.com/problems/running-sum-of-1d-array/)

_"On-site" Practical:_  Implement a function that takes in a list of objects then adds a value to each item, then filters the list based on that added items value.

_Behavioral:_  Can you explain a time where a different perspective was introduced that changed your viewpoint?

**Phase 3 Integration**

*Skills learned:* React, Next, Event Listeners, JSX.

*Knowledge technical:* React questions, Next questions

*"On-site" DS&A:* [Two Sum](https://leetcode.com/problems/two-sum/) & [Unique Number of Occurrences](https://leetcode.com/problems/unique-number-of-occurrences/)

*"On-site" Practical:* Re-build the VWC board page with a mocked API that returns different data than what's displayed on the real page.

*Behavioral:*  Can you give an example where you were given incorrect information for a task from a manager and how you handled it?

**Phase 4+**

Continued mock interviews tailored on a case-by-case basis on their needs or what they are expecting to see in a scheduled real interview.  An example of this would be asking Stephan to add features into a mocked Angular application to help prepare for a real interview on Angular.

## Technology

Option 1 - VS Code in-house w/ GitHub
* Editor: VSCode "Live Share" 
* Question Bank:  Git repo for each question that includes unit tests, answered grouped by complexity, and instructions for both the interviewer and the interviewee 
* Pros:
	* Free
	* Easy to implement
	* Most familiar for troops as VS Code is the standard editor
* Cons:
	* Unrealistic in most cases to interview environments
	* Relies on the interviewer giving access to their computer and potentially access to the terminal to run tests
	* Hard to scale, requires a lot of manual effort for interviewers to get up and running

Option 2 - CoderByte (or any other provider) Subscription
* Editor: CoderByte
* Question Bank: Created inside CoderByte (Stored in GitHub as well)
* Pros:
	* Standardized environment
	* Allows for question-based assessments, live interviews, and "take home" style interviews
	* Infrastructure is handled by CoderByte to include terminal access
	* Scales to handle whatever interview requirements VWC needs in the future
* Cons:
	* Expensive ($1,188/yr)
	* Requires everyone to become familiar with CoderByte
	* Could be overkill for current interview requirements

**Suggested Option**

Option 1 to start and if scaling & maintainability becomes an issue migrating to Option 2.

## Risks & Mitigation

* Does VetsWhoCode have enough mentors with enough time to conduct mock interviews?
* Does VetsWhoCode have enough mentors with enough time to build out question banks and become familiar with DS&A questions?

## Open Questions

* What does failing a mock interview mean?
	* What does failing multiple mock interviews mean?
* Is a more formal interview prep process overkill?
