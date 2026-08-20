# Khmer Sentence Builder

A browser game for practising Khmer sentence construction. You get an English
sentence and a scrambled bank of Khmer words; drag or tap them into order and
check your answer.

Romanised Khmer only — no Khmer script.

## Play

Open the GitHub Pages link for this repo, or run it locally:

```sh
python3 -m http.server 8000
```

then visit <http://localhost:8000>.

A local server is required — browsers block `fetch` on `file://`, so opening
`index.html` by double-clicking it will not load the sentences.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The game. Self-contained: no build step, no dependencies. |
| `sentences.json` | The sentence bank. Graded into three levels. |
| `khmerwords.json` | Vocabulary lexicon, ~500 entries. |
| `khmer-worksheet.md`, `khmer-worksheets/` | Earlier printable-worksheet generator. |

## Adding sentences

Append to `sentences.json`:

```json
{
  "id": 11,
  "level": 2,
  "english": "I will go to school tomorrow.",
  "khmer": ["knyom", "nung", "dtow", "sala-rean", "sa-aik"],
  "alsoAccept": [["sa-aik", "knyom", "nung", "dtow", "sala-rean"]],
  "note": "Time words can lead the sentence or trail it."
}
```

- `khmer` is the canonical word order — one word per tile.
- `alsoAccept` lists other orders that are equally correct. Khmer fronts time
  expressions freely, so without it the game will reject valid answers.
- `note` is optional and shown only after a correct answer.
- `level`: 1 = short statements, 2 = negation/tense/questions, 3 = longer.

## Vocabulary format

```json
{ "english": "friend", "khmer": "met-peak", "variants": ["bpouk-mak"] }
```

`khmer` is always a single canonical form. `variants` holds contractions and
synonyms. A few entries carry `pattern` for discontinuous constructions such as
`min ... dtay` (negation) or `aaj ... ban`.
