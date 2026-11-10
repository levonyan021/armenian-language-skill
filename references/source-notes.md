# Source notes — what this skill is built from

Origin: https://lib.armedu.am/category/79?f=&sb=146 (Ministry of Education electronic library, category "Դասագրքեր և մեթոդական ուղեցույցներ", subject filter «Հայոց լեզու»). The filter returned 13 files on 2026-11-10 (13 article pages, no further pagination).

| File | Grade | Kind | Edition | Text extraction |
|---|---|---|---|---|
| g7_textbook_b | 7 | textbook (Zangak) | 2023 | OK (Unicode) — **main source** |
| g7_textbook_a | 7 | textbook (Astghik Gratun, Meitikhanyan–Barseghyan) | 2023 | legacy font encoding, garbled |
| g7_guide | 7 | teacher guide | 2023 | OK |
| g8_textbook_a | 8 | textbook (Zangak) | 2024 | OK — **main source** |
| g8_textbook_b | 8 | textbook (Astghik Gratun) | 2024 | legacy font encoding, garbled |
| g8_guide_a | 8 | teacher guide | 2024 | scanned (no text) |
| g8_guide_b | 8 | teacher guide | 2024 | OK (not analyzed) |
| g9_textbook | 9 | textbook (Zangak) | 2025 | OK — **main source** |
| g10_textbook_a | 10 | textbook (Zangak) | 2024 | OK — **main source** |
| g10_textbook_b | 10 | textbook (Astghik Gratun) | 2024 | legacy font encoding, garbled |
| g10_guide_a | 10 | teacher guide | 2024 | scanned (no text) |
| g10_guide_b | 10 | teacher guide | 2024 | OK (not analyzed) |
| g11_textbook | 11 | textbook | 2025 | scanned (no text) |

## What was analyzed
Only the Unicode-readable Zangak textbooks (grades 7–10) were analyzed: table of contents of all four, and the theory blocks ("Գիտելիք" / "Ինչ է …") of grades 7–9, plus the readable definitions in grade 10. This is **not** a line-by-line study of every exercise.

## What was NOT analyzed (gaps)
- Grade 11 textbook (scanned images) and two scanned guides: need OCR (e.g. Tesseract with Armenian `hye` model).
- The three "Astghik Gratun" textbooks: text is in an old Armenian-ANSI font mapping (looks like `Ð²Úàò Èº¼àô` for `Հայոց լեզու`); a character-mapping table would decode them.
- Teacher guides (methodology): not mined for lesson-plan patterns or answer keys.
- Grade 10 phonetics/orthography detail rules and appendix tables (the book refers to "Հավելված 9"), which are not machine-readable here.
- Grades 1–6 and 12 are not in this category listing; they are not covered.

## Extraction caveats
`pdftotext` leaves artifacts: stray spaces inside words (`Ած ակ ան` for `Ածական`), soft hyphens (U+00AD), dot leaders in tables of contents. When quoting textbook examples, rejoin the letters and verify the word.

## Where rules are tagged *(general knowledge)*
They come from general knowledge of Eastern Armenian grammar, not from the extracted textbooks, and should be verified before being used as exam-grade authority.
