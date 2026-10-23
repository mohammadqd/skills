---
name: dez-create-ticket
description: To create tickets to be implemented
---

## Goal
Create a ticket for a new feature, bug fix, or improvement in the system.

## Instructions

1. Fill out the ticket template (assets/ticket-template.md) with the necessary information.
2. Store the new ticket as a file in a new folder with tickets name under the `tickets/` directory, using a descriptive filename (e.g., `issue-12-feature-new-login.md` under `tickets/issue-12-feature-new-login`).
3. Ensure the ticket includes a clear title, goal description, and definition of done and user approves all of them or modifies them to be approved.
4. use grill-me skill to review the ticket and make sure it is clear and complete.
5. use DoD skill to check if the ticket meets the definition of done and make sure it is clear and complete and customise it based on users needs and requirements and preferences.

## Guidelines

- the name of ticket should be descriptive and follow the format `issue-<ticket-number>-<short-description>` and stored as a markdown file in the `tickets/` directory with md extension.
- for ticket number in the ticket title try it to use the next available number in the sequence of tickets, if you are not sure about the next number, please ask the user to provide it.
- for the ticket status start with BACKLOG unless user asks for a different status.
- title of the ticket shoulb be exactly like its file name but short description could be more representative e.g. title: `issue-1-setup-phaser-project` and short description: `Set up the Issue Tracker Phaser project`.
- check if a duplica te ticket already exists in the tickets directory before creating a new one, if it does, ask the user if they want to update the existing ticket or create a new one with a different title.
- if a ticket should be subtask of another, then it should be created under parents folder and the parent ticket should be updated to include the new ticket as a subtask.
- before creating ticket show user the ticket content and ask for confirmation to create it, if user wants to make any changes, allow them to do so before creating the ticket.

## Assets

- template for tickets: assets/ticket-template.md
