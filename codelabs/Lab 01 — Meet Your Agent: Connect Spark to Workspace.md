# Lab 01 — Meet Your Agent: Connect Spark to Workspace

## 🏫 Scenario — The Training Coordinator

You're the **training coordinator** for a growing company. You organise internal training sessions, coordinate trainers, manage schedules, and keep track of the information that comes with each session.

Most of that information already lives in your Google Workspace:

- **Gmail** — registrations, questions, cancellations, and trainer communications.
- **Calendar** — training sessions, meetings, and speaker availability.
- **Drive** — training materials, attendance records, and previous session documents.
- **Docs and Sheets** — participant lists, session briefs, and follow-up reports.

The problem isn't that the information is difficult to find.

There's just **a lot of it**.

You've decided to build a Gemini Spark assistant to help with the routine work.

But before you ask it to do anything complicated, there's one thing you need to do first:

> **Give your new assistant access to the tools it needs.**

---

## 🎯 Goal

By the end of this lab, you will:

- Open Gemini Spark.
- Connect Spark to **Gmail, Calendar, and Drive**.
- Review the available approval controls.
- Run your first **read-only** agent task.
- Follow up on the result without starting a new task.

**Estimated time:** 10–15 minutes

---

## 🛠️ What You'll Build

A Gemini Spark agent that can access your:

- Gmail
- Calendar
- Drive

You'll also complete your first supervised task using Calendar data.

**Tools:** Gemini Spark, Google Account, Gmail, Calendar, Drive

---

## ✅ Prerequisites

Before you begin, make sure you have:

- A Google account with access to Gmail, Calendar, and Drive.
- Gemini Spark enabled for your account.
- Chrome or Microsoft Edge.
- You are signed in to the **correct Google account**.

> **Trainer note:** Confirm Spark availability before the workshop begins. Availability may depend on the user's account, plan, organisation, or region.

---

# 🚀 Steps

## Step 1 — Open Gemini

Open [Gemini](https://gemini.google.com/) in Chrome or Microsoft Edge.

Sign in using the Google account you will use throughout the workshop.

Make sure this is the account containing the Calendar, Gmail, and Drive data you want Spark to access.

---

## Step 2 — Find Spark

Open the area of Gemini where you can create or work with **agents**.

If you cannot find Spark or the agent functionality, **stop here and ask the trainer for help**.

> Don't spend five minutes fighting the UI. 😆

---

## Step 3 — Connect your Workspace

Open the available **connections, apps, or permissions** settings for Spark.

Connect the following:

- Gmail
- Calendar
- Drive

For this lab, **don't connect anything else unless the trainer asks you to.**

Follow Google's authorization flow and review what access is being requested before approving it.

---

## Step 4 — Check your approvals

Before giving Spark its first job, review the available **approval or confirmation controls**.

Keep approval/confirmation enabled.

The goal of this workshop is not to let the agent run wild.

> **You are still the human in the loop.**

This becomes especially important later when we move from reading information to creating or modifying things.

---

## Step 5 — Give Spark its first job

Time for the first task.

Start with something deliberately safe:

> **Read my Calendar and tell me what is coming up.**

Paste this instruction into Spark:

```text
List my next 3 calendar events with their date, time, and title.

Do not create, edit, delete, or change anything in my Calendar.
```

Run the task.

---

## Step 6 — Inspect the result

Look at what Spark returns.

![Lab 01](GDEGeminiSpark/assets/Lab01.jpeg)

Check:

- Are the three events correct?
- Are the dates and times correct?
- Are the titles correct?
- Did Spark leave your Calendar unchanged?

Don't just accept the answer automatically.

> **An agent's output is something you review, not something you blindly trust.**

---

## Step 7 — Keep the conversation going

Now let's see whether Spark can use the result from the previous task.

Ask:

```text
Of those 3 events, which ones have no agenda or description?
```

Notice that you didn't need to repeat the three event names.

Spark can use the context from the previous interaction to continue the task.

---

## Step 8 — Verify

Open your Calendar and confirm that nothing was changed.

You have just completed the basic agent loop:

```text
CONNECT
   ↓
INSTRUCT
   ↓
RUN
   ↓
REVIEW
   ↓
FOLLOW UP
```

Not bad for your first few minutes with an agent. 🚀

---

# ✅ Success Criteria

You're ready for the next lab when:

- [ ] Spark is connected to Gmail.
- [ ] Spark is connected to Calendar.
- [ ] Spark is connected to Drive.
- [ ] Approval/confirmation controls are enabled.
- [ ] Spark successfully returned your next three Calendar events.
- [ ] Your follow-up question worked using the previous context.
- [ ] Nothing in your Calendar was changed.

---

# 🧯 Troubleshooting

### I can't find Gemini Spark

Spark availability can vary depending on your Google account, subscription, organisation, or region.

If you cannot access Spark, **get Gemini AI Pro or Ultra**

### Spark can't access Gmail, Calendar, or Drive

Check that:

1. You're signed in with the correct Google account.
2. The relevant Workspace connection has been enabled.
3. You completed Google's authorization flow.
4. Your organisation hasn't restricted the required Workspace access.

If it still doesn't work, ask the trainer for help.

### Spark returned the wrong Calendar events

Check that you're using the Calendar associated with the Google account you connected to Spark.

You can also ask Spark to clarify which Calendar it is using.

---

# 🚀 Challenge

Ready for a little more?

Ask Spark:

```text
Look at my next 5 calendar events.

Tell me which events have guests outside my organisation.

Do not modify my Calendar.
```

Keep this task **read-only**.

Think about what information Spark had to inspect to answer the question.

---

# 🤔 Reflection

You've just experienced the difference between asking Gemini a question and giving an agent access to your Workspace.

In your own words:

> **What makes this interaction different from simply asking Gemini a question?**

Think about:

- What information Spark could access.
- What Spark actually did with that information.
- How you could continue the task without starting from scratch.
- Where you, as the human, remained in control.

---

## 🎉 Done!

You've connected your first agent to your Workspace.

You've also completed your first supervised task.

Next, we'll give your agent something more important than access:

# **Instructions.**

See you in **Lab 02 — Teach It the Job: Building an Agent Brief**. 🚀
