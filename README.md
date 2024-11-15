# Renovate preset configuration

To use it, add in your `.github/renovate.json5`:

```json5
{
  extends: [
    "github>camptocamp/gs-renovate-config-preset#<release>:recommended.json5",
    // Recommended configuration includes:
    "github>camptocamp/gs-renovate-config-preset#<release>:base.json5",
    "github>camptocamp/gs-renovate-config-preset#<release>:stabilization-branches.json5",
    "github>camptocamp/gs-renovate-config-preset#<release>:ci.json5",
    "github>camptocamp/gs-renovate-config-preset#<release>:pre-commit.json5",
    "github>camptocamp/gs-renovate-config-preset#<release>:python-version.json5",
    "github>camptocamp/gs-renovate-config-preset#<release>:json-schema.json5",
    "github>camptocamp/gs-renovate-config-preset#<release>:shellcheck.json5",
  ],
}
```
