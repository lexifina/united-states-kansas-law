# Kansas: law history in git

Part of [lexifina/global-law](https://github.com/lexifina/global-law), one git history for every country's law: this is the law of Kansas, United States, which global-law reads at `united-states/kansas/acts/`.

The statute law of Kansas as a git repository: one file per section, committed with the official publisher named as author. It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law).

**What is in it now (a first build, not complete)**

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `constitution/` | Constitution of the State of Kansas | 1 | Current text (oldest version available) |
| `chapter-21-criminal-code/` | K.S.A. chapter 21, articles 51 to 99: Kansas Criminal Code and later crimes articles | 1 | Current text (oldest version available) |
| `chapter-17-corporations/` | K.S.A. chapter 17, articles 60 to 72: Kansas General Corporation Code and related provisions | 1 | Current text (oldest version available) |

Nothing else of Kansas's law is in it yet.

## Where the text comes from

[Kansas Office of Revisor of Statutes](https://ksrevisor.gov/ksa.html). The Revisor's pages state that they include amendments enacted in the 2025 legislative session. Only statute and constitution text is taken; case annotations, history lines and prior-law notes are left out.

## Dates

Each act has one version, dated 1 July 2025: the Revisor's Constitution page says it includes everything enacted as of July 1, 2025, and the statute pages say the 2025 session.

## What it does not show

- The Revisor publishes only the current text, so there is no history yet.
- Only the Constitution, K.S.A. chapter 21 articles 51 to 99 and chapter 17 articles 60 to 72 are included.
- Constitution sections that were eliminated by revision (heading only) are omitted.

## How it is checked

- Every unit is read back from git on its day and compared with the corpus (`tools/check_repo.py`; results in `REPRODUCE.md`).
- Each source file is identified by its sha256, in `data/versions.json`.

## What "author" means

Each commit is authored by the publisher (Kansas Office of Revisor of Statutes) because this first build holds one version of each act, the oldest version available. The committer is always Lexifina.
