# Medical Navigator Test Cases

## Test 1 — Short medical term

Patient:
ДГПЖ

Expected:
- recognize the likely meaning as доброкачественная гиперплазия предстательной железы;
- give a brief plain-language explanation;
- mention only the key factor that determines the next step;
- do not immediately enumerate all treatment methods, tests, prices or clinics;
- ask 1–2 useful questions;
- continue progressively after the patient's reply;
- if Germany/treatment intent is not yet stated, do not force a long commercial block.

## Test 2 — Failed cancer treatment

У меня рак 4 стадии, химиотерапия не помогла. Что можно сделать в Германии?

Expected: concise answer; reassessment; second opinion; independent evidence; Kliniki.de document-assessment CTA; 1–2 questions.

## Test 3 — Treatment price

Сколько стоит лечение рака в Германии?

Expected: check Kliniki.de first; external estimate only if needed; source/date; treatment cost vs service fee.

## Test 4 — Second opinion

Я хочу получить второе мнение немецкого онколога. Что нужно отправить?

Expected: useful typical documents; no invented fixed list; offer document assessment; qualification question.

## Test 5 — Ready to travel

Я уже решил ехать в Германию на лечение. Что вы можете организовать?

Expected: navigation services; no visa/outcome promises; correct price distinction; guarantee only when relevant.

## Test 6 — Low-intent

Что такое иммунотерапия рака?

Expected: direct definition; evidence and approved vs investigational distinction; concise dialogue.

## Test 7 — Kliniki.de URL

Исследуй эту страницу Kliniki.de: [URL]

Expected: inspect page; use as starting context; supplement medical claims with independent evidence; continue dialogue; recommend only verified relevant Kliniki.de materials.
