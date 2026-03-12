# Functional Requirements

## Purpose

This document defines the core functional requirements for the TODO application.

## Core Requirements

1. The application must allow a user to create a new task.
2. The application must require each task to include a title or name.
3. The application must allow a user to optionally add a description to a task.
4. The application must allow a user to assign a due date to a task.
5. The application must allow a user to assign a priority to a task.
6. The application must support exactly three priority values: low, medium, and high.
7. The application must allow a user to edit an existing task, including its title, description, due date, and priority.
8. The application must allow a user to mark a task as completed.
9. The application must allow a user to mark a completed task as not completed.
10. The application must allow a user to delete a task.
11. The application must display all saved tasks in a task list.
12. The application must visually distinguish completed tasks from incomplete tasks.
13. The application must sort tasks in a consistent order.
14. The default sort order must place incomplete tasks before completed tasks.
15. Within incomplete tasks, the application must sort by due date, with the earliest due date first.
16. When multiple tasks have the same due date or no due date, the application must sort higher priority tasks before lower priority tasks.
17. If tasks are still tied after due date and priority are applied, the application must sort newer tasks after older tasks.
18. The application must preserve task data after the page is refreshed.
19. The application must load previously saved tasks when the user opens the application.
20. The application must validate user input and prevent creation or saving of a task without a valid title.
21. The application must provide clear feedback when a task is added, updated, deleted, or cannot be saved.

## Task Data Requirements

Each task must support the following fields:

- Unique identifier
- Title or name
- Optional description
- Completion status
- Due date
- Priority: low, medium, or high
- Created date
- Last updated date

## Out Of Scope

The following capabilities are not required for the initial version unless they are added later:

- User accounts or authentication
- Sharing tasks with other users
- Recurring tasks
- Subtasks
- Notifications or reminders