# Prompt Library

Reusable prompts for recurring Business Analyst tasks on the fictional Expense Approval System (EAS) pilot.

| Prompt Name | Workplace Task | Framework | Prompt | Expected Output |
|---|---|---|---|---|
| Requirements Extractor | Pull requirements from stakeholder notes | C.A.R.E. | Context: I am a Business Analyst reviewing anonymized workshop notes for the EAS pilot. Action: Extract requirements, constraints, assumptions, and open questions. Rules: Use only supplied notes; mark missing owners/dates [Not Specified]. Expected Output: Table with ID, category, statement, status, owner. | Traceable requirements table with gaps flagged |
| Status Brief Builder | Turn meeting notes into a brief | C.A.R.E. | Context: Raw notes from an EAS pilot check-in. Action: Summarize into a decision-ready brief. Rules: Keep names/dates/numbers; don't convert suggestions into decisions. Expected Output: 3-bullet summary plus action table (Owner, Deadline, Priority, Status). | Short brief with clear actions |
| Delay Notice Email | Communicate a schedule slip | R.C.T.O. | Role: Business Analyst. Context: EAS pilot delayed from Oct 1 to Oct 10 due to vendor testing. Task: Write a short update email to stakeholders. Output: Subject plus 2 short paragraphs, professional tone, no blame. | Concise, accurate delay email |
| Risk Log Builder | Convert updates into a risk log | C.A.R.E. | Context: Anonymized EAS pilot updates. Action: Identify risks, issues, dependencies. Rules: Don't assign probability/owner unless supported; flag unknowns. Expected Output: Table (Type, Description, Evidence, Owner, Status). | RAID-style log, gaps marked [Not Specified] |
| Rollout Plan Chain | Build a phased rollout plan | C.A.R.E. | Context: 4-week EAS pilot for one department. Action: Break goal into mechanisms, phases, tasks. Rules: Keep realistic; no invented owners/dates. Expected Output: 1-Goal, 2-Mechanisms, 3-Phases, 4-Tasks. | Short, actionable plan |

## When I'd Use These
- Requirements Extractor: after a stakeholder workshop
- Status Brief Builder: after a messy check-in meeting
- Delay Notice Email: when a confirmed schedule change needs communicating
- Risk Log Builder: during weekly pilot monitoring
- Rollout Plan Chain: when turning an approved goal into a work plan

## Example Outputs
**Status Brief Builder**: "EAS pilot testing is on track for 50 users; the approval-limit config is still pending; no owner assigned yet for user training."

**Delay Notice Email**: "Subject: EAS Pilot — Updated Start Date. The pilot start has moved from Oct 1 to Oct 10 due to vendor testing. Please adjust your schedules accordingly."
