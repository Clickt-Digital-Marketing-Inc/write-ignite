# Validation record

Build: `0.1.0`. Original behavioral checks: 2026-09-27. These results describe the original local build; public packaging is validated separately below.

## Public packaging checks

Validated on 2026-09-27 after preparing the public export:

- Codex plugin manifest and shared skill validators passed.
- Codex marketplace name and entry target validated.
- Claude Code strict validation passed for both the marketplace and plugin manifests.
- Both catalogs route to `plugins/write-ignite`; the manifests agree on name and version. There is one discoverable skill.
- All documentation-relative links resolve. The `/start` URLs in the fictional draft are illustrative CTA destinations.
- Public-content inspection found no personal filesystem paths, direct course-download/share URLs, credentials or original course assets.
- All four bundled no-ai-slop files match the original local package byte-for-byte, including the upstream license and provenance record.
- A separate read-only review confirmed the public-content cleanup, catalog routing, relative links and upstream-file preservation.

The public export has not replaced the original personal installations. This check validates the exported package; it does not claim marketplace-install execution in a fresh user account.

## Static and host checks

| Check | Result |
|---|---|
| Codex plugin-creator manifest validator | Passed |
| Codex skill-creator validator | Passed |
| Claude Code `plugin validate --strict` | Passed |
| Claude Code local `--plugin-dir` discovery | Listed as `write-ignite@inline`, version 0.1.0, enabled |
| Relative Markdown references | All resolved |
| Bundled no-ai-slop rules, evaluation and license | Byte-identical to fetched upstream files at `000650b156983f5159695b441477f4e63b25dc85` |

The Codex validators required PyYAML, which was installed only in a temporary validation directory. This is a build-time check dependency, not a plugin runtime dependency. The final workflow is Markdown and JSON only; it has no executable hooks, MCP server, background process or external model call.

## Behavioral checks

Two independent agents executed realistic requests using the skill and its references. The parent reviewed their actual outputs. These are bounded smoke tests, not conversion tests or proof of identical output in every model.

- **Complete draft:** A fictional invoice-reminder product with a £19 monthly price, seven-day no-card trial, approval-before-sending workflow and British English voice. The agent delivered copy and a review without stopping at an outline. It preserved the stated terms, omitted invented testimonials, discounts, scarcity and guarantees, and flagged unknown trial-to-paid behaviour. The first draft repeated the mechanism and included interpretive reader guidance. Short-page instructions were tightened; the revised [example](validation/draft-example.md) removed those issues. The final copy was 302 words versus the approximate 450-word target, with the shortfall disclosed instead of padding the facts.
- **Detection only:** An intentionally formulaic hero for a brand named Streamline. The agent produced six named findings with quoted text and brief fixes, preserved the brand name, and did not rewrite, score the text or infer AI authorship. See the [result](validation/detection-example.md).

The examples are fictional test outputs. They are not course examples, customer evidence or copy for a real product.

## Scope of confidence

Manifest compatibility, file integrity, skill discovery and the tested writing behaviours are supported by these checks. No generated sales copy was deployed to a live sales page. No mobile layout, checkout, spoken read-through or conversion outcome was tested. Core course resources were reviewed; videos and bonuses remain outside this build's source coverage.
