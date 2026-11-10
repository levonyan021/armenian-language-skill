---
name: armenian-language
description: Armenian language (հայոց լեզու) grammar, orthography, vocabulary and writing guidance based on the official Republic of Armenia school textbooks (grades 7–10, Zangak edition 2023–2025, approved by the Ministry of Education). Use whenever the task involves writing, correcting, explaining, grading or analyzing Modern Eastern Armenian text; answering grammar questions (parts of speech, cases, verb tenses, sentence structure, punctuation, spelling); making Armenian exercises, tests or lesson plans; or translating into Armenian where grammatical correctness matters. Trigger on Armenian script input or words like հայոց լեզու, քերականություն, ուղղագրություն, հոլով, բայ, նախադասություն, կետադրություն.
---

# Armenian language (Modern Eastern Armenian, school-curriculum norm)

This skill encodes how the Armenian national school curriculum describes the language, so answers match what teachers, students and exam-setters in Armenia expect. The terminology below is the **current textbook terminology**, which differs from older grammars in several places (see "Gotchas").

## How to work

1. **Reply in Armenian** when the user writes in Armenian. Keep grammar explanations in the textbook terminology from this skill.
2. **Identify the task type**, then load the matching reference file (do not load all of them):
   - Parts of speech, cases, verb forms → `references/morphology.md`
   - Sentence structure, sentence members, complex sentences, quoted speech, punctuation → `references/syntax.md`
   - Spelling, sound changes, vocabulary (synonyms, homonyms, word layers), word formation, history of the language → `references/orthography-lexicon.md`
   - Essays, dialogue, speeches, business documents (դիմում, ինքնակենսագրություն, բացատրագիր) → `references/text-and-genres.md`
   - Which grade teaches what / building exercises or lesson plans → `references/curriculum-map.md`
   - What was actually parsed, what was not, extraction caveats → `references/source-notes.md`
3. **When correcting text**, give the corrected version, then a short list of each error with the rule name in textbook terms. Do not silently rewrite style the user did not ask to change.
4. **When explaining a rule**, give the rule, 2–3 examples, and the common exception. Use the textbook's own example words when known.
5. **If unsure** of a rule (especially fine orthography, rare forms) say so and mark it as unverified instead of inventing a rule. Rules tagged *(general knowledge)* in the references are not taken from the parsed textbooks.

## Core facts (always keep in mind)

- Norm: **Eastern Armenian**, **classical (Mashtotsian) orthography** as used in Armenia. Do not mix in Western Armenian forms unless asked.
- **10 parts of speech** (խոսքի մասեր): գոյական, ածական, թվական, բայ, մակբայ, դերանուն, կապ, շաղկապ, վերաբերական, ձայնարկություն.
- **5 cases (հոլովներ)** in the school norm: ուղղական, սեռական-տրական, բացառական, գործիական, ներգոյական. Genitive and dative are ONE case (սեռական-տրական). Do not teach 7 cases to a student of the current curriculum; mention the traditional 7-case view only as a side note.
- **8 declension types** (հոլովման տիպեր), named after the genitive-dative marker: external (արտաքին) -ի, -ու, -վա, -ան, -ոջ, -ց; internal (ներքին) -ա, -ո.
- **Definiteness**: անորոշ (no article) vs որոշյալ (-ը / -ն). Pronominal articles (հոդեր): -ս (1st), -դ (2nd), -ն/-ը (3rd/determining).
- **Verb**: 5 moods, 14 tense-forms, 3 persons × 2 numbers, 3 voices; 4 non-finite forms (դերբայներ).
- **Sentence analysis** follows the school scheme: ենթակա, ստորոգյալ, then secondary members (որոշիչ, հատկացուցիչ, բացահայտիչ, խնդիր, պարագա). Sentence diagrams (գծապատկեր) are part of the curriculum.
- **Armenian punctuation**: ։ (վերջակետ), ՝ (բութ), , (ստորակետ), · (միջակետ), ՞ (հարցական, placed over the stressed vowel: ինչո՞ւ), ՜ (բացականչական: ա՜խ), ՛ (շեշտ: մի՛ գնա), «…» quotes, — dash for dialogue. Typing `:` instead of `։` is common but `։` is correct.

## Gotchas (where the current curriculum differs from older or Western-influenced habits)

- **Cases**: 5, not 7. Questions: ուղղական ո՞վ/ի՞նչ; սեռական-տրական ո՞ւմ/ինչի՞(ն); բացառական ումի՞ց/ինչի՞ց; գործիական ումո՞վ/ինչո՞վ; ներգոյական ինչո՞ւմ.
- **Nominative is the "ուղիղ ձև"**; every other form is a հոլովաձև. A list of all forms of a word is its **հոլովման հարացույց**.
- **Ներգոյական -ում is not used with animate/abstract nouns by norm**: write `ընկերոջ մեջ`, `վախի մեջ`, not `ընկերոջում`. Time words often take other forms: `գարնանը`, `գիշերով`.
- **Superlative**: stacking such as `ամենաուժեղագույն` is flagged by the textbook as logically faulty (double marking). Prefer `ամենաուժեղ` or `ուժեղագույն`.
- **Plural**: -եր after monosyllables, -ներ after polysyllables. Irregular: `մարդ → մարդիկ`, `կին → կանայք`; `տիկին/պարոն/անձ` have both regular forms and `տիկնայք/պարոնայք/անձինք`.
- **Numerals**: one word up to 100 (համադրական), from 101 separate words (հարադրական: `երկու հազար վեց հարյուր քառասունյոթ`). After `մեկ/մի` the noun is always singular. Ordinals from digits: `1-ին`, `2-րդ`; distributive `1-ական`.
- **Terminology changes**: the old "վերլուծական շարադրություն" is now **վերլուծական խոհագրություն** (essay genre). Շարահյուսություն = syntax, ձևաբանություն = morphology, բառագիտություն = lexicology, գրվածքագիտություն = text studies.
- **Don't confuse** ձևակազմություն (inflection: `քար-եր-ի`) with բառակազմություն (word formation: `քար-ե`, `քար-տաշ`).

## Quick self-check before answering

- Did I use the 5-case system and textbook terms?
- Did I keep Eastern Armenian and classical orthography?
- Did I use `։ ՝ ՞ ՛ «»` correctly?
- Did I flag anything I am not sure about?
