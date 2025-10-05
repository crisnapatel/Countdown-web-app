# Dual Project Time Visualization

Welcome! This repo is just a single-page tool that I use to keep an eye on long-running projects. Open `dual_project_time_visualization_clock_calendar.html` in any modern browser and you get two views you can toggle between:

* **Project Clock** – An analog-style display that shows how far you are through your project window (the big hand) alongside your current local time.
* **Project Calendar** – A month-by-month calendar that highlights elapsed days, today’s progress, and how far each date sits between your chosen start and goal.

The interface is designed to work offline and saves your inputs in `localStorage`, so you can close the tab and pick up right where you left off.

## Quick start

1. Clone or download the repo.
2. Double-click `dual_project_time_visualization_clock_calendar.html` (or serve it with any static web server if you prefer).
3. Set your **start** and **goal** dates in the Controls drawer.

That’s it—you now have a visual countdown and a calendar view for the same project window. The defaults point to a start date of “now” and a goal date of 06 Dec 2025, but feel free to change them.

## Controls & presets

* Use the **Controls** button in the top-right to open the drawer without shifting the layout.
* `Save` persists your chosen dates to `localStorage`; `Reset` clears stored values and reloads the page.
* The presets give you a one-click way to jump to the default goal or add 30 days from today.
* Keyboard shortcuts: `1` for the Project Clock, `2` for the Project Calendar, and `Esc` to close the drawer.

## How I use it (and how you might too)

For research projects (like my hydrogen storage experiments) I keep the start date at the beginning of the campaign and set the goal to the expected handover or milestone review. The day hand gives me a quick sense of overall progress, while the calendar is great for spotting empty windows for experiments, equipment maintenance, or data analysis sprints.

Feel free to adapt it for grant timelines, lab booking schedules, or personal milestones. The styling is compact enough to embed in other dashboards if you need it somewhere else.

## Customization pointers

The entire app lives in `dual_project_time_visualization_clock_calendar.html`. A few helpful anchors if you’re planning tweaks:

* All styling is inline in the `<style>` block at the top of the file—no external CSS required.
* The controls logic, clock animation, and calendar rendering are handled in the `<script>` block at the bottom.
* Local timezone detection happens during initialization, and the page re-renders responsive layouts on window resize.

If you decide to fork this for your own lab, let me know what you build with it!

Credits: GPT, Perplexity.
