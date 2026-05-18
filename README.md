# amlmarketplaces/hubspot

Claude Code marketplace federating all `@amlplugins/hubspot-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-hubspot": {
      "source": { "source": "github", "repo": "amlmarketplaces/hubspot" }
    }
  },
  "enabledPlugins": {
      "hubspot-automation-workflows@aml-hubspot": true,
      "hubspot-cms-pages@aml-hubspot": true,
      "hubspot-conversations@aml-hubspot": true,
      "hubspot-crm-companies@aml-hubspot": true,
      "hubspot-crm-contacts@aml-hubspot": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/hubspot`, cached under `~/.claude/plugins/cache/aml-hubspot/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (9 total)

- `hubspot-automation-workflows` — [@amlplugins/hubspot-automation-workflows](https://github.com/amlplugins/hubspot-automation-workflows)
- `hubspot-cms-pages` — [@amlplugins/hubspot-cms-pages](https://github.com/amlplugins/hubspot-cms-pages)
- `hubspot-conversations` — [@amlplugins/hubspot-conversations](https://github.com/amlplugins/hubspot-conversations)
- `hubspot-crm-companies` — [@amlplugins/hubspot-crm-companies](https://github.com/amlplugins/hubspot-crm-companies)
- `hubspot-crm-contacts` — [@amlplugins/hubspot-crm-contacts](https://github.com/amlplugins/hubspot-crm-contacts)
- `hubspot-crm-deals` — [@amlplugins/hubspot-crm-deals](https://github.com/amlplugins/hubspot-crm-deals)
- `hubspot-crm-tickets` — [@amlplugins/hubspot-crm-tickets](https://github.com/amlplugins/hubspot-crm-tickets)
- `hubspot-marketing-emails` — [@amlplugins/hubspot-marketing-emails](https://github.com/amlplugins/hubspot-marketing-emails)
- `hubspot-marketing-forms` — [@amlplugins/hubspot-marketing-forms](https://github.com/amlplugins/hubspot-marketing-forms)

## Related

- npm packages: `@amlplugins/hubspot-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
