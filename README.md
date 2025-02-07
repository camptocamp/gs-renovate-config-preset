# Renovate preset configuration

To use it, add in your `.github/renovate.json5`:

```json5
{
  extends: [
    // Recommended configuration:
    'github>camptocamp/gs-renovate-config-preset:base.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:preset.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:stabilization-branches.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:ci.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:pre-commit.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:python.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:security.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:docker.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:json-schema.json5#<release>',
    'github>camptocamp/gs-renovate-config-preset:shellcheck.json5#<release>',
  ],
}
```

See also the related [Renovate documentation](https://docs.renovatebot.com/config-presets/).

## Available Presets

- `base.json5`: Base configurations and dependency groups.
- `preset.json5`: Get the preset dependencies.
- `stabilization-branches.json5`: Configure version branches in format `x.y`.
- `ci.json5`: Groups and auto-merge CI dependency updates.
- `pre-commit.json5`: Get pre-commit hook dependencies.
- `python.json5`: Handles Python version management.
- `security.json5`: Ensures immediately update security related and critical packages (including `pytz`).
- `docker.json5`: Some image version parsing for Docker images.
- `own.json5`: Ensures immediately updates for internal packages.
- `json-schema.json5`: Get JSON Schema references in YAML files.
- `shellcheck.json5`: Provides correct version parsing for ShellCheck.
