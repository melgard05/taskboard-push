# taskboard-push

Cloudflare Worker behind the Steve's Sanitation Task Board: stores crew push
subscriptions, sends push on request (/send), and every 30 minutes alerts the
starter and assignees of overdue tasks (once per task per due date).

Cloudflare deploys this repo automatically on every push to `main`.
Secrets and variables live in Cloudflare (Settings → Variables and Secrets),
never in this repo. KV binding `SUBS` → namespace `SUBS`.
 

First automatic deploy: 2026-10-21.
