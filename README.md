# Daylist

Daylist is a responsive, browser-based task planning workspace. This MVP uses HTML, CSS, and plain JavaScript and stores tasks in the current browser with `localStorage`. It has no server or account system.

## Run locally

Open `index.html` in a modern browser. To serve it over HTTP, run a static web server from this folder, for example `npx serve .`.

## Included

- Overview dashboard with totals, pending, completed and overdue counts, a weekly completion chart, today's tasks, recent tasks, and upcoming deadlines.
- My Day, Upcoming, All Tasks, Important, Completed, Overdue, Archived, category lists, Calendar, and a drag-and-drop Kanban board.
- Create and edit tasks with a description, due date, priority, status, category, and important flag.
- Complete/reopen, archive, duplicate, delete with undo, search title/description/category, filter by status or priority, and sort tasks.
- Light/dark theme, responsive navigation, keyboard shortcut to search, CSV export, and local browser persistence.
- Overview quick-add and a working focus timer with 25-minute sessions and 5-minute breaks.
- Subtle animated accents and completion celebration, with reduced-motion preferences respected.
- Existing tasks from the earlier Daylist version are migrated when the app loads.
- First-time visitors start with ten editable demo tasks across dates, priorities, categories, and statuses; deleting them leaves the workspace empty on future visits.

## Data and deployment

Task data and theme preferences stay in the browser profile where they were created. CSV export creates a local download. Deploy the contents of this folder as a static site (for example, publish this folder on Netlify). A static deployment does not provide synchronization across devices or users.

Authentication, server-side storage, collaboration, email verification, secure shared backups, and server reminders require a backend and are not implemented in this frontend-only MVP. Browser notifications and recurring schedules are also not included.

## Checks

Run `node --check app.js` to check JavaScript syntax. Then open the page and try creating a task, changing its status, searching/filtering, editing, deleting and undoing, exporting CSV, and switching theme. Drag a card between columns on the Board view.
