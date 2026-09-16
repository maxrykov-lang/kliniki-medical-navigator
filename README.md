# Kliniki Medical Navigator

Claude-compatible multi-file Agent Skill for patient-facing medical navigation related to treatment, second opinions, German doctors and clinics, costs and medical travel to Germany.

## Structure

kliniki-medical-navigator/
├── SKILL.md
├── README.md
├── references/
│   ├── source-policy.md
│   ├── service-context.md
│   └── dialogue-framework.md
└── templates/
    └── test-cases.md

## Claude compatibility

The Skill uses required YAML frontmatter (`name` and `description`) in `SKILL.md` and a multi-file progressive-disclosure structure. Supporting resources are referenced explicitly from `SKILL.md`.

Package the folder as a ZIP with the skill folder as the ZIP root before uploading to Claude Customize → Skills → Create skill → Upload a skill.

## Limitations

The Navigator provides educational and navigation information. It does not diagnose, prescribe, guarantee admission, treatment outcome or visa approval.
