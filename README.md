# TickTick Task Creator for Obsidian

> [!NOTE]
> This plugin is in an early planning phase.
> I expect to begin development sometime this summer. First release may be in early fall.

TickTick Task Creator will allow you to create tasks in [TickTick](https://ticktick.com/) based on your [Obsidian](https://obsidian.md/) notes.

This plugin assumes that you rely on TickTick for task management (reminders, due dates, priorities, etc.), and use Obsidian to manage supporting information.

## Features

- Create TickTick tasks that link to your Obsidian notes, and add a link to the created task in note properties.
- Control TickTick task attributes based on note properties
  - Configure associations between task attributes and frontmatter properties in plugin settings
  - Set attributes using TickTick Quick Add syntax within Obsidian
- Update a task associated with a note when note properties are edited

> [!Note]
> The TickTick API currently does not support reading or editing tags.

## Scope

I'm creating this plugin primarily for my own use. At present, I only plan to implement simple features that I find essential to my own workflow. Bidirectional or TickTick → Obsidian sync is not currently on the roadmap.

Once I've released an MVP, I'd be happy to consider PRs and feature requests.

## Other TickTick Plugins

If you're looking for a way to manage your TickTick tasks within Obsidian, take a look at [TickTickSync](https://github.com/thesamim/TickTickSync), which is designed for compatibility with the [Tasks Plugin](https://github.com/obsidian-tasks-group/obsidian-tasks).
