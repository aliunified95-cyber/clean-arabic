---
name: clean-arabic-by-am95
description: Edit, review, localize, or create Arabic content when advanced grammatical accuracy, morphology, context-sensitive wording, game narrative, or GCC cultural fit matters.
metadata:
  short-description: Advanced context-aware Arabic editing and localization
---

# Clean Arabic by AM95

Produce accurate, natural Arabic that preserves intent, facts, voice, narrative function, and technical constraints. Translation transfers meaning and effect; it is not word substitution.

## Context and register
Identify deliverable, audience, locale, genre, speaker, relationship, tone, and function (UI, tutorial, quest, dialogue, lore, etc.). Use MSA for cross-market/formal content unless specified. A named Gulf variety is required for dialect localization; “GCC Arabic” is not one dialect. Use project briefs, context, approved strings, glossary, and character notes. Preserve implication, humor, ambiguity, reveals, and voice. Recast freely for idiomatic Arabic, but do not invent facts, mechanics, relationships, or lore. Ask only if a missing choice materially changes the result; otherwise state a reasonable assumption. Flag genuine source ambiguity rather than silently selecting a consequential meaning.

## Grammar, morphology, and orthography
Analyze clauses in context. Check syntax, case/mood where relevant, government, definiteness, tense/aspect/voice, negation, conditionality, coordination, relative clauses, ellipsis, and pronoun reference. Check derivation and inflection where useful: roots/patterns, weak and hamzated roots, gemination, verb forms, maṣdar, participles, sound/broken plurals, nisba, diminutives, and clitics. Never infer meaning from a guessed root or pattern alone. Distinguish valid variation and competing analyses from errors; do not impose one school-specific interpretation as universal.

Check standard contemporary spelling and house style: hamza, alif maqṣūra/yāʾ, tāʾ marbūṭa, shadda/tanwīn if required, clitic spacing, punctuation, numerals, and diacritics. Do not fully vocalize by default; vocalize for disambiguation or when requested.

Track every pronoun to an antecedent; check person, gender, number, function, attached/detached form, and ambiguity. Review agreement among subject, verb, adjective, demonstrative, numeral, relative pronoun, and pronoun. Account for Arabic patterns such as postverbal singular agreement with plural subjects in common standard constructions, feminine singular agreement with many non-human plurals, semantic agreement, and valid exceptions. Check duals, human/non-human reference, collectives, mass nouns, grammatical versus natural gender, sound/broken plurals, and numeral polarity/counted-noun form for 1–2, 3–10, 11–12, 13–19, tens, hundreds, and compounds. Never apply English agreement intuitions mechanically. Follow register and product conventions for dates, units, currencies, counters, and displayed quantities.

## Semantics and editing
Preserve agency, polarity, scope, certainty, politeness, emphasis, emotional force, and pragmatic effect. Check collocations, false friends, idioms, phrasal verbs, metaphors, wordplay, sarcasm, and cultural assumptions. Choose words by intended sense, not dictionary headword alone. Edit for clarity, rhythm, economy, naturalness, and voice. Remove calques, needless passives, inflated nominalizations, redundant pronouns/connectives, and ornamental synonym changes. Avoid archaic diction in contemporary UI unless intended; do not flatten literary voice.

## English-to-Arabic localization
First identify actor, action, object, player-facing purpose, and intended effect. Rebuild the sentence around natural Arabic information flow. Localize idioms and humor by effect; preserve world terms; adapt examples only when authorized. For UI prioritize clarity, brevity, consistent terminology, and action. Respect placeholders, markup, tags, line breaks, pluralization logic, gender variants, and character/byte limits. Never translate protected tokens. Preserve ambiguity only if it is intentional and works in Arabic; flag untranslatable wordplay with a proposed adaptation.

### Lifuna game narrative
Treat the supplied game bible, narrative, glossary, build strings, character profiles, and approved decisions as authority. Preserve canon, player knowledge, quest logic, emotional arcs, character voice, and consistent world terminology. Keep fictional terminology distinct from real-world cultural terms. Do not assume what Lifuna refers to or invent setting details. Ask or flag when context is insufficient.

### Variables and runtime strings
Variables are immutable interface contracts: preserve exact spelling, braces, case, markup, formatting, positional order, and syntax unless specs allow change. Reorder only using supported named tokens or explicit remapping. Check grammar around unknown names, selected gender, and runtime quantities; use neutral constructions if gender is unavailable. Do not attach clitics to tokens if formatting can split/change them. Distinguish tokens from sample values. Inspect full rendered text when fragments concatenate; Arabic may require different agreement, word order, spacing, or prepositions. Recommend whole-sentence strings/variants if concatenation makes correct Arabic impossible. Consider RTL rendering and mixed Arabic/Latin text, numerals, punctuation, parentheses, and codes.

## GCC cultural fit
Use the named market and audience. Do not treat Gulf, Saudi, or GCC as interchangeable. Check currencies, dates, units, names, honorifics, cultural/religious references, food, clothing, social roles, humor, and sensitive topics against the brief and approved policy. Do not add religious language, local color, or stereotypes not supported by source or brief. Record necessary adaptations and their rationale. Prefer neutral MSA across GCC where no market direction is given. Seek qualified local review for sensitive or market-specific decisions.

## Terminology governance
Use approved glossary and translation memory first. For each term record source, approved Arabic, sense/definition, part of speech, grammatical gender, plural/inflection, register/locale, prohibited variants, context, owner/status, and examples as useful. Separate product/UI terms, narrative canon, names, cultural terms, and linguistic terminology. Record decisions; never silently revise an approved term. Flag collisions, polysemy, inconsistent spellings, and changed source meaning. Dictionaries inform choices; product approval governs chosen terminology.

## QA protocol
1. Intent/context: compare source, scene, audience, function, and target effect.
2. Grammar/morphology: inspect syntax, inflection, agreement, pronouns, numerals, spelling.
3. Meaning/voice: check scope, nuance, idiomaticity, tone, and character consistency.
4. Localization/culture: check register, market assumptions, adaptation, terminology.
5. Technical integrity: compare tokens, tags, markup, line/length limits, RTL and concatenation.
6. Proofread Arabic alone, aloud if useful; ensure it works without leaning on English.

Classify defects as blocking (wrong meaning, broken token, canon/fact error, serious grammar), major (misleading/unnatural, inconsistent term, voice/register mismatch), or minor (punctuation or optional polish). Do not invent findings. For edit requests, give the final Arabic first; explain consequential changes only. For audits, report issue, correction, concise rationale. Separate errors from style choices and state uncertainty honestly.

## References
Use [Arabic sources](references/arabic-sources.md) when a decision needs reference support. Read only relevant parts. Verify online availability when current access matters. Cite when requested or when substantiating a disputed claim; a dictionary does not settle context or product style.

