

[Title](#navigating-challenges-with-unresponsive-partner-teams)

[Context](#context)

[Handling](#handling)


# Navigating Challenges with Unresponsive Partner Teams


## Context 

This example is from an infrastructure(PaaS) team. Its product/framework/service is used by internal teams (referred to as customer team) with in the same company.

Your product/service got an incident reported by a customer team. 
Your team triaged the incident and found out that, in-order to confirm the root cause, they need more information from a downstream dependency team. 
The customer team’s leadership is asking for a root cause analysis and corrective action items. 
The incident is not a high priority incident and SRE/command-center teams are not driving it. 
The onus is on you (as Engineering Manager for the infrastructure team) to drive this to closure and respond to the customer team's leadership.

### Terms used - 

+ `Team D` - team on which your team is dependent upon for finding the root cause 

+ `DM` - Engineering Manager of team D 

+ `Team C` - customer team which reported the incident 

+ `Team P` - your own team which manages the product on which the incident is reported 

### Actions Taken So Far

+ You tagged `Team D` and their manager `DM` in incident slack channel.

+ Sent direct message to `DM` in slack asking for a response on incident 

+ Waited for `Team D` to respond in reasonable time limit (for e.g., 24 hrs. for a P3 incident) 

### Anticipated Outcomes or Expectations

There are no incidents 🙂 (in a perfect world) 

`Team D` responds promptly, begins triage and shares the information with `Team P`. 
Based on analysis, both teams decide who is the correct owner for driving the triage ahead. 

The team driving the triage, take the responsibility of providing timely updates to `Team C` and other stakeholders for progress and action items. 

### What Actually Happened 

`Team D` did not respond or begin triage in a timely manner. 
You did not get any response from `Team D` manager for your slack message.
`Team C` leadership is waiting for the root cause analysis and action items to prevent similar issue to happen in future.

## Handling

### Approach 1 - When it's a onetime occurrence 

Set up a meeting with `DM`. Try to understand their side of the story for why there is a delay in response. 
May be `Team D` is busy with other high priority incident triage and simply does not have bandwidth to investigate this incident. 

Tell `DM` that you understand their side of the story. Present these options:

+ Could we establish a process for acknowledging incidents and providing estimates for their resolution? 

+ Could we consider tagging a SME (Subject Matter Expert) on the Slack channel to acknowledge the incident? 

#### Benefits 

Implementing this approach can contribute to building a reliable relationship between you and the `DM`. 
This, in turn, will facilitate smoother handling of future incidents. 

#### Leadership Principle in Action

+ Trust Each Other 


### Approach 2 - When it's a repeated occurrence 

If `Team D` remains unresponsive after trying Approach 1, follow this course of action:

+ Document Incident: Compile an incident report detailing the previous triage efforts and the information required from `Team D`. Within this document, assign an action item to `DM`.
+ Organize a Meeting: Arrange a meeting involving the managers of `Team D`, `Team C`, and `Team P` (i.e. you). Present the analysis report and request `DM` to take ownership of the assigned action item.
+ Escalate to Next Level: If engagement and ownership commitment aren't obtained from `DM`, escalate the matter to the next level of leadership within `Team D` through an email. Keep your own next-level leadership in the email loop. This might help to get a resolution faster.
+ Focus on Customer Experience: In your escalation email, emphasize that the intention is not to blame `Team D`, but to deliver the expected customer experience.
+ Confirm Ownership: Upon `Team D` agreeing to take ownership, notify `Team C` about the new arrangement and that `Team D` will lead the resolution efforts, providing regular updates.
+ Request Regular Updates: If updates are not received within a reasonable timeframe (e.g., 24 hours), utilize the escalation email thread to ask for an update from `DM`. Also, request the updates be shared with `Team C` through the slack channel.
+ Resolution and Appreciation: Once the issue is resolved, use the email thread to express gratitude to `Team D`. Highlight the collaborative spirit and customer-centric approach demonstrated by both teams.

#### Benefits 

Taking these steps to address issues, fosters trust with `Team C`, showcasing your commitment to resolving customer concerns effectively.
When `DM` observes you escalating matters to `Team D` leadership, they are likely to prioritize prompt responses to future engagement requests.
This highlights the impact of your actions on expediting resolutions. 

#### Leadership Principles in Action

+ Do the Right Thing 

+ Be Transparent 
