# Issues

Issues come in many flavors, for example feature requests, bug reports, customer complaints, security alerts, team retrospectives, etc.; this page describes how our team uses issues, and how we communicate about them.

* []()


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

* Emphasize thoroughness.
* Highlight exploratory information; this helps find patterns across issues.
* Include confidential information as approriate.


## Score

We score each issue in ways that help us compare them, to know what we want to work on. There are a variety of ways to score, and here are some we've seen work well in practice.


### Score by priority

Score by a priority rank:

  * Example: "Priority 1" means high priority, "Priority 2" means medium priority, "Priority 3" means low priority.

  * An analogy is a todo list, where priority 1 is your highest priority.

  * Pros: compatible with typical bug trackers.


### Score by severity

Score by a severity rating:

  * Example: "Severity 1" means least, "Severity 5" means most.

  * An analogy is movie ratings that use 1 star to 5 star.

  * Pros: easy for everyone to understand, especially visually using stars.

  
### Score by magnitude

Score by magnitude scale:

  * Example: magnitude 1 is trivial impact, 9 is extreme impact.

  * An analogy is the earthquake Richter scale.

  * Pros: a suitably wide range, and a well-known analogy.
  

### Score by category

Score by category mnemonic MoSCoW which stands for "must have", "should have", "could have", "would have".

  * Example: Each "must have" issue is critical to the current delivery in order for it to be a success, and if even one "must have" issue is not complete, then the delivery is a failure.

  * An analogy is a conversation about something you want.

  * Pros: the plain English wording of the categories has value in getting stakeholders to better understand the impact of setting a priority, compared to alternatives like High, Medium, Low.
  
  * Notes: MoSCoW traditionally uses "won't have" not "would have"; we choose to use "would have" because in our experience with stakeholders, the "would have" wording tends to be clearer that an issue is still possible to be included in a release, and also is still possible to be included in a future release.


## Priority rank examples

Priority rank examples that are typical in many popular techology projects:

* Priority 0 = Immediate
* Priority 1 = Must have
* Priority 2 = Should have
* Priority 3 = Could have
* Priority 4 = Would have


### Priority 0 = Immediate

* Summary: Do this immediately, update team immediately, and work 24x7 to solution.

* Impact: Severe business loss that is continuing and/or worsening, or the team is in failure state, etc.

* Response time goal? Within X minutes.

* Milestone blocker? Yes.

* Feature examples: None, because no feature is this important.

* Incident examples: System is down, or is corrupting data, or significant customers are entirely blocked.


### Priority 1 = Must have

* Summary: Primary working area

* Impact: typically high number of users and/or high business value and/or high visibility.

* Response time goal? Within X hours.

* Milestone blocker? Yes.

* Impact: Must meet its deadline, otherwise there will be significant business loss, and/or the team fails.

* Feature examples: critical to the current delivery for it to be a success; if even one must-have requirement is not included, the delivery should be considered a failure.

* Incident examples: typically most system crashes, or most data loss, or regressions, or a critical issues for which there is no work around yet other areas of the system are still functioning.


### Priority 2 = Should have

* Summary: Wanted for current milestone; most work should have this priority.

* Response time goal? Within X days.

* Milestone blocker? No.

* Feature examples: Any typical planned feature.

* Incident examples: A bug that has a reasonable workaround, and will be addressed in next significant update.


### Priority 3 = Could have

* Summary: Desirable but not necessary; could improve user experience or customer satisfaction; could take little development time/effort/cost. These will typically be included if time and resources permit.

* Response time goal? Within X weeks.

* Milestone blocker? No.

* Feature examples: an enhancement request; a feature that could improve user experience or customer satisfaction; a feature that could take little development time/effort/cost; a "quick win".

* Incident examples: a bug in a less-used area, or that has a workaround, or that causes insignificant business value loss.


### Priority 4 = Would have

* Summary: least-wanted and/or lowest-value and/or smallest-visibilty items for this milestone; still possible 
to be included in a milestone (though unlikely) and/or still possible to be included in a future milestone.

* Response time goal? Within X months.

* Milestone blocker? No.

* Feature examples: an enhancement request that is minor, or for a small number of customers, or that delivers a relatively small business value.

* Incident examples: a typo, harmless, or otherwise, that is fixable when time is available.


## Issue template

An issue template can help a team cover important areas efficiently and succinctly.

Our issue template uses:

  * Participants a.k.a. Px: who is involved, such as users, employees, partners, specific people, etc.

  * Symptoms a.k.a. Sx: what is going wrong on the surface, such as the users' perspectives, or triggers, or alerts, etc.

  * History a.k.a. Hx: relevant background information, such as prior similar issues, or reports, or references, etc.

  * Diagnosis a.k.a. Dx: what is going wrong under the surface, such as the root causes, or cascading causes, etc. 

  * Fracture a.k.a. Fx: what's broken, such as a failed part, or crashed application, or stuck process, etc. 
  
  * Treatment a.k.a. Tx: what we're doing to make it better, such as action items, to do lists, mitigations, etc. 

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

