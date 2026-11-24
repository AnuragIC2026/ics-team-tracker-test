# ICS Team Tracker

IC Solutions Team Tracker: daily work logs, task planning with carry-over and redo, holidays and leave, monthly scores.

This repository hosts the GitHub Pages build. It runs fully in the browser; data is saved per browser.
The production app (Node + MySQL, server-checked login and roles, email OTP, notices, Claude scoring) is deployed on the VPS from a private repository.

**Roles**
- **Admin** sees and manages everyone, and sets each person's role and project manager in the Team tab.
- **Project manager** sees everyone's scores, plus full task details for their assigned team members, and plans, reviews, redoes and unlocks for them.
- **Team member** sees everyone's scores, but only their own tasks, updates and comments.

**Deadline**: each day's update can be filled that day or until 8 am IST the next morning; after that it locks and scores 0. All dates and times are IST.

**Redo / reassign**: a project manager (within their team) or the admin can repost an unsatisfactory task to the same person or reassign it to someone else; it then stops carrying over for the first person.

**Tasks**: planned tasks can be Urgent, High or Low (Urgent + High = Critical) and are listed in that order. Team members score tasks on collapsible cards, can add tasks for themselves, and mark backlog (carried-over) tasks Pending, In progress or Done.

**Team**: the admin adds people in the Team tab (they sign in with their work email and FirstName123), removes them (history kept, can be restored) or deletes them permanently.

**Plan tasks and Review** show a scrollable team list on the left (grouped by project manager, with search and filters) and one person at a time on the right, with Save & next / Approve & next.

**Past days** are read-only: only the admin can add or change tasks on them. **Click a name** in the Month ledger to open that person's day-by-day page (admin: anyone; project manager: their team and themselves; team member: only themselves). People who leave move to **Former members** in Team, with their work kept.

**Logs** (admin only): a Logs tab shows who did what and when: activity (updates, plans, scores, leave, holidays, team changes), sign-ins (including wrong passwords), emails sent and Claude's suggested scores, with filters for person, dates and words. Each person's page also shows their recent activity. On this test site the log is kept in your browser and no emails are sent; the hosted version keeps everything on the server, forever.

**Leave**: only the admin assigns leave: paid, unpaid or partial. On a partial-leave day the person can still log a little work; task self-scores and the day's score go up to 4.

**Sign-in (temporary passwords)**
- Admin: anurag.p@icsoln.com / Anurag123
- Project manager: priyanshi@icsoln.com / Priyanshi123 (manages Praveen and Krisha)
- Team members: praveen@icsoln.com / Praveen123, krisha@icsoln.com / Krisha123

These passwords are placeholders for this build only. Don't reuse them anywhere.
