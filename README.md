# Issues

Issues come in many flavors, for example feature requests, bug reports, customer complaints, security alerts, team retrospectives, etc.; this page describes how our team uses issues, and how we communicate about them.

* [What is an issue?](#what-is-an-issue)
* [Public issue or private issue?](#public-issue-or-private-issue)
* [Score](#score)
* [Score discussion](#score-discussion)
* [Issue template](#issue-template)
* [Postmortem triggers](#postmortem-triggers)
* [Blameless postmortems](#blameless-postmortems)
* [Posts about issues, incidents, postmortems, and more](#posts-about-issues-incidents-postmortems-and-more)

## What is an issue?

For our teams the word "issue" is a generic term such as:

Examples:

* A feature request
* A bug report
* A customer complaint
* A security alert
* A team retrospective

## Public issue or private issue?

For many of our projects we create a public issue and a private issue.

The public issue is external-facing intended for our users, customers, promoters, etc.

The private issue is internal-facing intended for our employees, contractors, partners, etc.

### For a public issue

Emphasize summarization.

Highlight actionable information.

Exclude confidential information.

### For a private issue

Emphasize thoroughness.

Highlight exploratory information because this helps discover patterns across issues.

Include confidential information as approriate.

## Score

We score each issue in ways that help us compare them, to know what we want to work on. There are a variety of ways to score, and here are some we've seen work well in practice.

### Score by priority rank

Example: Priority 1 (do first), Priority 2 (do second), Priority 3 (do third), etc.

Analogy: a to-do list, where Priority 1 is your first priority.

Pros: easy to understand what the team will work on and in what order; compatible with many bug trackers, todo list apps, and task management tools.

Misguided: some teams use Priority 0 (P0) to mean emergency alert or release blocker.
 
### Score by severity of impact

Example: Severity 1 (minimal impact) to 5 (catastrophic impact).

Analogy: the Saffir-Simpson Hurricane scale of 1 (minimal), 2 (moderate), 3 (extensive), 4 (extreme), 5 (catastrophic).

Benefits: easy to understand in terms of business impact; can use real world analogies; good for color coding from green to red; different evaluators can assess severity in each of their own perspectives, independent of what to work on first.

Misguided: some teams reverse the scale and use Severity 1 (catastrophic impact) to 5everity 5 (mimimal). We discourage this because it's reversed.

### Score by magnitude of damage

Example: Magnitude 1 (minor damage) to 10 (catastrophic damage).

Analogy: the Richter earthquake scale from 1 (minor damage) to 10 (permanent total destruction).

Benefits: easy to understand in terms of customer impact; can use real world analogies; good for brightness coding from light to dark; different evaluators can assess severity in each of their own perspectives, independent of what to work on first.

### Score by size name

Example: increasing size names "Small", "Medium", "Large".

Analogy: clothing sizes.

Benefits: easy to understand approximately how much work needs to be done.

### Score by harm grade

Medical practitioners use a harm grade to rank patient issues: No Harm, Low Harm, Moderate Harm, Severe Harm, Fatal.

If you're interested in this score, and the specifics of each harm grade, then you can read more about it searching UK NHS Learn from Patient Safety Events (LFPSE).

### Score by level of danger

Example: international regulations define five levels of failure conditions, categorized by their effects on the aircraft, crew, and passengers.

Level A – Catastrophic: Failure may cause multiple fatalities, usually with loss of the airplane.

Level B – Hazardous: Failure has a large negative impact on safety or performance, reduces the ability of the crew to operate the aircraft due to physical distress or a higher workload, or causes serious or fatal injuries among the passengers.

Level C – Major: Failure significantly reduces the safety margin or significantly increases crew workload. May result in passenger discomfort (or even minor injuries).

Level D – Minor: Failure slightly reduces the safety margin or slightly increases crew workload. Examples might include causing passenger inconvenience or a routine flight plan change.

Level E – No Effect: Failure has no impact on safety, aircraft operation, or crew workload.

### Score by MoSCoW requirement

Example: MoSCoW is a mnemonic for "must", "should", "could", "won't". A feature is "must have", "should have", "could have", "won't have" (or "would have").

Analogy: any planning conversation when a person says "We must do this" or another person says "This is a nice to have".

Benefits: the plain English wording of the categories is valuable in getting stakeholders to talk about issues; widespread use among user interaction experts.

Note: We prefer to use the word "would" (instead of "won't") because in our experience with stakeholders, "would" shows that an issue is still possible to be included in the future if something changes; we say "would if X".

### Score by frequency rate

Example: "Frequency 1%" means 1% of use is affected, "Frequency 100%" means 100% of use is affected.

Analogy: the rate at which something occurs or is repeated over a particular period of time or in a given sample.

Benefits: measures how often the issue happens; can be a rate phrase such as "20 times per day"; can be a summary word such as "always", "often", "sometimes", "seldom", "never"; can be a percentage such as "80% of use is affected".

### Score by combination

Example: score an issue by a combination of priority, severity, magnitude, size, MoSCoW, frequency.

Suppose an important customer is coming into the office in an hour to sign a contract, and the sales team finds a misspelling in the customer's company name on the website.

* Sales team says Priority 1 meaning work on it first.

* Product team says Severity 1 (minimal impact) because a typo is trivial and doesn't affect others.

* Marketing team says Magnitude 3 (some damage) because the typo ended up on presenation collateral.

* Project manager says size "small" because the work estimate is tiny.

* Design team says MoSCoW "must" because it must be fixed.

* Quality team says Frequency 2% because inspection discovered typos in 2% of customer names.

## Score discussion

This section has score discussion notes. The quotes are excerpted, synthesized, and sometimes anonymized.

"Usually the other orthogonal assessment in addition to severity is frequency. If the bug is unlikely to be seen during regular use, then even if severity is high, the priority might be lowered. This is usually how risk is managed in my experience."

"A developer or tester might be good at specifying how severe a bug is, but doesn't know if everyone hits the issue or just some users hit the issue. The frequency is a different dimension. The severity can then be multiplied by frequency to calculate the priority."

"I think the formula should be: severity * frequency - ease of workaround = priority. So if any of those measures change (e.g. an easy workaround is discovered, or it's determined that the web page that is crashing is also almost never viewed) then the priority should be adjusted. Having just severity without a measure of 'how many people does this impact?' and 'just how badly does this impact them?' seems like it's missing part of the picture."

"The QA engineer sets the severity during the initial investigation based on technical criteria. This is then one of the data points that the product manager uses during triage to set the priority, which is the controlling value from that point in the process onward."

"One user sometimes suffers a total crash, which then loses all their work, which makes them angry. The user would score the issue as highest severity. But if it's just one user experiencing the issue, and it's intermittent, and the user has a workaround such as saving more often, then the product manager would score the issue as low priority."

"Severity is how the reporter sees the problem: if it interferes with their particular use case, it's of the highest severity. Priority is how the project management team sees the bug: highest priority bugs are there because of the most valuable vocal complainers such as high-paying customers, an inconvenienced CEO, etc. Don't use the severity of the bug to rank the priority, because they're not strongly correlated."

"My experience with priority and severity is that, while the distinction may exist academically, the reality is that most people don't understand it. The result being that the words are so frequently misused that, in practice, they are indistinguishable dimensions."

"Google's internal bug tracker has both priority and severity. P0 S0 is most urgent. P2 S2 is standard. P4 S4 is least urgent. It's kind of a running joke that severity is meaningless (because it isn't meaningfully different from priority). On my team for example we leave it at its default value and ignore it completely."

"We use a single priority field. The tester uses a heuristic to assign an initial priority (e.g., crashes are P1, cosmetic are P5). The developer uses this to prioritize which bugs to triage first, and when they've determined a new priority based on customer experience combined with app behaviour, they replace the old priority score with the new priority score. If we really needed to go back and check what the tester assigned, then we use the "history" or "revision" feature in our bug tracking app."

## Issue template

An issue template can help a team cover important areas efficiently and succinctly.

Our issue template uses:

* Chief Complaint (CC): summarize the problem as reported by the affected person.

* Participants (Pt): who is involved, such as users, employees, partners, specific people, etc.

* Symptoms (Sx): what is going wrong on the surface, such as the users' perspectives, or triggers, or alerts, etc.

* Fractures (Fx): what is broken, such as a failed part, or crashed application, or stuck process, etc.

* History (Hx): relevant background information, such as prior similar issues, or reports, or references, etc.

* Investigations (Ix): what we're doing to research the issue, such as the steps we're taking, or tests we're trying, etc.

* Diagnosis (Dx): what is going wrong under the surface, such as the root causes, or cascading causes, etc.

* Treatments (Tx): what we're doing to make it better, such as action items, to do lists, mitigations, etc.

* Prognosis (Px): what is the prediction, such as a forecast, potential outcomes, changes in effects, etc.

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

## Posts about issues, incidents, postmortems, and more

* [Post-Mortem Meeting Template and Tips by Brett Harned at TeamGannt on 2017-09-05](https://www.teamgantt.com/blog/post-mortem-meeting-template-and-tips)
