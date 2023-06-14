# Graasp Renovate defaults

This repository provide Renovate defaults [config presets](https://docs.renovatebot.com/config-presets/) and can be extended by any Graasp project.

This is an overview of the defaults presets:

* Group some dependencies using multiple packages together (sentry, eslint...)
* Automerge sementic patch update and linters
* Automerge outside of office hours (avoid saturating the pipeline)

To get the presets from `default.json` just extend it in your `renovate.json`:

```json
"extends": ["github>graasp/renovate-config"],
```

Or take a named preset `<name>.json`from this repo:

```json
"extends": ["github>graasp/renovate-config:<name>"],
```

If you use the same Renovate config in multiple repositories, consider adding it to this repository's `default.json` or create your own named preset if it's used by multiple repositories but not all of them.