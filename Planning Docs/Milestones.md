# Milestone Chart - Obsidian TickTick Task Creator

## Overview

Obsidian TickTick Task Creator is an Obsidian plugin designed to create TickTick tasks based on note properties. This plugin is intended to support a workflow in which TickTick is used as the primary task management tool (used to schedule, track, and prioritize), while Obsidian is used to manage detailed project plans and supporting information.

## Milestones

| Milestones                                          | Deliverables                                                                                                                                                                                                                                                                                         | Target Date | Dependencies                                                  | Status   |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ------------------------------------------------------------- | -------- |
| Basic task creation                                 | TickTick Task Creator can create a task in TickTick based on the title of an Obsidian note. Task creation is controlled on a per-note basis.<br><br>Authorization flow for initial setup                                                                                                             | 2025-07-11  | None                                                          | Planned  |
| Task ↔ Note links                                   | Insert a link to the Obsidian note in the description of a created TickTick task.<br><br>Add a link to a created TickTick task to the properties of the associated Obsidian note.                                                                                                                    | 2025-07-18  | Basic task creation                                           | Planned  |
| Set task attributes from note properties            | Set the due date, list, priority, and tags of a created TickTick task based on YAML properties of the Obsidian note.<br><br>Create plugin settings to configure associations between frontmatter keys and task attributes.                                                                           | 2025-08-08  | Basic task creation                                           | Planned  |
| Set task attributes using TickTick Quick Add syntax | Set task attributes using TickTick Quick Add syntax in Obsidian note properties. For instance, `ticktick-attrs: !High ~Home`  creates a task with High priority in the user's Home list.<br><br>The plugin is responsible for parsing this input, as it isn't supported directly by the TickTick API. | 2025-08-22  | Basic task creation                                           | Planned  |
| Sync edits to note properties to TickTick           | For notes associated with tasks, watch for changes to note properties, and update associated tasks accordingly.<br><br>                                                                                                                                                                              | 2025-09-05  | Set task attributes from note properties<br>Task ↔ Note links | Planned  |
| Beta Testing                                        | User-facing documentation<br><br>Security review<br><br>Call for beta testers                                                                                                                                                                                                                        | 2025-09-12  | All previous milestones                                       | Planned  |
| Release                                             | Request review for inclusion in Obsidian Community Plugins<br><br>                                                                                                                                                                                                                                   | 2025-09-26  | Beta testing complete; issues resolved                        | Planned  |

```mermaid
gantt
    title Obsidian TickTick Task Creator
    dateformat YYYY-MM-DD
    axisFormat %b %e

    section Milestones
        Basic task creation   :a, 2025-07-08, 7d
        Obsidian ↔ Note links :b, after a, 7d
        Set task attributes from note properties :c, after b, 14d
        Quick Add syntax :d, after c,14d
        Sync edits :e, after d, 14d
        Beta testing :f, after e, 14d
        Release :after f, 14d
```
