---
name: '#6 Task'
about: 'Task that should be linked to user story #1'
title: 'Squash with Traceability to Task and PR in Commit Message Integration Strategy, without Any Commits in the Branch Referencing the Task'
labels: ''
assignees: ''

---

References user story #1

## TODO:
- [ ] :question: Answer question `Task6_Q1` on Canvas
- [ ] :bust_in_silhouette: Assign yourself to this task (this will prompt the [WorkflowLearning GitHub App](https://github.com/apps/workflowlearning) to create the `task_6_squash_preferred_project_workflow` branch)
- [ ] :hourglass_flowing_sand: Wait (at most) 60 seconds until the [WorkflowLearning GitHub App](https://github.com/apps/workflowlearning) will comment on this task and confirm that the branch `task_6_squash_preferred_project_workflow` was created (refresh the page if you don't see the confirmation comment)
- [ ] Create a new PR having the **base** branch `master` and the **compare** branch `task_6_squash_preferred_project_workflow`
- [ ] Edit the description of the PR to reference this task
- [ ] :brain: Understand the commits and file changes made in the PR
- :thumbsup: Notice that the commits in the branch **DO NOT** reference this task `#6`. This is intentional, as to not clutter this task with references of commits containing partial (and incomplete) implementations (that do not contain the entire change in one commit), and which can be altered in subsequent commits in the same branch
- [ ] :question: Answer question `Task6_Q2` on Canvas
- [ ] :arrows_counterclockwise: Refresh this page (to ensure that any commits referencing this task are shown on this page) and scroll all the way to the bottom of the page
- [ ] :question: Answer question `Task6_Q3` on Canvas

<h4 align='center'>Starting integration...</h4>

- [ ] In the PR, integrate the changes into `master`
- using the `Squash and merge` option
- with the squashed commit message `Closes #6 (#<ID_PR>)` and
- with an empty squashed commit extended description (i.e., **delete the entire squashed commit extended description, which lists the individual commits that are in the pull request**)

<h4 align='center'>Integration completed.</h4>

- [ ] :eyes: Inspect the history of all the branches and commits via [`Insights` -> `Network`](../network)
- [ ] :x: In the PR, use the GitHub interface to **delete** the branch (since the branch content was successfully integrated into `master`)
- [ ] :eyes: Inspect the history of all the branches and commits via [`Insights` -> `Network`](../network)
- :tada: :smile: **FUN FACT**: the branch `task_6_squash_preferred_project_workflow` was deleted (more accurately hidden) from the repository, because GitHub keeps all deleted branches indefinitely, which means the commits in the branch (and the PR) can always be accessed
- [ ] :arrows_counterclockwise: Refresh this page (to ensure that any commits referencing this task are shown on this page) and scroll all the way to the bottom of the page
- [ ] :question: Answer question `Task6_Q4` on Canvas
- [ ] :question: Answer question `Task6_Q5` on Canvas

## :thumbsup: Advantages of this "preferred workflow" (which will be used throughout the remaining sprints of the group project)
Any developer inspecting the squashed commit in `master` can directly navigate
- to task `#6`, which will be referenced by only one "atomic" commit containing the final implementation of the task, and this commit can be easily deployed or [cherry-picked](https://git-scm.com/docs/git-cherry-pick) to other branches if needed, or
- to the PR (to see all the intermediate commits for the implementation)

:bulb: Again, it is important to highlight that the intermediate (and incomplete) commits in the branch `task_6_squash_preferred_project_workflow` **DO NOT** reference this task `#6` at all, and hence, they do not clutter this task with unnecessary (and confusing) references of partial (and incomplete) commits. Moreover, developers can contribute to the branch without constantly worrying about adding traceability for every intermediate commit, since they only need to establish the traceability to the task and PR once, during the integration.
