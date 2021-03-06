# Product Development

## Deadlines for major product releases
For major product releases, it may be helpful to establish a deadline, in order to help support account managers in communicating upcoming changes with customers, and in general, help them with general Tilt rollout plans. In particular:
- Victor is responsible identifying major product releases.
- Victor is responsible for establishing these deadlines, in close collaboration with Dan, Nick, and engineering folks in general, especially as it pertains to effort and timeline estimation.
- Victor is responsible for communicating these deadlines to all Tilters _internally_. Account managers are responsible for communicating downstream expectations to customers per their good judgment.
- Everyone should work together to avoid significantly delaying an established deadline, especially if downstream expectations have already been communicated to many customers.
- We should use the due date field on epics and stories to capture deadlines. We should apply the due dates to the final marketing deliverables (e.g. blog posts, docs), instead of product change deliverables, so that account managers are equipped with artifacts to share with customers.

## Encourage users to create and subscribe to GitHub issues
We use Clubhouse stories and epics to track product changes. But we rely on GitHub issues to engage with the Tilt community. In addition to the [Exterminator creating GitHub issues for feature requests](../user-support/README.md#exterminator), Tilters should encourage all users to create GitHub issues, subscribe to existing issues, and 👍 them. In particular, by subscribing to an issue, a user will get a notification when it is closed (possibly informing them that a feature request is now implemented), bringing them back to Tilt for further product discussion.

## Workflow
We want a good internal workflow so we can understand our customer pain points, collaborate to solve their problems, and measure the effectiveness of what we release.

<img src="images/workflow.png" height="550" />

The illustration above maps the people, tools, and deliverables in this product development cycle. Ideally, we run a flow where conversations with customers drive an internal process where high-level strategy informs the scoped and defined product changes we ship. And when we ship to customers, we measure impact so we can continue to adjust what we strategize and deliver.

### Free-form discussion in Clubhouse stories
All Tilters are encouraged to collaborate in _discussing_ general ideas in a free-form fashion, with no strict process, no structure, no specific timelines, and no specific implementation commitments. Tilters should prefer discussing ideas in Clubhouse stories, linking ideas together, thus building a web of good ideas that are easily searchable for posterity.

### Defining high-level business initiatives with Clubhouse epics
All Tilters are encouraged to collaborate in _definining_ high-level business initiatives. Similar to general ideas, there is no strict process for collaboration, except that each business initiative should be documented as a Clubhouse epic. As an epic becomes increasingly well-defined over time, it should have more and more of these components with increasing fidelity:
- Problem statement
- Solution scope
- Attached stories with relevant ideas, including designs
- Link to specific metrics and/or charts that this change targets to improve

## Before an Epic Starts

### Unstarted Epics

To start, Victor is the owner of all epics until they are assigned to
someone. Victor is responsible for ensuring that the [backlog of unstarted
epics](https://app.clubhouse.io/windmill/epics?state_ids=500008016&state_ids=500008001)
is continually full and that epics are increasingly being better defined. There
should be no shortage of epics.

If you have a question or comment about an unstarted epic's scope, design, timeline, priority, or any other aspect, you should direct it at Victor.

<img src="images/epics-priority.png" height="100" />

### Epic Priority

Dan B and Nick, and Victor are responsible for maintaining a rough priority of
the backlog (higher priority toward the top in the Clubhouse view, when the
triangle is pointing down).

Higher epics should be more well-defined. As we go down, it's OK if the epics
are less well-defined and more loosely ordered.

Prioritizing an epic does not make any guarantees about when it will be started
or who should pick it up. It's just a way to help us communicate about what's
important.

Victor is responsible for tracking [open customer requests](https://companies-b164c.firebaseapp.com/customer-requests) as an input for prioritization.

### Epic description template

Before an epic starts, it should contain this template.

The "Problem statement and references" section should be completed. (Other
sections can remain not yet completed.)

Copy and paste the template below into the epic description. Update each section, with as much applicable content as possible. When a section is done, replace `:white_small_square:` with `:white_check_mark:` to indicate it is done.

```
---

# Acceptance criteria
See [Product Development](https://github.com/tilt-dev/company/blob/master/product-development/README.md) for details.

When a section is done, replace :white_small_square: with :white_check_mark:

## :white_small_square: Problem statement and references
- E.g. Tilt users find it difficult to understand the colors in the Tilt Web UI sidebar
- Links to related [Tilt rollout cookbook recipes](https://docs.tilt.dev/rollout)
- Links to Clubhouse/GitHub/Slack/docs

## :white_small_square: Feature discovery and adoption
- How will users discover and adopt this feature? 
- UI change to alert user?
- Assign DevEx engineer in partner team to update Tiltfile?

## :white_small_square: Final scope, implementation, and demo
- E.g. We decided to add tooltips to all the different statuses in the sidebar
- User journey, with links to Figma or screenshots
- Presented (or will present) in [weekly epics meeting](https://github.com/tilt-dev/company/blob/master/product-development/README.md#weekly-epics-meeting)

## :white_small_square: Updated docs and blog posts
- Links

## :white_small_square: Out of scope, related, and/or future work
- Links to Clubhouse/GitHub/Slack/docs

## :white_small_square: Customer validation and metrics
- Links to Slack conversations
- Links to customer docs
- Links to customer metrics dashboards
- Links to internal metrics dashboards
- Links to future work to collect data
```

## How an Epic Starts

### DRIs

Epics are assigned to a
[DRI](https://medium.com/@mmamet/directly-responsible-individuals-f5009f465da4).

The DRI is responsible for:
- maintaining the epic state, description, and attached stories updated as the single source of truth of overall work status
- reducing scope if additional work is discovered
- driving the epic to completion

The acceptance criteria sections are _especially critical_, including presenting
the problem and final implementation in the [weekly epics
meeting](#weekly-epics-meeting).

### How DRIs are Assigned

When assigning DRIs, we're operating on a few hypotheses:

- Projects are far more likely to succeed when the person working on it feels
  connected to the project, and feels it lets them use their skills well.

- Conversely, Tilters should be empowered to try epics they feel strongly about,
  even if other people on the team disagree. Consensus is a bad way to make
  decisions, and we shouldn't require consensus on an idea to move forward.
  
- It's anxiety-producing and not helpful when people are constantly switching
  back and forth between execution and prioritization. We don't want each DRI
  to have to do a prioritization exercise every week when they finish their epic.
  
So we're trying a new system.

Each Tilter is responsible for reading the backlog of epics. They don't need to
understand every epic. But they should understand enough to be able to
affirmatively articulate what epics in the backlog they want to work on and why.

Every two weeks, Nick will talk to you your impressions of the backlog, and try
to get a sense of what you think is important and want to work on.

Nick will assign epics near the top of the backlog, trying to balance
preferences and current priority order.

If there's an epic that's high in priority order but no one wants to work on,
then Nick should dig more into why. Do we need to do more research upfront?  Is
the epic defined incorrectly? Is it misaligned with what we're currently
focusing on?

There may be rare cases where someone gets assigned to an epic that they
don't want to work on, but in those cases we should explicitly call out
that this is happening and why.

At all times, every Tilter should have 1-2 epics assigned to them that haven't
been started yet. The epics are their "Next Up" list.  This isn't final - they
may get reassigned. But we bias towards keeping the current assignment so that
Tilters know what's coming next.

### Starting an Epic

When you're ready to start an epic, it should be clear which epic to start work
on -- it's the highest-priority backlog epic assigned to you.

Move it into the `In Progress` state.

## How an Epic Progresses

A given epic may have a fairly broad initial business problem. The engineer(s) should carve out and define a smaller problem, and spec out a solution that can be accomplished within a target of **_7 business days_** (counted from when the epic moves into `In Progress`, more below on states). 

### Reducing Scope

If the solution cannot be finished within 7 business days, keep reducing scope. 

The DRI should update the epic description with smaller scope and acceptance criteria. They may need to communicate radical changes in scope to other stakeholders, but it's ultimately the DRI's call.

The DRI may create additional epics and/or stories to capture the future work. Alternatively, they may create a separate epic with the smaller scope and start work on that one instead (putting the original epic back into the backlog).

The target time period is business calendar time, regardless of how many folks are working on the epic. So if for unplanned circumstances a person in a two person epic needs to be pulled away, the remaining person (who should be the epic owner DRI) may reduce scope to try to meet the target time period due to reduced capacity, saving the unfinished work for a future epic.

The purpose of a single epic is _not_ to completely solve a business problem. Rather, completing an epic should likely achieve incremental progress at addressing a single problem, adding incremental user value as a result. In some cases, any realized user value may only appear in future epics.

Certain initiatives may require a sustained effort of multiple epics to get to a place where folks are comfortable with the result. Tilters should therefore advocate for epics that close the gap of new but incomplete functionality, or fix tech debt, as per the [advocacy process outlined above](#defining-high-level-business-initiatives-with-clubhouse-epics).

### Example

For example, suppose usability research suggests that the Tilt Web UI right sidebar is difficult for users to learn. Two engineers develop some ideas to iterate on the existing designs in order to address the problems. But they discover that it's a better idea to first re-architect some of the frontend JavaScript and CSS to accommodate the design changes, repaying some previously incurred tech debt. In this case, the first epic's scope would simply be non-user facing code re-architecture work, that doesn't have immediate user impact, but contributes to solving the usability problem indirectly as an incremental first step. The engineers may work on the second epic right after the first one is done, or it may be given to another team, or simply deferred to a future time. By scoping work to smaller units, Tilt is more flexible in prioritizing whatever is best at (almost) any moment of time as a small organization.

## How an Epic Ends

For an epic to be completed (and marked as `Closed` in Clubhouse), the epic description needs to have all the acceptance criteria in its description marked as completed.

Here is an example of how an epic description should look when all the acceptance criteria have been completed.

<img src="images/epic-acceptance-criteria-example.png" height="650" />

Between the end of one epic and the start of a new one, it is OK to knock out small feature requests or [bug fixes](https://github.com/tilt-dev/company/blob/master/development/README.md#assign-yourself-a-bug) that you have context on.

## Weekly epics meeting
There is a weekly meeting for discussing epics where all Tilters are invited. The purpose of this meeting is to make sure that the team is aligned on current work (Tilters know what teammates are working on, blockers are surfaced) and planned work (Tilters advocate to de/prioritize epics, ask questions about existing epics/prioritization), as well as to celebrate wins (demos of completed epics, shout-outs, etc.).

Each meeting will be recorded (with permission from participants) and shared internally for all Tilters to watch if they want, [listed here](https://docs.google.com/document/d/173tL_bu4hs73VXo5kHxU0rDSXFlmKS-gpMJokpcdWE0/edit). Tilters should add agenda topics per the following categories, preferably prior to the meeting starting.

Agenda topics include:
- DRI links to and presents their epic, including problem and final implementation, preferably with a demo. (This presentation is part of an epic's [acceptance criteria](#finishing-an-epic-with-acceptance-criteria).)
- For each in progress epic, the DRI highlights the biggest change and also shouts out to people that have helped, from the past week. This section should also highlight epics that are stalled or taking longer than expected, and give the DRI a chance to ask for help.
- Somebody advocates for an epic to be high priority or otherwise discusses epic priorities. You should add a [meeting agenda item](https://docs.google.com/document/d/173tL_bu4hs73VXo5kHxU0rDSXFlmKS-gpMJokpcdWE0/edit) if you would like to discuss this at the next meeting.

## Weekly company meeting
Victor will use the weekly company meeting to highlight epics (new or otherwise) that have recently moved to high priority or of general interest. Newly-prioritized epics shoud be briefly described, and the reason behind their prioritization explained (e.g.: "this epic is about improving a user's experience with the resource URLs that Tilt surfaces; we've prioritized it because it would be a big quality-of-life improvement for Acme Company for not that much technical work").

## Design process
There is a light-weight design process where work is tracked in Clubhouse stories, in a [separate Clubhouse project / workflow](https://app.clubhouse.io/windmill/stories/space/4524/everything). Victor and Han manage this work for Sascha. Together they ensure that design work necessary for important product changes happens ahead of implementation.

Han and Sascha collaborate actively on design, particularly in the early stages. Sascha is responsible for delivering the final mocks, flows, etc that Victor uses to scope into implementation work. Sascha uses Han as a resource for thinking through complex design issues. To maintain momentum and unblock his work, Sascha works with Victor as his point person for clarifications, reviews, and facilitating collaboration with others. Victor is responsible for bringing in other stakeholders for additional discussion as needed.
