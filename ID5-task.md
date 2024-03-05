---
name: '#5 Task'
about: 'Task that should be linked to user story #1'
title: 'Squash with Traceability to Task and PR in Commit Message Integration Strategy, but with Some Commits in the Branch Referencing the Task'
labels: ''
assignees: ''

---

References user story #1

## TODO:
- [ ] :question: Answer question `Task5_Q1` on Canvas
- [ ] :bust_in_silhouette: Assign yourself to this task (this will prompt the [WorkflowLearning GitHub App](https://github.com/apps/workflowlearning) to create the `task_5_squash_with_link_to_task` branch)
- [ ] :hourglass_flowing_sand: Wait (at most) 60 seconds until the [WorkflowLearning GitHub App](https://github.com/apps/workflowlearning) will comment on this task and confirm that the branch `task_5_squash_with_link_to_task` was created (refresh the page if you don't see the confirmation comment)
- [ ] Create a new PR having the **base** branch `master` and the **compare** branch `task_5_squash_with_link_to_task`
- [ ] Edit the description of the PR to reference this task
- [ ] :brain: Understand the commits and file changes made in the PR
- [ ] :question: Answer question `Task5_Q2` on Canvas
- [ ] :arrows_counterclockwise: Refresh this page (to ensure that any commits referencing this task are shown on this page) and scroll all the way to the bottom of the page
- [ ] :question: Answer question `Task5_Q3` on Canvas

<h4 align='center'>Starting integration...</h4>

- [ ] In the PR, integrate the changes into `master`
- using the `Squash and merge` option
- with the squashed commit message `Closes #5 (#<ID_PR>)` and
- with an empty squashed commit extended description (i.e., **delete the entire squashed commit extended description, which lists the individual commits that are in the pull request**)

<h4 align='center'>Integration completed.</h4>

- [ ] :eyes: Inspect the history of all the branches and commits via [`Insights` -> `Network`](../network)
- [ ] :x: In the PR, use the GitHub interface to **delete** the branch (since the branch content was successfully integrated into `master`)
- [ ] :eyes: Inspect the history of all the branches and commits via [`Insights` -> `Network`](../network)
- [ ] :arrows_counterclockwise: Refresh this page (to ensure that any commits referencing this task are shown on this page) and scroll all the way to the bottom of the page
- [ ] :question: Answer question `Task5_Q4` on Canvas
- [ ] :question: Answer question `Task5_Q5` on Canvas

## :thumbsup: Advantages of this workflow
Any developer inspecting the squashed ("atomic") commit in `master` can directly navigate
- to task `#5` or
- to the PR (to see all the intermediate commits for the implementation)

## :heavy_exclamation_mark: Disadvantages of this workflow
If the branch contains multiple commits (each containing a partial/incomplete implementation of the task) that are referencing task `#5` (like it was the case with branch `task_5_squash_with_link_to_task`), then these commits will automatically appear in task `#5` as being referenced, and this unnecessarily clutters task `#5` and confuses any developer trying to understand the changes performed in task `#5`.
