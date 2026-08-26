# Lab 03 — Send It to Work: Research & Organise

> **Connected project:** In Lab 02, you learned how to brief your Gemini Spark agent. Now it's time to give that agent some actual work.

## 🎯 Goal

Use Gemini Spark to complete practical, one-off tasks across your Google Workspace.

You'll ask the agent to:

- Research information and turn it into a useful document.
- Organise information from Gmail.
- Propose a better structure for files in Drive.
- Take action only after you've reviewed and approved the plan.

The key idea:

> **Delegation doesn't have to mean automation.**

Sometimes you just need an agent to take a job off your plate once.

**Estimated time:** 15–20 minutes

---

## 🏫 Scenario — Preparing the Next Training Session

Your next internal training session is coming up.

You've already booked the session and have the basic logistics in place, but there is still plenty of preparation to do.

You need to:

- Find useful ideas for the session.
- Make sense of recent training-related emails.
- Organise the materials you've collected in Drive.

Normally, you'd open several tabs, search through emails, browse folders, and manually put everything together.

This time, you're going to delegate some of that work.

You won't create a permanent automation yet.

Instead, you'll give Spark **three different one-off jobs** and review what it produces.

---

## 🛠️ What You'll Build

By the end of this lab, you'll have:

- A structured research brief in Google Docs.
- A proposed organisation scheme for training-related emails.
- A proposed folder structure for training materials.
- A small, approved set of Workspace changes.

**Tools and techniques:** One-off agent tasks, research, summarisation, Gmail organisation, Drive organisation, Google Docs, review and approval

---

## ✅ Prerequisites

Before starting, make sure you have:

- Lab 01 complete.
- Lab 02 complete.
- Gemini Spark connected to Gmail, Calendar, and Drive.
- Your **Agent Brief** from Lab 02.
- Some non-confidential emails in Gmail.
- A Drive folder containing several files you can safely experiment with.

> **Tip:** If you don't want to use your real Workspace data, create a small set of practice emails and files specifically for this lab.

---

# 🚀 Steps

## Step 1 — Give Spark a research assignment

Let's start with something that doesn't require changing anything.

Imagine you're preparing an upcoming training session and want some fresh ideas for making the session more engaging.

Give Spark this task:

```text
CONTEXT:
I am preparing an internal employee training session.

JOB:
Research 3 practical ways to make a training session more interactive.

OUTPUT:
Create a Google Doc titled "Training Engagement Ideas".
For each idea, include a short explanation, one example activity, and the source.
Keep the document concise.

BOUNDARIES:
Use reliable sources.
Do not create or modify anything outside the requested document.
```

Run the task.

---

## Step 2 — Review the research

Open the resulting Google Doc.

Check whether it contains:

- The requested title.
- Three distinct ideas.
- A useful explanation for each idea.
- An example activity.
- Sources.
- Information that is actually relevant to your training session.

Don't focus only on whether Spark completed the task.

Ask yourself:

> **Would I actually use this document?**

If not, identify what needs improvement.

---

## Step 3 — Improve the result

If the research is too generic, give Spark a refinement.

For example:

```text
Make the three ideas more suitable for a 60-minute
internal training session with adult employees.

Keep the existing structure, but replace any ideas
that would require expensive equipment or extensive preparation.
```

Review the updated document.

Notice what just happened:

```text
TASK
 ↓
RESULT
 ↓
REVIEW
 ↓
FEEDBACK
 ↓
BETTER RESULT
```

This is an important part of working with agents.

**Your first instruction doesn't have to be perfect.**

---

## Step 4 — Delegate an inbox task

Now let's move from research to organisation.

Your inbox contains messages related to training, but they're mixed together with everything else.

Ask Spark to **classify** the relevant emails.

Use:

```text
CONTEXT:
I am preparing for upcoming internal training sessions.

JOB:
Review my unread emails from the last 7 days and identify messages
related to training, registrations, trainers, venues, or participants.

OUTPUT:
Create a list grouped into:
- Registration
- Trainer
- Logistics
- Participant
- Other

For each email, include the sender and subject.

BOUNDARIES:
Do not archive, delete, label, reply to, or send anything.
```

Run the task.

---

## Step 5 — Review before changing anything

Review Spark's classification.

Look for:

- Incorrect categories.
- Messages that aren't actually training-related.
- Important messages that Spark missed.
- Messages that you're not sure about.

If something is wrong, tell Spark what to correct.

For example:

```text
Move the email from Alex about the training room
from "Other" to "Logistics".
Do not make any other changes.
```

The important part is that **you decide what happens next**.

---

## Step 6 — Give Spark a Drive organisation job

Now let's look at your training materials.

Ask Spark to inspect a folder containing several files and **propose** a better structure.

For example:

```text
CONTEXT:
My Drive contains materials for upcoming and previous training sessions.

JOB:
Review the files in my training materials folder and suggest
a folder structure that would make them easier to find.

OUTPUT:
Show me:
1. The proposed folder structure.
2. Which existing files would go into each folder.
3. Any files that don't clearly belong anywhere.

BOUNDARIES:
Do not create folders.
Do not move, rename, delete, or modify files yet.
```

Run the task.

---

## Step 7 — Review the proposed structure

Look at Spark's proposal.

Ask yourself:

- Does the structure make sense?
- Are the categories useful?
- Did Spark understand the purpose of the files?
- Are any files in the wrong place?
- Is the structure unnecessarily complicated?

Make at least **one change** to the proposal.

For example:

```text
Combine "Trainer Materials" and "Presentation Materials"
into one folder called "Session Materials".

Show me the updated structure.
Do not move anything yet.
```

Review the updated proposal.

---

## Step 8 — Approve a small change

Now let's allow the agent to act.

Choose a small, safe subset of files.

For example:

```text
Create the "Session Materials" folder
and move only the two files we discussed into it.

Do not move, rename, or delete anything else.
Ask for confirmation before making the changes.
```

Review the proposed action and approve it if everything looks correct.

---

## Step 9 — Verify the result

Open Google Drive yourself.

Check that:

- The folder was created correctly.
- Only the files you approved were moved.
- The files still open correctly.
- Nothing else was changed.

You've just experienced an important distinction:

```text
READ
 ↓
PROPOSE
 ↓
REVIEW
 ↓
APPROVE
 ↓
ACT
 ↓
VERIFY
```

That's a very different experience from simply asking Gemini for an answer.

---

# 🧠 What Did We Just Learn?

You've now used Spark for three different kinds of work:

| Task | Agent behaviour |
|---|---|
| Research | Find and synthesise information |
| Gmail | Inspect and organise information |
| Drive | Plan and perform an action |

Notice that not every task needed automation.

The research task was useful **right now**.

The Gmail task might be useful every week.

The Drive organisation task might only be needed occasionally.

That's the difference between:

> **"Can an agent do this?"**

and:

> **"Should I automate this?"**

We'll explore that distinction later.

---

# ✅ Success Criteria

You're ready for the next lab when you can show:

- [ ] A research Doc created by Spark.
- [ ] The research output reviewed and refined.
- [ ] Training-related emails classified without unwanted changes.
- [ ] A Drive organisation plan generated by Spark.
- [ ] At least one change made to the proposed structure.
- [ ] A small set of Drive changes approved and completed.
- [ ] The final changes verified manually.

---

# 🧯 Troubleshooting

### The research result is too generic

Your research task may need more context.

Specify:

- Who the training is for.
- How long the session is.
- What type of training you're preparing.
- Any practical constraints.

For example:

```text
The session is 60 minutes long and is delivered
to employees with mixed technical backgrounds.

Prioritise activities that require little preparation
and can be completed in a normal meeting room.
```

### Spark classified an email incorrectly

Tell it exactly what was wrong.

For example:

```text
The email from Sarah about room setup is related to logistics,
not registration.

Reclassify that email only.
```

Then review the result again.

### Spark wants to move everything immediately

Don't approve the action.

Ask it to show the proposed changes first:

```text
Show me the proposed changes before making them.
Do not move, rename, delete, or modify anything yet.
```

Keep your approval controls enabled.

### Spark proposed too many folders

Tell it to simplify.

For example:

```text
Reduce the structure to no more than 4 top-level folders.
Keep the categories broad enough to remain useful.
```

Remember:

> **The best organisation system is usually the one you'll actually use.**

### Spark can't access the files

Check that:

1. The correct Google account is connected.
2. The folder is accessible to that account.
3. The files are actually inside the folder you specified.
4. Your organisation hasn't restricted access to the required Drive content.

---

# 🚀 Challenge

Let's push the agent a little further.

Ask Spark to inspect a training materials folder and identify **possible duplicate or near-duplicate files**.

Use:

```text
Review the files in my training materials folder.

Identify files that appear to be duplicates or different versions
of the same document.

For each group, show:
- File names
- Why they appear related
- Which file you recommend keeping
- Which files could potentially be archived

Do not delete, move, rename, or archive anything.
This is a proposal only.
```

Review its recommendations.

### Bonus question

Ask yourself:

> **Would you trust an agent to automatically delete the files it identified?**

Why or why not?

---

# 🤔 Reflection

You've now delegated several real tasks to your agent.

Think about the experience:

> **Which task saved you the most effort?**

Then consider:

> **Which task would benefit from being repeated regularly?**

And finally:

> **Would you automate it, or would you still prefer to run it manually when needed? Why?**

---

## 🎉 Done!

You've moved beyond simply **asking** your agent questions.

You've started **delegating work**.

You've also seen why review and approval matter when an agent can interact with your Workspace.

Next, we'll give Spark a job that lives in almost everyone's favourite place:

# **The Inbox. 📬**

See you in **Lab 04 — Inbox Duty**.
