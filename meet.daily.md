---
id: y3365btw652ck48bx90y5cx
title: Daily
desc: ''
updated: 1650393896441
created: 1650393873781
documentId: 1rXFHzitEiZP9IoMy_jGJJCfjS5Tdd2QzPEe5ydfPIe0
revisionId: >-
  ALm37BUeTtofXmGyC_csc5uUfiTRNa6f4ZQyKYnMZvaNawvL0V6W6_turi2qvq--WX5LuIOFpJhZRNNh1U97PLY
commentsUpdated: false
---
### 

**@kevin: amplitude resource naming**
- [[Amplitude Resource Naming|dendron://private/area.metrics.sop.amplitude-resource-naming]]: sop on naming charts and cohorts in amplitude and tracking them in dendron
	- @tuling: ack
	- @jerry: ack
	- @joshi: ack

**@kevin: vendor service docs**

We use a lot of external services as a team (github, amplitude, segment, etc).

The following is a convention for documenting relevant details of various external services to socialize best practices and learnings from these various tools.

[[Vendor Services|dendron://dev/vs]]

- @tuling: ack
- @jerry: ack
- @joshi: ack

### 

**@jonathan: add ‘additional data topics’ for meet.metrics to meet.planning**
Since we’re now covering metrics during planning, if you have any additional data topics, please add them to meet.planning ahead of the meeting.  I created a sub-section under Discussions / Data-Topics.

	- @hikchoi: ack
	- @kaan: ack
	- @kevin: ack
	- @tuling: ack
	- @joshi: ack

**@kevin: change in format for weekly planning - we are combining metrics meeting with weekly planning**
- 35min metrics/35min planning
- end time extended to 8:30AM PST (though we'll aim to finish by 8:15AM PST)
	- @joshi: ack
	- @jonathan: ack
	- @hikchoi: ack
	- @kaan: ack
	- @tuling: ack

**@kevin: inactive user interview**

We just did our first inactive user survey, see notes below in [[Report|dendron://private/task.interview-inactive.ashraf-nazar.report]]

No action items, sharing for information though any comments or thoughts always appreciated

- @joshi: ack
- @jonathan: ack
- @hikchoi: ack
- @john: ack
- @kaan: ack
- @tuling: ack

**@kaan: Rollout of self contained vaults**We’re in the process of rolling out self contained vaults as an AB test. I wrote down what’s different about self contained vaults, and how you can enable or disable them here:

[[Self Contained Vaults Rollout|dendron://private/scratch.2022.04.15.163718.self-contained-vaults-rollout]]

I suggest you read this to familiarize yourself with self contained vaults, both for future development and for customer support.

- @joshi: ack
- @hikchoi: ack
- @john: ack
- @kevin: ack
- @tuling: ack
- @jonathan: ack

**@jonathan/@hikchoi: Consolidating to UpperCamelCasing for naming convention on telemetry events**

See Docs Update: [Dendron workspace sync · dendronhq/org-private@d451660 (github.com)](https://github.com/dendronhq/org-private/commit/d451660b075392e61898416882317144e01cbf80).  Code also has a comment now to remind on the new syntax.

- @joshi: ack
- @kevin: ack
- @kaan: ack
- @tuling: ack
### 

**@kevin: rfc about supporting local overrides to dendron configurations**

the purpose here is to support a default configuration while allowing for local modifications (eg. adding your personal vault when using the team vault). details in [https://github.com/dendronhq/dendron/discussions/2759](https://github.com/dendronhq/dendron/discussions/2759)

please leave any comments in the public github discussion

- @kaan: ack
- @hikchoi: ack
- @joshi: ack
- @jonathan: ack
- @tuling: ack

**@kevin: amplitude metric updates**

previous versions of dendron dumped configuration data into amplitude that created over a thousand distinct event property values. this week, we deleted these metrics and put a block on future metrics (in case clients are still running old versions)

updated [[Feature Instrumentation|dendron://private/area.metrics.sop.feature-instrumentation]] to mention this caveat when creating new property values

diff: https://github.com/dendronhq/org-private/commit/f8f01ddc9ee51309531cae60c62660879b91f270

- @jonathan: ack
- @hikchoi: ack
- @joshi: ack
- @kaan: ack
- @tuling: ack

**@kevin: rfc discussing purpose of root.md**

  The role of `root.md` is a frequently brought up question by our users. opened up an rfc proposing to remove it

  . please leave comments inside the gdoc

- @kaan: ack
- @jonathan: ack
- @hikchoi: ack
- @joshi: ack
- @tuling: ack


