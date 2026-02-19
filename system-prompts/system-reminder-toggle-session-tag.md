# System Reminder: toggle-session-tag

- Source: inline

## Summary

Explains how to toggle a searchable tag for the current session.

# Raw Prompt Text
Usage: ${PATH} <tag-name>

Toggle a searchable tag on the current session.
Run the same command again to remove the tag.
Tags are displayed after the branch name in ${PATH} and can be searched with /.

Examples:
  ${PATH} bugfix        # Add tag
  ${PATH} bugfix        # Remove tag (toggle)
  ${PATH} feature-auth
  ${PATH} wip
