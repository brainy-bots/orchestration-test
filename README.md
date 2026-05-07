# orchestration-test

Test repo for `gh-conductor`'s first end-to-end orchestration cycle.

The daemon at `brainy-bots/gh-conductor` watches this repo for events. To trigger a cycle:

1. Create an issue. Body must include a line like `**Branch**: epic/1-something`.
2. Apply the `orchestration-active` label to the issue.
3. The daemon receives the webhook, runs the orchestrator skill, and creates an epic PR.
