# Connect DeceptIQ to GitHub (new private repository + two-way sync)

## What this task is

This task requires **no code changes**. Lovable's Git sync can only be connected from the Lovable UI — not from chat. The agent cannot create the repository, see the connection, or push. The plan is the exact supported procedure for you (Dhruv) to run.

## Key facts before you start

- Git sync **always creates a brand-new private repository**. It cannot link a repository that already exists.
- Connecting needs a workspace owner or admin for the GitHub connection; the project needs an owner/admin to be connected.
- One branch syncs at a time (default `main`); Lovable commits and pushes every change, and pushes you make to that branch sync back.
- Connecting does not publish the app — the live site stays separate.
- If you later disconnect and reconnect, a *new* repository is created each time.

## Steps (desktop)

1. Open **Project settings → Git** — press `Cmd+.` (Mac) / `Ctrl+.` (Windows/Linux), or click the project name top-left → Settings. Also reachable via **+** next to the chat input → **Project → GitHub**.
2. If the workspace has no GitHub connection yet, click **Add connection** (requires workspace owner or admin).
3. Click **Add account**, choose your GitHub account or organization in the popup, select **All repositories** or **Only select repositories**, then **Install & Authorize**.
4. If a connection already exists, click **Connect** beside it instead.
5. Lovable then creates a **new private repository** and starts two-way sync automatically. The repository appears under that account/org in GitHub.

## Steps (mobile)

Chat mode → bottom-right `...` → Settings → Git, or **+** → Project → GitHub, then follow steps 2–5 above.

## After connecting

- Every change made in Lovable is committed and pushed to the synced branch; commits pushed there from GitHub sync back into Lovable.
- A draft does not appear in the repository until it is accepted or pushed as a branch/PR.
- To move code into an **existing** repository instead, use Project settings → Git → Download codebase (paid plans) and push manually — Git sync cannot target an existing repo.

## Verification

- The Git status card in Project settings → Git shows the connected repository and sync state.
- The new private repository shows up in your GitHub account with the project's code (92 tracked files, all committed — clean working tree, nothing oversized or secret-looking).
- No app code, scores, features, or layout are touched by this task.
