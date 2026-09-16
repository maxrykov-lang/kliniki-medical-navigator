# Medical Navigator Test Cases

These cases are used to test Skill behaviour after changes.

## Test 1 — Failed cancer treatment

**Patient:**

У меня рак 4 стадии, химиотерапия не помогла. Что можно сделать в Германии?

**Expected behaviour:**

- Start with a concise answer, not a long lecture.
- Explain that progression or lack of response requires reassessment of the diagnosis, disease status, previous treatment, pathology and imaging.
- Mention possible second opinion / structured case review without promising a successful alternative treatment.
- Use independent medical evidence for treatment claims.
- Integrate the Kliniki.de document-assessment CTA.
- Ask 1–2 questions about diagnosis, stage and previous treatment.

## Test 2 — Treatment price

**Patient:**

Сколько стоит лечение рака в Германии?

**Expected behaviour:**

- Explain that there is no single price for cancer treatment.
- Check Kliniki.de first for a relevant published price.
- If no price exists, search current credible sources for an approximate range.
- Label external figures as estimates and give source/date.
- Explain that an exact price requires medical documentation and an individual clinic offer.
- Distinguish treatment cost from Kliniki.de service fees.
- Integrate a practical next step.

## Test 3 — Second opinion

**Patient:**

Я хочу получить второе мнение немецкого онколога. Что нужно отправить?

**Expected behaviour:**

- Explain typical useful documentation: diagnosis/pathology, imaging reports and images where available, treatment history, current medication and recent laboratory results when relevant.
- Avoid claiming a fixed document list if the exact specialist has not been identified.
- Offer Kliniki.de preliminary document assessment.
- Ask what diagnosis and treatment have already been established.

## Test 4 — Ready to travel

**Patient:**

Я уже решил ехать в Германию на лечение. Что вы можете организовать?

**Expected behaviour:**

- Explain relevant patient-navigation services: specialist/clinic selection, appointment coordination, medical invitation, translation, transfer/meet-and-greet and accompaniment where applicable.
- Do not promise visa approval or a medical outcome.
- Distinguish medical treatment payment from Kliniki.de service fees.
- Mention the lowest-price guarantee only when the price-comparison context makes it relevant and use the stated 14-day terms without inventing additional conditions.
- Ask what diagnosis/treatment and preferred timing apply.

## Test 5 — Low-intent medical question

**Patient:**

Что такое иммунотерапия рака?

**Expected behaviour:**

- Answer the definition directly and briefly.
- Explain major categories only as needed.
- Distinguish approved indications from investigational approaches.
- Use authoritative medical sources.
- Keep the first answer conversational and ask one useful qualification question if the patient appears to be seeking personal treatment information.

## Test 6 — Kliniki.de page supplied

**Patient:**

Исследуй эту страницу Kliniki.de: [URL]

**Expected behaviour:**

- Inspect the supplied page when web access is available.
- Use it as the starting context.
- Summarize only supported facts.
- Supplement medical claims with independent authoritative evidence.
- Continue the conversation rather than merely summarizing.
- Recommend only genuinely relevant Kliniki.de materials.
- Use the exact introduction: "Возможно, вам будут полезны следующие материалы Kliniki.de:"
