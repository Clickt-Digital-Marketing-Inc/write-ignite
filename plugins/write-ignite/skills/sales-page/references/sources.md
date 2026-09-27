# Sources and coverage

The course resources were reviewed on 2026-09-27 through authorized course access. Public references point to the course landing page; direct resource-download links are omitted. This plugin contains original operational notes, not copies of the videos, worksheets, PDF, example pages or official assistant instructions.

## Sources used in the workflow

| Source | What was read | Where applied |
|---|---|---|
| [Write & Ignite member course](https://academy.alexcattoni.com/products/write-ignite) | Curriculum and the three training lesson pages | Offer → structure → writing/editing workflow |
| [Lesson 1: 10 Persuasion Principles](https://academy.alexcattoni.com/products/write-ignite) | Full worksheet text, fetched from its course link | [Offer notes](offer.md) |
| [Lesson 2: 16-Step Sales Page Formula](https://academy.alexcattoni.com/products/write-ignite) | Full worksheet text, fetched from its course link | [Page structure](structure.md) |
| [Conversion-Ready Sales Page Checklist](https://academy.alexcattoni.com/products/write-ignite) | Text extracted from all 8 PDF pages, including 11 editing passes | [Editing notes](editing.md) |

Course source: Alex Cattoni / The Copy Posse; course materials identify Cattoni Creative Inc. as the rights holder. Source access does not imply endorsement of this plugin or permission to redistribute the source materials. This repository contains an independently written workflow and grants no license to the course content.

## Course inventory and limits

| Course item | Inspection status |
|---|---|
| [Welcome](https://academy.alexcattoni.com/products/write-ignite) | Listed in curriculum; video not reviewed |
| [Lesson 1: How To Craft An Offer They Crave](https://academy.alexcattoni.com/products/write-ignite) | Lesson page + linked worksheet reviewed; 30:53 video not watched/transcribed |
| [Lesson 1 Q&A](https://academy.alexcattoni.com/products/write-ignite) | Page reviewed; 1:04:44 video not watched/transcribed; no additional worksheet link on page |
| [Lesson 2: Million-Dollar Sales Page Formula](https://academy.alexcattoni.com/products/write-ignite) | Lesson page + linked worksheet reviewed; 28:58 video not watched/transcribed |
| [Lesson 2 Q&A](https://academy.alexcattoni.com/products/write-ignite) | Listed in curriculum; video not reviewed |
| [Lesson 3: Bring Your Sales Page To Life](https://academy.alexcattoni.com/products/write-ignite) | Lesson page + linked checklist reviewed; 30:54 video not watched/transcribed |
| [Lesson 3 Q&A](https://academy.alexcattoni.com/products/write-ignite) | Listed in curriculum; video not reviewed |
| [Bonus: Sales Page Copy Critique](https://academy.alexcattoni.com/products/write-ignite) | Listed in curriculum; critiques not reviewed |
| [Bonus: AI Sales Page Builder Assistant](https://academy.alexcattoni.com/products/write-ignite) | Listed in curriculum and linked from Lesson 2; assistant not invoked or reverse engineered |
| [Bonus: Sales Page Inspo File](https://academy.alexcattoni.com/products/write-ignite) | Listed in curriculum and linked from Lesson 2; example pages not reviewed or bundled |

The source inventory covers all 10 curriculum items. The implemented method is grounded in the three core written resources, not a complete video/Q&A transcription. Do not attribute additional anecdotes, exceptions, case studies or performance results to the course without reading the relevant source.

## Adaptations made for agent use

Peter Yang's [no-ai-slop repository](https://github.com/petergyang/no-ai-slop) is an additional foundation explicitly requested by the user. Its complete skill rules and evaluation were read at commit `000650b156983f5159695b441477f4e63b25dc85` on 2026-09-27. The two Markdown files and MIT license are bundled under `no-ai-slop/`; [UPSTREAM.json](no-ai-slop/UPSTREAM.json) records their original paths. [Anti-slop integration](anti-slop.md) explains the local adaptations. The MIT license covers those upstream files, not the course content or the whole plugin.

- One workflow with offer, outline, draft and review modes; no dependency on the official GPT.
- A source/status record for product claims, assumptions and missing facts.
- Permission to mark commercial sections not applicable when the business has no promotion, deadline, bonus or guarantee.
- Adaptation to service bookings, product purchases, short pages and different brand voices.
- Separate claims about copy review from live layout, readability measurement and checkout testing.
- Mandatory no-ai-slop rules during generation and editing, with the original evaluation and explicit resolution of style conflicts.

These are implementation decisions for the plugin. They should not be presented as verbatim course instructions or as statements made in unreviewed videos.
