# Information Processing Example
Tasks demonstrated: summarizing, extracting, prioritizing

## 1. Raw Input
> EAS check-in recap: testing group confirmed at 50 users starting Oct 10 (confirmed by Sara). IT still owes the approval-limit config - "almost done." Finance flagged that manager training isn't scheduled yet. Someone asked if we're expanding to a second department - no decision. Budget increase still not approved. Next check-in Thursday.

## 2. Prompt Used
Context: Raw check-in notes for the EAS pilot, read by the project sponsor. Action: Summarize, extract decisions/actions, flag risks and open questions. Rules: Preserve names/dates/numbers; don't turn questions into decisions; mark gaps [Not Specified].

## 3. AI Output — First Draft
| Action Item | Owner | Deadline | Status |
|---|---|---|---|
| Finish approval-limit configuration | IT | Oct 10 | In progress |
| Schedule manager training | Finance | Oct 10 | Planned |

**Issue found on review:** config due date was only "almost done," not Oct 10. Manager training has no owner or date — Finance only flagged it, didn't take it on.

## 4. Human Review
Corrected the invented deadline and owner; preserved uncertainty.

## 5. Final Structured Output
**Bottom line:** Testing (50 users) confirmed for Oct 10 by Sara. Config and manager training remain open. Second-department expansion and budget increase are undecided.

| Action Item | Owner | Deadline | Priority | Status |
|---|---|---|---|---|
| Finish approval-limit config | IT | [Not Specified] ("almost done") | High | Open |
| Assign owner & schedule manager training | [Not Specified] | Before Oct 10 | High | Open |
| Decide on second-department expansion | [Not Specified] | [Not Specified] | Medium | Open decision |
| Approve budget increase | Sponsor | [Not Specified] | Medium | Pending |
