# Lab 01 - Setting up Spark & Workspace

## Scenario
## 🏫 The Training Coordinator

You are the **training coordinator** for a growing company. Every month, you organise internal training sessions for employees across different teams.
Your work is spread across Google Workspace:

- **Gmail** contains registration requests, questions, cancellations, and trainer communications.
- **Calendar** contains training sessions, meetings, and speaker availability.
- **Drive** contains training materials, attendance records, and previous session documents.
- **Docs and Sheets** are used to prepare participant lists, session briefs, and follow-up reports.

The training programme is growing, but the process hasn't changed. You still spend too much time searching for information, copying details between documents, preparing meetings, and keeping track of follow-ups.

You decide to build an **AI training assistant with Gemini Spark**.
The assistant won't replace you. Instead, it will handle the routine work while **you remain in control and review its actions**.

Across this workshop, you'll teach your agent how to:
1. Find and organise information across your Workspace.
2. Prepare useful summaries and documents.
3. Help manage email and follow-ups.
4. Work with Docs, Sheets, Slides and Calendar.
5. Turn a useful workflow into a reusable Skill.

### Your first mission

Before teaching the agent anything complicated, you need to make sure it can access the information it needs.

Connect Gemini Spark to your **Gmail, Calendar and Drive**, then run a simple supervised task.

> **Your goal: give your new assistant access to its workplace.**

Once that's working, we'll start teaching it how to do the job.

## Goal

Access Gemini Spark, connect it to Gmail, Calendar and Drive, and run a first supervised task.

## What you'll build

A working Gemini Spark connected to Gmail, Calendar and Drive, plus one completed, reviewed first task.

**Tools and techniques:** Gemini Spark, Google account, Gmail, Calendar, Drive, approvals

## Prerequisites

- A Google account with Workspace access (Gmail, Calendar, Drive).
- Gemini Spark enabled on your account — the trainer confirms this at the start of Day 1.
- Chrome or Edge, signed in to the correct Google account.

## Steps

### Step 1
Open gemini.google.com in Chrome or Edge and sign in with the Google account you will use for the course.

### Step 2
Find Gemini Spark (the agent/automation area). If you cannot see it, tell the trainer — access is confirmed at the start of Day 1.

### Step 3
Open the connections/permissions panel and confirm Spark can access Gmail, Calendar and Drive. Grant access to those three only, for now.
### Step 4
Read the approval setting: confirm Spark will ask before it sends email, shares files or edits anything. Leave approvals ON.

### Step 5
Run a first, safe task: ask the agent to list your three next calendar events. This only reads data, so it is a gentle first run.

Instruction to give the agent (paste into Gemini Spark):

```text
List my next 3 calendar events with date, time and title. Do not change anything.
```

### Step 6
Watch how the agent works: it states a plan, carries it out, and shows you the result. Read the result before doing anything else.

### Step 7
Ask one follow-up so you see the agent hold context: have it note which of those events has no agenda yet.

Instruction to give the agent (paste into Gemini Spark):

```text
Of those 3 events, tell me which have no agenda in the description.
```

### Step 8
Confirm nothing was changed in your calendar — this was a read-only task. You have now seen the full loop safely.

## Test it
Gemini Spark is connected to Gmail, Calendar and Drive, approvals are ON, and the agent has returned a correct list of your next three events without changing anything.

## Troubleshooting

- **You can't see Gemini Spark on your account.** Gemini Spark only available for PRO and ULTRA users at this moment
- **Spark says it can't access Gmail/Calendar/Drive.** Re-open the connections panel and grant access to those three apps. Make sure you granted access for the same Google account you are signed in to.

## Challenge

Ask the agent to also tell you which of your next five events are external (have guests outside your organisation) — still read-only.

## Reflection

LO1 — In your own words, what is the difference between Gemini answering a question and Gemini acting as an agent on your Workspace?
