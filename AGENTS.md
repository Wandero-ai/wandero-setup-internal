# Wandero Setup — Agent Instructions

> Guide users through complete Wandero setup. This repo is PUBLIC.

---

## Step 1: Verify GitHub Access

Ask the user:
- **Do you have a GitHub account?**
  - No → Guide them to https://github.com/signup
  - Yes → Continue

- **Have you been invited to the Wandero GitHub org?**
  - No → Tell them: "Ask your admin (Zaal) to invite you to the Wandero-ai GitHub org and add you to the appropriate team (admins or team)."
  - Yes → Continue

**Important:** The user's access level depends on which GitHub team they're in:
- `admins` team → ADMIN access (full access)
- `team` team → TEAM access (processes, playbooks)
- No team → ALL access (public docs only)

---

## Step 2: Install AI Coding Tool

Ask the user: **Are you a developer?**

### For Non-Developers → Antigravity

1. Go to https://www.antigravity.so/
2. Download and install Antigravity
3. Sign in with GitHub when prompted
4. Paste this repo URL when asked for a project

### For Developers → Windsurf

1. Go to https://codeium.com/windsurf
2. Download and install Windsurf
3. Sign in with GitHub when prompted
4. Open Windsurf and use this setup repo

---

## Step 3: Clone Wandero

Run this command:

```bash
git clone --recurse-submodules https://github.com/Wandero-ai/wandero.git
cd wandero
```

---

## Step 4: Verify Access

After cloning, check what folders are visible:

| Folder | Access Level | Who Can See |
|--------|--------------|-------------|
| `wandero/` | ALL | Everyone |
| `wandero/team/` | TEAM | Team members + Admins |
| `wandero/team/admin/` | ADMIN | Admins only |

**If `team/` is empty or missing:** The user doesn't have TEAM access. This is expected for external collaborators. Tell them to contact their admin if they believe they should have higher access.

---

## Step 5: Clone Admin Repo (Admins Only)

If the user is in the `admins` GitHub team, they also have access to `wandero-admin`:

```bash
git clone --recurse-submodules https://github.com/Wandero-ai/wandero-admin.git
cd wandero-admin
```

**What's in wandero-admin:**
- Partnerships and strategic documents
- Product sprints and roadmap
- Projects and experiments
- Internal operations

Skip this step if the user is not an admin or doesn't need admin-level access.

---

## Step 6: Get Started

1. Read `AGENTS.md` in the cloned wandero repo for detailed instructions
2. Start with `_index.md` files in each domain for overviews
3. Ask the user what they need help with

---

## Company Context

**Wandero** — Agentic AI platform automating travel company operations:
- Inquiry handling
- Itinerary generation
- Quote creation
- Ops handoff

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| "Permission denied" on clone | User not invited to org. Contact admin. |
| `team/` folder empty | User lacks TEAM access. Expected for external users. |
| `team/admin/` folder empty | User lacks ADMIN access. Expected for non-admins. |
| Git not installed | Install from https://git-scm.com/downloads |

---

*Repo: https://github.com/Wandero-ai/wandero-setup-internal*
