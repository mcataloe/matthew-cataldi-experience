# Personnel Operations Platform

## Context

Rockford Symphony Orchestra required recurring personnel operations across musician booking, scheduling, attendance, contracting, payroll calculation/preparation, replacements, auditions, reporting, travel/mileage rules, and season/cycle management.

Matthew's official role was personnel management. In practice, the work evolved into roughly a 50/50 mix of personnel operations and software/platform development because he built software to streamline and operate the domain.

## Matthew's contribution

Matthew independently built and operated a live internal production-use platform using Microsoft Access, VBA, and Access/SQL query logic.

Implemented capabilities included:

- contracts;
- attendance;
- mileage and travel calculations;
- auditions, including campaign setup, deposit intake/recording, time-slot scheduling, and multiple audition rounds;
- season and cycle management;
- venues, ensembles, and auxiliary personnel;
- reporting;
- role-based permissions and user settings;
- startup/configuration tasks;
- Microsoft Office automation;
- Outlook, Word, Excel, Acrobat, Dropbox, and Google API workflow integrations.

## Domain model and correctness

The platform modeled seasons, cycles, and services with override behavior at different levels. It used database keys and unique constraints to prevent duplicate payroll, attendance, and booking records.

Payroll processing used transaction/rollback behavior, and Matthew ran post-processing reconciliation checks to ensure musicians who attended a concert cycle were represented in payroll.

These are approved local database/workflow correctness patterns. They should not be described as distributed exactly-once processing, message-queue semantics, or enterprise ledger architecture.

## Operational scale

The cumulative database contained records for more than 1,200 roster, substitute, and historical musicians. The core orchestra was typically around 60–70 musicians, and the largest active cycle was approximately 110 people.

The 1,200+ figure is not a direct-report count and does not represent simultaneous active staffing.

## Production-use boundary

The application was live and relied upon for consequential personnel workflows including payroll calculation/preparation, attendance, contracts, cycle staffing, scheduling, mileage/travel/cartage calculations, roster history, and audition administration.

Safe public wording includes `live internal production-use platform` or `production-use internal application` when the internal-platform boundary is preserved.

Production use does not imply public SaaS, cloud hosting, enterprise scale, conventional software-company operations, formal SRE/on-call practice, or multi-engineer production operations.

## Outcomes

Approved qualitative outcomes include reduced manual work, fewer duplicate records, better payroll confidence, improved leadership visibility, faster contract and payroll preparation, cleaner roster history, and substantially streamlined audition workflows.

No measured percentages, quantified time savings, or quantified payroll-error reductions are approved.

## Evidence boundaries

- Matthew was not originally hired primarily as a software engineer.
- Do not rewrite the official Personnel Manager role as a conventional Software Engineer title.
- The exact date when software became roughly half of the role is not established, so the full 2013–2018 interval should not be mechanically counted as full-time software-development years.
- The platform was not a cloud platform, web application, enterprise SaaS product, or multi-engineer system.
- Payroll responsibility should be framed as calculation/preparation/support, not ownership of the orchestra's entire finance function.
- Google API usage is verified; do not generalize that into broad API/WebAPI implementation claims for this project.
- Music-sector personnel management is not software-engineering management.
