# Renovate preset configuration

To use it, add in your `.github/renovate.json5`:

```json5
{
  extends: [
    // Recommended configuration:
    "github>camptocamp/gs-renovate-config-preset:base.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:preset.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:stabilization-branches.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:ci.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:pre-commit.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:python.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:python-version.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:json-schema.json5#<release>",
    "github>camptocamp/gs-renovate-config-preset:shellcheck.json5#<release>",
  ],
}
```

See also the related [Renovate documentation](https://docs.renovatebot.com/config-presets/).
