# Write & Ignite Sales Page Toolkit

An unofficial plugin for **Codex and Claude Code** that turns a real product or service brief into a sales-page outline, draft, rewrite or critique.

It combines original operational notes informed by Alex Cattoni's Write & Ignite course with Peter Yang's [no-ai-slop](https://github.com/petergyang/no-ai-slop) rules and evaluation. Anti-slop guidance applies throughout drafting and review, preserving the brand's voice and supported details.

## Install

### Codex

```sh
codex plugin marketplace add Clickt-Digital-Marketing-Inc/write-ignite
codex plugin add write-ignite@write-ignite
```

Start a new chat, select the plugin's `sales-page` skill, or ask:

> Use Write & Ignite to draft a sales page from this brief. Develop the offer, write the full page, then review it for unsupported claims and AI slop.

### Claude Code

```sh
claude plugin marketplace add Clickt-Digital-Marketing-Inc/write-ignite
claude plugin install write-ignite@write-ignite
```

Start a new session or run `/reload-plugins`, then invoke:

```text
/write-ignite:sales-page Draft a sales page from this brief: …
```

For local development:

```sh
git clone https://github.com/Clickt-Digital-Marketing-Inc/write-ignite.git
cd write-ignite
claude --plugin-dir ./plugins/write-ignite
```

The repository is a marketplace containing one plugin. Its plugin manifests are inside `plugins/write-ignite`, and both hosts use the same skill files.

## Use it

- **Offer:** turn product notes into an offer brief, feature-to-benefit mapping and material gaps.
- **Outline:** plan the reader's path from problem to solution, offer and action.
- **Draft or rewrite:** produce complete copy in the brand's voice, then review it.
- **Critique:** identify specific weaknesses and propose concrete revisions.
- **Detect slop:** name patterns, quote affected passages and suggest brief fixes without rewriting, scoring or guessing authorship.

Supply the product, audience, offer facts, proof, price and terms, desired action and any voice examples. The skill reuses available facts and asks about material gaps. It can also handle a narrow request such as a hero rewrite.

The workflow adapts to evergreen offers and service bookings. It does not invent promotions, scarcity, testimonials, guarantees, research or comparison prices to fill a template. Copy checks are reported separately from mobile, readability measurement and checkout testing.

## Sources and scope

The course-informed notes cover offer development, sales-page structure and editing. The core written resources were reviewed; videos, Q&A recordings, bonus critiques and inspiration examples were not transcribed or incorporated. See [source coverage](plugins/write-ignite/skills/sales-page/references/sources.md).

This is an independent implementation with no endorsement or affiliation claimed with Alex Cattoni, The Copy Posse or Cattoni Creative Inc. Original course worksheets, PDFs, videos, transcripts, swipe files, branding assets and official assistant prompts are not included. Direct course-resource download links are omitted from the public package.

The bundled no-ai-slop files are preserved at commit `000650b156983f5159695b441477f4e63b25dc85`, with their MIT license. See [third-party notices](THIRD_PARTY_NOTICES.md). The upstream license does not license the course content or automatically apply to the entire repository.

## Validation

Both plugin manifests and the shared skill have been validated. The [validation record](VALIDATION.md) includes bounded writing and detection tests, their limitations, and fictional example outputs.

To validate the Claude manifests locally:

```sh
claude plugin validate --strict .
claude plugin validate --strict ./plugins/write-ignite
```

No API keys, server, executable hooks or paid API are required by this plugin. Normal host usage limits apply. The bundled references work offline; live research and page checks depend on tools available in the host.
