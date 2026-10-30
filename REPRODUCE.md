# How this repository was made (United States (Kansas))

This file is written by the build on 2026-10-30, the day the source data was retrieved.

## Sources

| Source | Address | Retrieved | Licence |
| --- | --- | --- | --- |
| Kansas Office of Revisor of Statutes | <https://ksrevisor.gov/ksa.html> | 2026-10-30 | Statute text is not copyrightable (Georgia v. Public.Resource.Org, 2020). Case annotations, history lines and prior-law notes omitted. |

Every word of law in this repository comes from these sources. Lexifina reads them and records each act's dated versions, and the laws that made each change, in one corpus file. This repository is built from that file.

## What is in it

| Act | Title | Versions | Span |
| --- | --- | ---: | --- |
| `constitution` | Constitution of the State of Kansas | 1 | 2025-07-01 to 2025-07-01 |
| `chapter-21-criminal-code` | K.S.A. Chapter 21, Articles 51 to 99: Kansas Criminal Code and related crimes provisions | 1 | 2025-07-01 to 2025-07-01 |
| `chapter-17-corporations` | K.S.A. Chapter 17, Articles 60 to 72: Kansas General Corporation Code and related provisions | 1 | 2025-07-01 to 2025-07-01 |

The build made 3 commits:

| Commits | Kind |
| ---: | --- |
| 3 | first version of an act |
| 0 | one law on its in-force day |
| 0 | changes no amendment note explains, credited to the publisher |

Other counts:
- 0 commits on the branch `future`: laws not yet in force on 2026-10-30.
- 0 commits dated 1 January 1970: in force before 1970, with the real day in their `In-force` trailer.
- 1 laws in the record.
- 3 tags.

## Dates

Each commit is dated at noon (America/Chicago) on the day the change took effect. The other dates, enacted and published, are trailers.

When a law gives no date of its own, the default rule applies: The Revisor publishes only the current text, stated to include the 2025 session (the Constitution page says "as of July 1, 2025"); that is the only version and is dated 2025-07-01. https://ksrevisor.gov/ksa.html

## How the history is built

`tools/build.py` turns the corpus into this history in one pass: one commit per law, on the day it took effect. The same corpus always gives the same commit hashes. `tools/check_repo.py` reads every version back from git and compares it with the corpus. `tools/on.py` shows the law as it stood on any date. The corpus format is described in `tools/SCHEMA.md`.

- Corpus: sha256 `94cb96aa5aedb9f4662697d50e039a4664ea4f971b5b9478f3e197db5cf1f2fd` (1556398 bytes).
- Builder blob hashes (`git hash-object`): `build.py` `a4faa25af85facb64b956b372f6b528aafdd7ec1`, `check.py` `3e59cb6f05eccb94a9ec14431a7f6781221e83ef`, `on.py` `644a6c0857fbcc72562032b58d57aa113fee0641`.
- Python 3.12.10; git version 2.46.0.windows.1.

## Checks

Not yet run for this build.

No second build of this corpus has been compared yet.

## Decisions made by hand

- Only the current text is online, so each act has one version, the oldest version available, dated 2025-07-01 from the Revisor's statement that it includes enactments as of July 1, 2025.
- Scope: the State Constitution, K.S.A. chapter 21 articles 51 to 99 (the Kansas Criminal Code of 2011 and later crimes articles) and chapter 17 articles 60 to 72 (corporation code). Other chapters are not included.
- Constitution sections eliminated by revision (heading only, no text) are omitted; case annotations, history lines and prior-law lines are dropped.

## What AI did and did not do

The scripts that read the sources and build this repository were written by Claude Code running Claude Opus 5.5 (`claude-opus-5-5`) under Lexifina's direction.

No model wrote, translated or corrected legal text. No model runs at build time. Every word of law in this repository comes from the official sources above.

The commit messages are written by `build.py` from the source data.

Model use at data-build time:
- none
