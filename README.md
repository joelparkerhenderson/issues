# Issues

Issues come in many flavors, for example feature requests, bug reports, customer complaints, security alerts, team retrospectives, etc.; this page describes how our team uses issues, and how we communicate about them.

## What is an issue?

For our teams the word "issue" is a generic term such as:

Examples:

* A feature request
* A bug report
* A customer complaint
* A security alert
* A team retrospective


## Public or private?

For many of our projects we use a public issue and a private issue.

For a public issue:

* Emphasize summarization.

* Highlight actionable information.

* Omit/redact all confidential information.

For a private issue:

* Emphasize thoroughness.

* Highlight exploratory information; this helps find patterns across issues.

* Include confidential information as approriate.


## Score

We score each issue in ways that help us compare them, to know what we want to work on. There are a variety of ways to score, and here are some we've seen work well in practice.


### Score by priority

Score by a priority rank:

  * Example: "Priority 1" means do this first, "Priority 2" means do this second, "Priority 3" means do this third, etc.

  * Analogy: a todo list where priority 1 is your highest priority.

  * Pros: easy to understand what the team will work on and in what order; compatible with many bug trackers, todo list apps, and task management tools.

 
### Score by severity

Score by a severity scale:

  * Example: "Severity 1" means minimum impact, "Severity 5" means maximum impact.

  * Analogy: a severe weather warning scale, which ranges from 1 (minimum impact) to 5 (maximum impact), or an earthquake Richter scale, which ranges from magnitude 1 (trivial damage) to 9 (extreme damage), or a hospital pain numerical rating scale, which ranges from 0 (hurts the least) to 10 (hurts the most).

  * Pros: easy to understand the impact; can use many real world analogies; different evaluators can assess severity in each of their own perspectives, independent of what to work on first.


### Score by category

Score by a category name:

  * Example: The category mnemonic "MoSCoW" which we describe as "must have", "should have", "could have", "would have". Each "must have" issue is critical to the current delivery in order for it to be a success, and if even one "must have" issue is not complete, then the delivery is a failure. We like to use the phrase "would have" (instead of the usual "won't have") because in our experience with stakeholders, using "would have" wording shows that an issue is still possible to be included in a release and/or roadmap.

  * An analogy is a conversation about something you want.

  * Pros: the plain English wording of the categories has value in getting stakeholders to better understand the impact of setting a priority, compared to alternatives like High, Medium, Low.


### Score by combination

Score by a combination of priority and/or severity and/or category and/or tag:

* Example: an important customer is coming into the office in an hour to sign a contract, and the team finds a misspelling in the customer's company name on the website. 

* The sales team may score this issue as Priority 1 meaning work on it first.

* The programmer may score this issue as Severity 1 meaning the software impact is not at all severe.

* The product manager may score this issue as Category "could have" meaning the app could have the issue fixed or not because the issue doesn't actually affect the usability of the software.


## Issue template

An issue template can help a team cover important areas efficiently and succinctly.

Our issue template uses:

  * Chief Complaint (CC): summarize the problem as reported by the affected person.

  * Participants (Pt): who is involved, such as users, employees, partners, specific people, etc.

  * Symptoms (Sx): what is going wrong on the surface, such as the users' perspectives, or triggers, or alerts, etc.

  * History (Hx): relevant background information, such as prior similar issues, or reports, or references, etc.

  * Diagnosis (Dx): what is going wrong under the surface, such as the root causes, or cascading causes, etc.

  * Prognosis (Px): what is the prediction, such as a forecast, potential outcomes, changes in effects, etc.

  * Fracture (Fx): what is broken, such as a failed part, or crashed application, or stuck process, etc.

  * Treatment (Tx): what we're doing to make it better, such as action items, to do lists, mitigations, etc.

Our issue template is this file: [TEMPLATE.md](TEMPLATE.md)


## Postmortem triggers

Postmortem triggers can make it easy and fast for a team to know when to do a postmortem writeup.

Postmortem triggers can include:

 * Any user-visible issues, such as unexpected outages or errors.

 * Any on-demand intervention, such as by engineers or executives.

 * Any manual incident discovery, because this shows we need monitoring.

 * Any request by a stakeholder for a postmortem, or review, or mitigation.


## Blameless postmortems

Blameless postmortems focus on the incident's symptoms, causes, and treatments, rather than focus on blaming a person or a group of people.

Blameless postmortems start by affirming that everyone has good intentions, and does their best they can at the time, with the information they have at the time.

# Posts about issues, incidents, postmortems, etc.

* [Post-Mortem Meeting Template and Tips by Brett Harned at TeamGannt on 2017-09-05](https://www.teamgantt.com/blog/post-mortem-meeting-template-and-tips)
