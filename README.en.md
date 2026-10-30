# Si tian kao yan tu · 司天考驗圖

**English documentation · [完整中文說明](README.md#完整中文說明)**

An independently collated AI transcription of Bodleian **MS.Chin.c.25**, with unresolved readings retained. This English guide translates the project documentation; it does not introduce a new data release or additional validation. The data version remains **v0.2.0**.

**No human expert review has been completed.** Prepared by Chu, Chen-Yu (曲宸宇; GitHub: [poplolioi11](https://github.com/poplolioi11); [ORCID](https://orcid.org/0009-0003-9738-6914)).

[Read the text](transcription.txt) · [Structured JSON](transcription.json) · [TEI P5 XML](transcription.tei.xml) · [Uncertain readings](uncertainties.json) · [Official manuscript images](https://digital.bodleian.ox.ac.uk/objects/d547c5a0-f642-4dbe-92f4-6766edac9943/) · [Version DOI](https://doi.org/10.5281/zenodo.23723751)

## What this edition provides

This edition adds another independent image-reading pass, comparison, and adjudication against the images for the declared text layers and full-page layouts across all 30 canvases. The scope includes titles, inscriptions, star-chart labels, explanatory verses and prognostications, two world maps, eclipse diagrams, seals, collection marks, and blank surfaces.

The files can support name indexing, source location, and further textual collation. Before formally quoting verses, prognostications, or uncertain passages, check the original images and uncertainty records. This is **not human double-proofreading, an expert-established edition, or a certification of transcription accuracy**.

## Manuscript source and scope

*Si tian kao yan tu* (《司天考驗圖》), by Wu Wei'e (吳維鍔), Qing dynasty. The source is **MS.Chin.c.25**, Bodleian Libraries, University of Oxford. The library's manuscript catalogue date of **1800–1899** is not treated as a date of composition or publication.

The **30 IIIF canvases** retain the library's original sequence; they must not be interpreted as 30 leaves. The blank surfaces are **c002, c003, c004, c028, c029, and c030**.

[Digital Bodleian images](https://digital.bodleian.ox.ac.uk/objects/d547c5a0-f642-4dbe-92f4-6766edac9943/) · [Official IIIF manifest](https://iiif.bodleian.ox.ac.uk/iiif/manifest/d547c5a0-f642-4dbe-92f4-6766edac9943.json) · [Library catalogue record](https://east-asian.bodleian.ox.ac.uk/catalog/volume_594)

Source credit: **MS.Chin.c.25. Photo: © Bodleian Libraries, University of Oxford.**

The manuscript images are **not redistributed in this package**. The applicable source rights remain [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). The preparer's own documentation and original arrangement are separately licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). These rights apply to distinct layers; see [LICENSE.md](LICENSE.md).

## Contents of v0.2.0

The edition contains **1,410 text blocks**, **311 located uncertainty records**, and **101 occurrences of `□`** in the transcription. An uncertainty record may also refer to a character that has been transcribed. A single `□` may stand for a passage of undetermined length. These counts therefore cannot be treated as counts of missing characters, error rates, or accuracy measurements.

Figures remain represented by **36 modern descriptions**. The geometry of star points, connecting lines, coastlines, and latitude–longitude grids has not been reconstructed.

Compared with the fixed v0.1.0 release, text in **335 existing blocks** changed, **20 incorrectly framed or duplicate units** were removed, and **16 source units** were added. These are block-level changes, including regrouping and corrections to recorded written forms; they are not counts of erroneous characters. See [corrections.json](corrections.json), [region-mapping.json](region-mapping.json), and [COLLATION.md](COLLATION.md) for individual changes.

| File | Purpose and limits |
| --- | --- |
| [TXT](transcription.txt) | Read the transcription directly. Navigation text and role labels in square brackets are modern additions, not manuscript text. |
| [JSON](transcription.json) | The primary dataset, preserving sources, transcribed text, roles, approximate text boxes, uncertain readings, and review status. |
| [TEI P5 XML](transcription.tei.xml) | Text agrees with the JSON block by block. `surface`/`zone`, `ab`, `figure`, and uncertainty `note` elements retain source correspondence. Consult the accompanying JSON for the complete data. |
| [Uncertain readings](uncertainties.json) | Located uncertainties and associated records. |
| [Source index](source-index.json) | Source references and regions of the official high-resolution images. |
| [Collation report](collation-report.json) | Summary of the review. |
| [Format validation](VALIDATION.json) | Recorded format-validation results. |
| [Checksums](SHA256SUMS) | Checksums for the fixed archived package. |
| [Citation metadata](CITATION.cff) | Machine-readable citation information. |

`bbox=[x,y,width,height]` uses actual pixels in the fixed working images. Text positions are **1-based Unicode code-point positions**. Boxes provide approximate locations or reading neighbourhoods and may include neighbouring characters. They are not precise character boundaries, star-point coordinates, or measurement data. Names within figures are transcribed separately by location rather than joined into invented continuous sentences.

## Review process and limitations

The independent reading pass preceded comparison of the two drafts. Differences, uncertain readings, and explicitly listed high-risk items were then adjudicated against the images. Star-official terminology and expressions in the *Bu tian ge* (《步天歌》) were used to raise questions; they do not override the manuscript's written forms.

Punctuation is not automatically supplied, variant characters are not automatically unified, place names are not normalized, and possible errors in the manuscript itself are not silently corrected. When the source does not support a unique reading, candidates and reasons are retained.

This round used Codex image workers (**requested: `gpt-6-astra`, `ultra`; the actual serving model for each request was not independently reported**) and Gemini image work through AI Coop (**reported: `gemini-3.8-flash-high`**). Programs handled deterministic comparison, encoding, hashing, and consistency checks only. There was **no human expert review, peer review, character-by-character accuracy measurement against a human reference, or complete collation against other witnesses**. See [PROVENANCE.md](PROVENANCE.md).

Separate validation covered JSON/TXT/TEI readback, page order, IDs, source hashes, text-box bounds, uncertainty locations, the official TEI Relax NG schema, and the complete CFF 1.2.0 schema. **These checks do not establish that the transcription is error-free.**

The dedicated programs, prompts, crops, and complete collaboration records are privately retained. A method for fully rerunning recognition from the original images is **not provided**.

## Citation, versions, and corrections

This version is archived on Zenodo:

- [Version DOI: 10.5281/zenodo.23723751](https://doi.org/10.5281/zenodo.23723751)
- [Concept DOI for all versions: 10.5281/zenodo.23588494](https://doi.org/10.5281/zenodo.23588494)
- [Fixed GitHub v0.2.0 release](https://github.com/poplolioi11/ms-chin-c25-sitian-kaoyantu/releases/tag/v0.2.0)

Chu, Chen-Yu（曲宸宇）. (2026). 《司天考驗圖》MS.Chin.c.25：獨立 AI 二校（保留疑字）, v0.2.0. https://doi.org/10.5281/zenodo.23723751

Research citations should additionally identify the historical author, the Bodleian manuscript, and the specific canvas or block used. The v0.1.0 initial transcription, earlier tags, files, and [earlier version DOI](https://doi.org/10.5281/zenodo.23588495) remain available. Later versions do not overwrite earlier ones.

Corrections supported by evidence from the original page are welcome through [Issues](https://github.com/poplolioi11/ms-chin-c25-sitian-kaoyantu/issues); see [CONTRIBUTING.md](CONTRIBUTING.md).

The fixed v0.2.0 tag, ZIP, and Zenodo files were prepared **before the DOI was created**. Any pending status in those files is a snapshot of that time. The main README is the current entry point after publication. `SHA256SUMS` verifies the fixed archived package; later updates to the `main` README and `CITATION.cff` are tracked separately through Git commits. The transcription and fixed package have not been overwritten.

## Short summary

An independently collated AI transcription of *Si tian kao yan tu*, attributed to Wu Wei'e, Bodleian MS.Chin.c.25. All declared text layers and page layouts across 30 canvases were reviewed, including star-chart and world-map labels, captions, prognostications, eclipse diagrams and paratext. Unresolved readings are explicitly retained. There has been no human expert review or measured character-accuracy evaluation. This is a provisional source-aligned research aid; verify quotations against the manuscript images. Geometry is not reconstructed. Source applicable rights remain CC BY-NC 4.0; original documentation and arrangement are separately CC BY 4.0. Scans and private processing materials are excluded.
