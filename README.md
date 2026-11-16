# COSMOS Tool Templates (Archived)

This repository holds the Angular, React, and Svelte tool templates that
used to ship with [OpenC3 COSMOS](https://github.com/OpenC3/cosmos) in
`openc3/templates/`. They were removed from COSMOS and the
`cli generate tool_angular`, `tool_react`, and `tool_svelte` generators no
longer exist. The git history from the COSMOS repo has been kept.

| Directory       | Framework |
| --------------- | --------- |
| `tool_angular/` | Angular   |
| `tool_react/`   | React     |
| `tool_svelte/`  | Svelte    |

These templates are not maintained. COSMOS tools are written in Vue.js, and
`openc3.sh cli generate tool` creates a Vue.js tool. See the
[Custom Tools guide](https://docs.openc3.com/docs/guides/custom-tools).

COSMOS loads tools through [single-spa](https://single-spa.js.org/), so a
tool can still be written in another framework. The templates here show how
that was done, but their dependencies are out of date and the files contain
ERB tags (such as `<%= tool_name %>`) that the COSMOS generator filled in.
