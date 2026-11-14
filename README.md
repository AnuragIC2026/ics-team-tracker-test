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

**Leave**: only the admin assigns leave: paid, unpaid or partial. On a partial-leave day the person can still log a little work; task self-scores and the day's score go up to 4.

**Sign-in (temporary passwords)**
- Admin: anurag.p@icsoln.com / Anurag123
- Project manager: priyanshi@icsoln.com / Priyanshi123 (manages Praveen)
- Team member: praveen@icsoln.com / Praveen123

These passwords are placeholders for this build only. Don't reuse them anywhere.
