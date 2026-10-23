---
name: dez-ticket-implement
description: To implement tickets
---

## Goal
Implement a ticket for a new feature, bug fix, or improvement in the system.

## Instructions

1. first figure out what ticket should be implemented next, if you are not sure about it, ask the user to provide it.
2. use worktree and use ticket's title as branch name so you can implement the ticket as a separate branch and worktree
2. use grill-me skill to ask user about all unknown requirements and store the result as a md file called research.md under ticket's folder.
3. use ponytail skill to create a plan for the implementation of the ticket, the plan should be iterative incremental to be tested and evaluated more easily
4. check the final plan with user and if confirmed store it as plan.md in ticket's folder.
5. follow the plan and existing conventions to implement the ticket, focus on one iteration and implement it to achieve it goal, do verification according to plan to see if it is done or not
6. At the end update the ticket's status to DONE and put crossed on the definition of done items which are doneand provide a summary of the implementation in the ticket's folder as a md file called summary.md


## Guidelines

- the ticket should be implemented in the order of priority, if you are not sure about it, ask the user to provide it.
- after doing research, the outcome should be stored as a md file called research.md under ticket's folder.
- after planning, the final plan should be stored as a md file called plan.md under ticket's folder.
- after implementing each iteration, the outcome should be verified according to plan to see if it is done or not, if it is not done, then the next iteration should be planned and implemented until the ticket is done.
- act as a moderator and for each step like doing research or planning or implementing an iteration or testing an interation call a new subagent to do the task and provide the result, then you can use the result to do the next step.
