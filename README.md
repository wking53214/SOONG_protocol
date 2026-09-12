# SOONG Protocol — governing constraint

A timestamped, hash-sealed reconstruction of what the SOONG protocol's governing constraint was, and
how it was arrived at, derived only from archived conversation records.

**[`SOONG_GOVERNING_CONSTRAINT_DERIVATION.md`](SOONG_GOVERNING_CONSTRAINT_DERIVATION.md)** — Rev 04,
sealed `88e2d71278472f2a4bac697ad26e9ffe4fbcfa5ee8977c2ede8a48de3f639d9b`

## The finding

The governing constraint was the **Alpha-Omega Pillar**: a first-position gate requiring every output
to originate in Mark 12:30-31 and terminate in John 13:34, with a failing query **aborted rather than
filtered**.

Two properties carry the weight:

- **It was a position, not just a rule.** The moral anchor already existed at slot 2, already labelled
  "the Non-Negotiable Variable," and did nothing. It became governing when it was moved to slot 01,
  ahead of the adversarial logic.
- **Its failure mode was abort.** Not softened, not corrected.

It was reached through an engineering argument rather than a devotional one — a constraint applied
last is a filter an optimizer routes around; a constraint applied first is a precondition it cannot.
The schema was reordered at `2026-03-25T18:55:45Z`, and the rename from SOONG to **Submission
Protocol** followed **44 seconds later**, as a consequence of the reorder rather than as a separate
event.

Elapsed from the first SOONG record to the final governing constraint: **2 days, 19 hours**.

It was never revoked. By `2026-07-06` it had been demoted from root node to the third of four modules,
described as scrubbing text fields — **a gate that aborted a query had become a gate that cleans a
string** — as a by-product of a documented campaign to strip theological nomenclature from the
architecture. No decision was ever recorded against it.

## How to read it

| Section | Contents |
|---|---|
| 0 | Scope, exclusions, evidentiary rules, source limitations |
| 1 | The answer |
| 2 | The derivation — 16 dated steps, verbatim quotes, source indices |
| 3 | Summary table |
| 4 | Where the record contradicts itself, and the forward trace (4.5) |
| 5 | Ten gaps the archive does not close |
| 6 | Method |
| 7 | Integrity block |

## Verifying the seal

```
sed '/^SHA-256 (body): /,$d' SOONG_GOVERNING_CONSTRAINT_DERIVATION.md | sha256sum
```

The hash covers the document from its first character through the line preceding the `SHA-256` marker.

## Evidence

The artifact cites primary records by source index; the underlying corpus lives in the archive
repositories (`gemini_extraction`, `gemini_history`, `chatgpt_history`, `claude_history`,
`copilot_history`). SHA-256 hashes for every primary evidence file are recorded in §0.3, so quotations
can be checked against the exact bytes they were drawn from.

## Standards applied

- **Record-derived findings and author attestation are kept separate.** Attestation appears once
  (§4.2.4), is labelled, and only corroborates a finding that stands without it.
- **Gaps are stated as gaps.** Where the archive cannot decide a question, §5 says so rather than
  filling it.
- **Corrections are logged, not silently absorbed.** Two of the four revisions correct earlier work in
  this same document — a provenance error in Rev 02, a mischaracterisation in Rev 03, and a
  search-coverage hole in Rev 04. The revision log at the top records each.
- Material concerning family, marriage, and private spiritual practice was excluded at the requester's
  instruction; every exclusion is enumerated in §0.1.
