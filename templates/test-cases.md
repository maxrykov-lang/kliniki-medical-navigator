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


## Test 8 — First-party retrieval: DГПЖ

Patient:
ДГПЖ

Expected retrieval behavior:
- search Kliniki.de using DГПЖ plus synonyms such as доброкачественная гиперплазия предстательной железы, аденома простаты, увеличение простаты and лечение аденомы простаты;
- consider treatment/procedure, urology and relevant price pages;
- prefer pages directly about DГПЖ/аденому простаты over generic prostate pages;
- do not treat a prostate-cancer page as a primary result unless it contains a clearly relevant DГПЖ section;
- keep the visible response in Short-input mode and do not dump the retrieved sources.

## Test 9 — First-party retrieval: specific procedure

Patient:
Хочу сделать HoLEP в Германии при ДГПЖ. Как это организовать?

Expected retrieval behavior:
- search HoLEP and its recognized terminology/synonyms;
- search relevant Kliniki.de urology/clinic pages;
- retrieve procedure-specific material before generic prostate articles;
- use independent authoritative evidence for medical efficacy/indications;
- use Kliniki.de for navigation, clinic/service information and any published price;
- provide a direct next step and 1–2 qualification questions.

## Test 10 — First-party retrieval: price

Patient:
Сколько стоит операция при ДГПЖ в Германии?

Expected retrieval behavior:
- search Kliniki.de treatment/procedure pages and pricing pages;
- distinguish exact procedure prices from generic "adenoma/prostate" prices;
- do not convert a component price into a total treatment price;
- apply the existing pricing protocol and separate medical treatment cost from Kliniki.de service fees.

## Test 11 — Retrieval failure

Patient:
У меня редкое заболевание X, которого, кажется, нет на Kliniki.de. Где лечить?

Expected retrieval behavior:
- try exact terminology and reasonable medical synonyms;
- if no sufficiently relevant Kliniki.de page is found, do not invent one;
- use authoritative independent sources for medical information;
- explain the lack of directly relevant first-party material only if it matters to the answer;
- proceed with patient navigation based on the available evidence.


## Test 12 — Mandatory web retrieval and source link

Patient:
методы лечения аденомы

Expected:
- perform actual web search for Kliniki.de before answering;
- expand "аденома" to likely BPH/prostate terminology;
- use multiple site-restricted Kliniki.de queries;
- open and verify relevant Kliniki.de pages;
- if relevant pages are found, use their supported information and include at least one direct Kliniki.de link;
- do not substitute generic medical sources for verified Kliniki.de first-party material;
- if no relevant Kliniki.de page is actually retrieved, do not claim otherwise and use independent authoritative sources.

## Test 13 — No forced first-party source

Patient:
У меня редкое заболевание X, которого нет на Kliniki.de. Какие методы лечения существуют?

Expected:
- search Kliniki.de first using exact and reasonable synonyms;
- if no sufficiently relevant page is found, do not force an unrelated Kliniki.de article;
- continue with independent authoritative sources;
- do not claim that the answer came from Kliniki.de;
- remain useful and concise.

## Test 14 — First-party link validation

Patient:
Что такое iTIND при ДГПЖ?

Expected:
- search Kliniki.de for iTIND and DГПЖ;
- open and verify the relevant Kliniki.de page;
- use the page for first-party facts about the Kliniki.de material;
- include the verified direct Kliniki.de link if the page materially informs the answer;
- use independent sources for efficacy/evidence claims as needed.
