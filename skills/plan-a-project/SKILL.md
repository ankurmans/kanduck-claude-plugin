---
name: plan-a-project
description: Turn a goal, brief or messy list into a Kanduck board with lists and cards. Use when the person asks to plan a project, launch, trip or sprint, or to "put this on a board".
---

# Plan a project on a Kanduck board

Use the Kanduck tools to build the plan where the person will work on it.

1. Call `list_boards` first. If a board for this project already exists, add to it instead of making a second one.
2. If not, call `create_board` with a short title, one emoji, and lists that match how the work flows. For most projects use Backlog, This week, In progress, Waiting on, Done. The last list is where finished cards go.
3. Break the goal into cards with `add_cards`. Add them all in one call. Keep titles under 60 characters and start them with a verb. Put detail in `notes`, steps in `checklist`, and a `due` date only when the person gave one or the plan needs one.
4. Use `set_labels` to define two to four labels (for example Marketing, Engineering) and attach them to cards.
5. Put the first few cards in "This week" and the rest in "Backlog".
6. Reply with the board name, how many cards went into each list, and the board link: `https://kanduck.com/b/<boardId>`.

Only create what the person asked for. Do not delete or rename existing lists or cards while planning.
