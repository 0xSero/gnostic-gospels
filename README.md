# The Gnostic Gospels — a reading edition

Eleven texts from the Nag Hammadi library and the related codices, each as its own
small PDF, in the order they are best read. One text per file, one continuous text per
page, no apparatus to wade through first.

Typeset at **100 × 178 mm** — a phone-shaped page — so it reads at fit-width in any PDF
viewer on an iPhone, iPad, or Android tablet, one-handed, without pinch-zooming.

## Read it

| Where | What |
|---|---|
| [**Wiki**](../../wiki) | The full text of every gospel, readable in a browser. Start at [Home](../../wiki). |
| [`pdfs/`](pdfs) | The same texts as PDFs, formatted for a phone. |
| [Google Drive](https://drive.google.com/drive/folders/1Cusfvp3INiyFQ0T8PWGj3MWNQ3Uv9Vgz) | Mirror of the PDFs, same order. |

Print order is the reading order: open `00-Start-Here.pdf` first.

## Reading order

| # | Text | Pages | Translator | Why it sits here |
|---|---|---|---|---|
| 00 | [Start Here](pdfs/00-Start-Here.pdf) | 5 | — | Orientation and the order, one page. |
| 01 | [Gospel of Thomas](pdfs/01-Gospel-of-Thomas.pdf) | 30 | Thomas O. Lambdin | 114 sayings, no narrative, no framework needed. The only one that stands alone. |
| 02 | [Gospel of Mary](pdfs/02-Gospel-of-Mary.pdf) | 10 | Mark M. Mattison | Short. Introduces the genre's core moves: secret teaching, the disciple who understood, the fight over her authority. |
| 03 | [Gospel of Truth](pdfs/03-Gospel-of-Truth.pdf) | 29 | Harold W. Attridge & George W. MacRae | A sermon, not a gospel. States the theology plainly: ignorance as the root problem, error without a cause. |
| 04 | [Apocryphon of John](pdfs/04-Apocryphon-of-John.pdf) | 45 | Michael Waldstein & Frederik Wisse | The backbone of the whole system: emanations, Sophia's fall, the demiurge, the spark in you. Everything after this is legible. |
| 05 | [Gospel of Philip](pdfs/05-Gospel-of-Philip.pdf) | 45 | Wesley W. Isenberg | Aphoristic and sacramental. Dense — read it after the myth is in place, not before. |
| 06 | [Gospel of Judas](pdfs/06-Gospel-of-Judas.pdf) | 22 | Mark M. Mattison | A deliberate reversal of the standard myth. Only lands once you know what it is inverting. |
| 07 | [Hypostasis of the Archons](pdfs/07-Hypostasis-of-the-Archons.pdf) | 19 | Bentley Layton | The same myth as Apocryphon of John, told shorter and sharper. |
| 08 | [On the Origin of the World](pdfs/08-On-the-Origin-of-the-World.pdf) | 42 | Hans-Gebhard Bethge & Bentley Layton | The long version of that myth, with the cosmogony filled in. |
| 09 | [Thunder, Perfect Mind](pdfs/09-Thunder-Perfect-Mind.pdf) | 13 | George W. MacRae | Not a gospel at all — a revelation poem of "I am" paradoxes. Read for its own sake. |
| 10 | [Dialogue of the Savior](pdfs/10-Dialogue-of-the-Savior.pdf) | 22 | Stephen Emmel | A fragmentary dialogue gospel; useful as a control on how much of this genre is questions and answers. |
| 11 | [Gospel of the Egyptians](pdfs/11-Gospel-of-the-Egyptians.pdf) | 28 | Alexander Böhlig & Frederik Wisse | The Sethian *Holy Book of the Great Invisible Spirit* (NHC III,2 / IV,2) — the ritual-liturgical edge of the same tradition. |

Two branches through the set:

- **Want the sayings?** Thomas, then stop. You have the wisdom material.
- **Want the system?** Start at Apocryphon of John, then work back to Thomas.

## What these are not

They are not a canon, and there was never one movement that owned them. This is a
library of competing texts written across roughly the 2nd–4th centuries, by people who
disagreed with each other and with the emerging orthodox church. "Gnostic" itself is a
contested category — a useful label that flattens real differences. Read them as
arguments with one another, not as chapters of one book.

## Provenance

Every PDF names its translator and source URL on its colophon page. Machine-readable
detail is in [`MANIFEST.json`](MANIFEST.json) — order, translator, source, pages, bytes,
SHA-256.

Two texts are explicitly public domain (Mattison's Mary and Judas). The rest are
twentieth-century scholarly translations — Lambdin, Isenberg, Attridge & MacRae,
Layton, Bethge & Layton, Waldstein & Wisse, Böhlig & Wisse, Emmel, MacRae — published
openly on [Early Christian Writings](https://earlychristianwritings.com) and
[gnosis.org](https://gnosis.org), which carry the Coptic Gnostic Library Project's
copyright assertion. The translation text is theirs; the typesetting, introductions,
reading order and navigation here are not theirs. Attribution travels with every file
so you can check anything against its source.

Three honest caveats:

- **Gospel of the Egyptians** is NHC III,2 / IV,2, the *Holy Book of the Great Invisible
  Spirit*. NHC VI,3 is *Authoritative Teaching* — a different text, often mis-cited.
- **Gospel of Philip** is numbered 1–100 here (Isenberg's paragraph units). The 127-saying
  division used in some editions splits the same text more finely, so external
  cross-references will not line up.
- **Gospel of Mary** is missing manuscript pages 1–6 and 11–14; **Gospel of Judas** has
  holes throughout. Both are marked where they fall.

## Rebuilding

The build is reproducible from local source HTML: `extract.py` (HTML → JSON) →
`make.sh` (Typst → PDF) → `verify.py` (magic bytes, page box, terminal markers). The
PDFs here were compiled with Typst; page size, margins, and measure are set in the
Typst source, so the phone layout is a parameter, not a redraw.
