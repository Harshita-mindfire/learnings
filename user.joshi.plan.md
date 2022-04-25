---
id: 7qc8ccko6fefzaukecyg0oi
title: Plan
desc: ''
updated: 1650431982573
created: 1650431982573
documentId: 1rXFHzitEiZP9IoMy_jGJJCfjS5Tdd2QzPEe5ydfPIe0
revisionId: >-
  ALm37BWuYeiBt4APqZvRaeFSQi6U17jynLuicAgDdf-DJMuYT21thWCrPysPjZp4qqwSCrk9mHqIuYWGDnQIj3Q
commentsUpdated: true
---
### 

**@kevin: amplitude resource naming**
- [[Amplitude Resource Naming|dendron://private/area.metrics.sop.amplitude-resource-naming]]: sop on naming charts and cohorts in amplitude and tracking them in dendron
	- @tuling: ack
	- @jerry: ack
	- @joshi: ack
	- @kaan: ack
	- @hikchoi: ack

**@kevin: vendor service docs**

We use a lot of external services as a team (github, amplitude, segment, etc).

The following is a convention for documenting relevant details of various external services to socialize best practices and learnings from these various tools.

[[Vendor Services|dendron://dev/vs]]

- @tuling: ack
- @jerry: ack
- @joshi: ack
- @kaan: ack
- @hikchoi: ack

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


### Comments

 - Chengyun Liu:  IMO names-like-this-are-hard-to-read

	 replies to this comment: 

	 - Chengyun Liu: Also, when I'm doing exploratory stuff I want to go fast and discard most of my work - I would only do Dendron linking and formatting for finalized shareable products (cohorts, charts, dashboards)
	 - Kevin Lin: see my response to kaan's comments below
- Kaan Genc:  - Is the naming convention only for the Dendron notes? Can we still use descriptive names on the actual charts?
- Do we need to create a note for all charts? Or only when it's a chart we want other people to be able to reference?

	 replies to this comment: 

	 - Kevin Lin: > - Is the naming convention only for the Dendron notes? Can we still use descriptive names on the actual charts?
yes, will clarify in the doc

> - Do we need to create a note for all charts? Or only when it's a chart we want other people to be able to reference?
no. all charts that are used in reports
- Kaan Genc:  It looks like the biggest thing we need is more documentation. Maybe we should all take some time to write docs and tutorials?

	 replies to this comment: 

	 - Kevin Lin: i think its going to be a mix of better docs but also making things easy enough that users can discover/learn by using dendron
- Jonathan Yeung:  where is this block implemented?

	 replies to this comment: 

	 - Kevin Lin: https://analytics.amplitude.com/dendron/govern/project/322132/advanced/blockfilters
	 - Jonathan Yeung: cool, I haven't looked at this 'govern' tab before
- Hyun Ik Choi:  general comment:

The concierge approach and doing a wizard-of-oz testing again reminded me of the concepts and methodology that user-centered design talks about.

- lightweight experiments

refactoring
- one main point I wanted to learn and verify is that refactoring would be used a lot more if we have simpler refactor-derivative commands.
- we instead of trying to come up with a whole suite of common refactoring patterns and implementing them, we can pick one that we think would be most beneficial and create a quick build with that included.
- we could have users sign up and give us feedback on the experience of using the simplified version of refactor vs the as-is regex based refactoring.

meeting notes
- this may be simpler if we just go ahead and implement something like _Create Meeting Note_ and suggest a default template for it, but I think this is something we can highlight by just recording a video MVP of it by using our existing templating feature and showing off how we do it internally in Dendron.
- pair this with a beta sign-up to gather a group who wants to try out a new set of features revolving around meeting notes, and then get focused feedback from them. (opposed to generally releasing them and adding metrics that we need to wait for to analyze.)
- or maybe just get some templates ready and ask any of our users who mentioned that they use Dendron mainly for meeting notes, and doing a pass of concierge MVP with them.

	 replies to this comment: 

	 - Jonathan Yeung: nice! - @hikchoi, on the refactoring ideas, do you want to add that to the 'build' section of [[Refactoring Hypothesis Testing|dendron://private/proj.2022.04.refactoring-hypothesis-testing]]?
	 - Hyun Ik Choi: will do
- Kaan Genc:  > Note: Edits without saving do not propogate to the engine. The engine reflects the state of the notes on disk so it will not change until the user explicitly saves

This didn't use the be the case, we used to sync the note state as it was edited to the engine. Is that no longer the case?

	 replies to this comment: 

	 - Kevin Lin: yes - this is to reduce calls to the engine. the engine should be a reflection of what is "on disk" - propagating non-saved state to it wasn't a great pattern
	 - Kaan Genc: 
- Hyun Ik Choi:  note: 

- this is not in master yet.
- thanks @kaan for the suggestion!

	 replies to this comment: 

	 - Jonathan Yeung: What about the approach of returning a promise? 

I'm a little weary of having too many test wrappers - for me at least, it makes it harder to read the code and to understand when certain asynchronous issues are occurring.
	 - Hyun Ik Choi: [[Like this?|dendron://private/task.2022.03.29.fix-nav_order-issue-with-tree-view-v1#^7imfowrcov2y]]
	 - Hyun Ik Choi: (just synced again with a better example.)
	 - Hyun Ik Choi: actually, this probably could just be async at this point 😅 I'll keep it around to pass forward an example of how we should test async code.
	 - Jonathan Yeung: 👍
- Hyun Ik Choi:  nice! would be nice they are linked in a docstring for  `NOTE_PRESETS_V4` so they show up in intellisense

	 replies to this comment: 

	 - Kevin Lin: agreed. future work :)
- Kevin Lin:  left small comment, feel free to merge

	 replies to this comment: 

	 - Hyun Ik Choi: merged.
	 - Kevin Lin: 
- John Joaquin:  saving the note, then exporting does not solve the issue of missing tags,details when export is completed. In my case, it is solved when I do Reload Window then export. However, this is taking too much time as it takes 15-20 seconds to complete the reloading.
- Kaan Genc:  Just a heads up that there are known bugs with V1 that seem to be fixed when users migrated to V2. V1 not respecting `nav_order` is one that comes off the top of my head.

Also any thoughts on why we're deprecating V2, rather than deprecating V1 and merging V2 with the website component? Wouldn't that reduce work on our part even more?

	 replies to this comment: 

	 - Kevin Lin: more details on rationale behind deprecating:
- originally, we wanted to use a single tree view for published dendron and dendron in vscode, thus introducing the webview
- the antd tree view does not lend itself well to collapsing on mobile and small screen sizes, after a few iterations, we ended up implementing a custom menu component to manage the "tree view" for published sites
- at this point, tree view v2 is only used in vscode. it is not native to vscode and is using the deprecated `dendron-next-server` method of rendering a web ui (by loading a page within an iframe instead of directly)
- we have an action item to remove `dendron-next-server` and consolidate all views within `dendron-plugin-views`. since treeviewv2 no longer unifies publishing and the code ui, does not have native look and feel, and has some outstanding issues, we decided its best to just remove it completely
	 - Hyun Ik Choi: ah. then we should fix the outstanding bug on V1 before removing V2. I'll take a look if I can get that fixed during my oncall week.
	 - Hyun Ik Choi: @kevin I'll update the rationale section of the impactful change notice with your comment
- Hyun Ik Choi:  added here: [[Deprecated|dendron://private/weekly.journal.2022.03.29#deprecated]]
- Hyun Ik Choi:  This wasn't pushed properly. It is now. Apologies.
- Kevin Lin:  heads up - since this is applicable to both plugin and other tests, can we move the docs for it from plugin.qa.test to [[Test|dendron://dendron.docs/pkg.engine-test-utils.qa.test]]?

	 replies to this comment: 

	 - Tuling Ma: 👍
- Hyun Ik Choi:  Love this! nice.
- Jonathan Yeung:  Yeah, I've had this issue too, and when I want to create a new note I end up navigating back to that `03.24` note
- Jonathan Yeung:  Thanks a lot everyone for the detailed feedback!

I'll add a task to track lookup perf - I have also noticed issues with both leading characters and trailing characters getting dropped.

Harshita is taking a look at some of the issues with note rename, and Mark has an item on tree view / engine reliability.  These coupled with a few other pending changes should hopefully make further improvements to perf and stability.
- Derek Ardolf:  Same. Often needing to reload index, as links aren't loading properly from the latest sync, etc.
- Derek Ardolf:  I'm a big fan of this being a Dendron Doctor command, good to hear :)

	 replies to this comment: 

	 - Hyun Ik Choi: We are generally moving towards 
1. having a command that does it
2. prompting users to do it when we see that they should

instead of running them automatically without consent.

I think the community feedback on this has been positive as well.
- Hyun Ik Choi:  yup. also paired with Harshita today with similar issues with the graph view today. which was super helpful because both were sharing some similar issues.
