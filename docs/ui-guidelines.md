# UI Guidelines

## Purpose

This document defines the core UI guidelines for the TODO application. These guidelines are intended to keep the interface consistent, predictable, and easy to extend as new features are added.

## Component Library

- The frontend should use Material UI components as the default building blocks for the application interface.
- Prefer standard Material components before creating custom equivalents.
- Use Material form controls for task creation and editing, including inputs, text areas, date pickers, selects, buttons, dialogs, snackbars, and cards or list items.
- Custom styling should extend Material components rather than replace them unless there is a clear product need.

## Color Palette

The application should use a restrained palette based on dark blue, white, and light gray.

- Primary color: dark blue for primary actions, active states, top-level navigation, and emphasis.
- Secondary color: white for main surfaces and content areas.
- Neutral color: light gray for page backgrounds, dividers, disabled states, and subtle containers.
- Text should remain high contrast against its background.
- Avoid introducing additional accent colors unless they are needed for status communication such as validation or priority indicators.

Recommended baseline palette:

- Dark blue: `#163A5F`
- White: `#FFFFFF`
- Light gray: `#F3F4F6`
- Dark text: `#1F2937`
- Border gray: `#D1D5DB`

## Typography

- The primary font family must be Helvetica.
- Use a fallback stack of `Helvetica, Arial, sans-serif`.
- Typography should follow a clear hierarchy with larger, heavier headings and readable body text.
- Avoid using more than one font family in the application.
- Button labels, form labels, and helper text should remain simple and legible.

Recommended baseline sizes:

- Page title: `32px`
- Section title: `24px`
- Card or item title: `18px`
- Body text: `16px`
- Helper text and metadata: `14px`

## Layout And Spacing

- Use a standard gutter size of `16px` between adjacent layout elements.
- Use a standard page margin of `24px` on desktop screens.
- On smaller screens, reduce outer margins to `16px`.
- Use consistent vertical spacing between sections, form fields, and task items.
- Prefer an `8px` spacing scale for internal padding and alignment decisions.

Recommended spacing scale:

- `8px`: tight internal spacing
- `16px`: standard gutter and default component spacing
- `24px`: page margin and section spacing
- `32px`: larger separation between major content areas

## Core Screen Patterns

- The main TODO screen should clearly separate task entry from the task list.
- Primary actions such as adding or saving a task should use the dark blue primary style.
- Secondary actions such as canceling should use a lower-emphasis Material button treatment.
- Task items should be displayed in Material cards, list rows, or other structured containers with consistent padding.
- Completed tasks should be visually distinct but still readable.
- Empty states should clearly explain that no tasks exist yet and indicate the next action.

## Forms And Feedback

- All task forms should use Material inputs with visible labels.
- Required fields must be clearly marked.
- Validation errors should appear near the relevant input and use accessible error styling.
- Success and failure feedback should use Material snackbar or alert components.
- Interactive controls should provide clear hover, focus, and disabled states.

## Accessibility

- Maintain sufficient color contrast for text, controls, and status indicators.
- Do not rely on color alone to communicate task status or priority.
- All interactive elements must have clear focus states.
- Form inputs must have associated labels.
- The layout should remain usable on desktop and mobile screen sizes.

## Implementation Notes

- Define shared theme values in one place so colors, typography, and spacing remain consistent.
- Reuse Material theme tokens for palette, typography, and spacing whenever possible.
- Any deviation from these guidelines should be intentional and documented in the relevant feature or design notes.