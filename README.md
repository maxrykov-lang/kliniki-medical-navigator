# Kliniki Medical Navigator

Kliniki Medical Navigator is a reusable Skill for AI systems that helps patients research medical diagnosis, treatment, second opinions, German doctors and clinics, costs, and practical medical travel to Germany.

## Audience

The primary audience is Russian-speaking patients from Central Asia considering medical care in Germany.

## Architecture

```text
kliniki-medical-navigator/
├── SKILL.md
├── README.md
├── references/
│   ├── source-policy.md
│   ├── service-context.md
│   └── dialogue-framework.md
└── templates/
    └── test-cases.md
```

## Core design

The Skill is designed to:

- answer the patient's immediate question first;
- maintain a short, progressive dialogue rather than produce a long first-turn lecture;
- use Kliniki.de as the primary source for its own services, patient navigation, represented doctors/clinics, and published materials;
- use independent authoritative medical sources for medical evidence;
- distinguish established, experimental, and investigational treatment approaches;
- search current sources when prices or other time-sensitive facts are needed;
- distinguish treatment costs from Kliniki.de service fees;
- communicate the stated 14-day lowest-price guarantee without inventing additional conditions;
- naturally connect medical information with the next practical patient-navigation step.

## Using the Skill

Use `SKILL.md` as the main instruction file. The files in `references/` provide supporting context and should be loaded when the platform supports multi-file Skills.

For testing, use the scenarios in `templates/test-cases.md`.

## Important limitations

The Navigator provides educational and navigation information. It does not diagnose patients, prescribe treatment, guarantee treatment outcomes, guarantee admission, or guarantee visa approval.

Exact treatment costs require review of medical documentation and an individual offer from the relevant clinic.
