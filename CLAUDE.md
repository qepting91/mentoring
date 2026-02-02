# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **framework-driven mentorship template repository** built on best practices from four foundational books:
- *The Coaching Habit* (Michael Bungay Stanier)
- *One Minute Mentoring* (Ken Blanchard & Claire Diaz-Ortiz)
- *Lean In* (Sheryl Sandberg)
- *Tribe of Mentors* (Tim Ferriss)

The repository provides templates, guides, and tracking documents for effective mentor-mentee relationships.

## Core Frameworks Integrated

### The Coaching Habit
- **The Advice Monster**: Mentors resist rushing to advice
- **Seven Essential Questions**: AWE ("And What Else?"), Focus ("What is the real challenge here for you?"), Foundation ("What do you want?"), and others integrated into meeting templates

### One Minute Mentoring
- **M.E.N.T.O.R. Model**: Mission, Engagement, Networking, Trust, Opportunity, Review
- **ROE (Return on Energy)**: Mentees report back on applied guidance
- **Sunset Clause**: Defined relationship endpoints

### Lean In
- **Mentee Ownership**: Drive the relationship, don't wait passively
- **Mentor vs. Sponsor**: Different roles, both tracked

### Tribe of Mentors
- **Multiple Mentors**: Build a "tribe" for different needs
- **Powerful Questions**: Specific, well-crafted questions unlock wisdom

## Repository Structure

```
mentoring/
├── guides/                         # Role-specific handbooks
│   ├── mentor_guide.md
│   ├── mentee_guide.md
│   └── conflict_resolution.md
├── goals/                          # SMART goals with framework integration
│   ├── long_term_goals.md
│   └── short_term_goals.md
├── meetings/                       # Templates with 7 Essential Questions
│   ├── 00-first-meeting-kickoff.md # Relationship launch
│   ├── YYYY-MM-DD.md               # Ongoing meetings
│   └── ending_the_mentorship.md    # Graceful conclusion guide
├── action-items/                   # Task tracking + ROE log
│   └── action_items.md
├── resources/                      # Books, courses, tools, web resources
│   ├── books.md
│   ├── courses.md
│   ├── tools.md
│   ├── web_resources.md
│   ├── seven_questions_quick_reference.md
│   └── claude_code.md              # Claude Code CLI cheatsheet
├── progress/                       # Skills matrix, certifications
│   ├── skills_matrix.md
│   └── certifications.md
├── reflections/                    # Structured journal templates
│   └── journal.md
├── feedback/                       # Radical Candor-based feedback
│   ├── mentor_feedback.md
│   ├── mentee_feedback_to_mentor.md
│   └── self_evaluation.md
├── networking/                     # Contacts + introductions tracking
│   ├── contacts.md
│   └── events.md
├── achievements/                   # Projects portfolio
│   ├── projects.md
│   └── certificates/
│       └── certificates.md
├── LICENSE                         # MIT License
├── README.md                       # Project overview and setup
├── relationship_agreement.md       # The mentorship contract
└── relationship_health_check.md    # M.E.N.T.O.R. diagnostic
```

## Key Conventions

- **ROE (Return on Energy)**: Mentees always report back on how they applied previous guidance
- **The Seven Questions**: Meeting templates include The Coaching Habit questions
- **Sunset Clause**: All mentorships have defined endpoints (typically 3-6 months)
- **Specificity**: Templates encourage specific questions over vague ones ("What should I do?" is discouraged)
- **Mentee-Driven**: Mentees own the agenda, scheduling, and follow-through

## Key Documents

| Document | Purpose |
|----------|---------|
| `relationship_agreement.md` | Must complete at start - defines terms, sunset clause |
| `guides/mentor_guide.md` | Complete mentor handbook with Advice Monster warning |
| `guides/mentee_guide.md` | Complete mentee handbook with ownership principles |
| `guides/conflict_resolution.md` | Handle disagreements using Radical Candor |
| `meetings/00-first-meeting-kickoff.md` | Different from regular meetings - relationship launch |
| `meetings/ending_the_mentorship.md` | Gracefully conclude the mentorship |
| `relationship_health_check.md` | M.E.N.T.O.R. framework diagnostic for stuck relationships |
| `resources/seven_questions_quick_reference.md` | Quick reference for The Coaching Habit questions |
| `feedback/mentee_feedback_to_mentor.md` | Bi-directional feedback templates |

## Local Viewing

```bash
npm install -g md-fileserver
mdstart
```
Navigate to http://localhost:4000
