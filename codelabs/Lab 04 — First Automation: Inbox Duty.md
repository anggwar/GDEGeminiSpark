# Lab 04 — First Automation: Inbox Duty 📬

> **Connected project:** In Lab 03, you gave your Gemini Spark agent several one-off jobs. Now we're going to turn one of the most repetitive jobs — dealing with email — into a repeatable workflow.

## 🎯 Goal

Use Gemini Spark to turn a messy inbox into an actionable workflow.

You'll have Spark:

- Prioritise incoming email.
- Summarise what actually needs your attention.
- Draft replies using your preferred communication style.
- Save those replies for your review.
- Send only the responses you explicitly approve.

The key idea:

> **Let the agent prepare the work. You make the final call.**

**Estimated time:** 15–20 minutes

---

## 🏫 Scenario — Inbox Duty

The training programme is getting busier.

Every morning, your inbox contains messages about:

- Employee registrations.
- Trainer availability.
- Training cancellations.
- Venue changes.
- Questions from participants.
- Requests for additional training.
- General announcements.

Most of these emails aren't difficult.

The problem is figuring out:

> **Which ones actually need your attention?**

And once you've found them, you still need to reply.

So today, you're going to give Spark a repeatable inbox workflow:

```text
READ
 ↓
PRIORITISE
 ↓
SUMMARISE
 ↓
DRAFT
 ↓
REVIEW
 ↓
APPROVE
 ↓
SEND
```

---

## 🛠️ What You'll Build

By the end of this lab, you'll have:

- A prioritised inbox digest.
- Reply drafts for emails that require action.
- A simple instruction describing your email style.
- Reviewed and approved replies ready to send.

**Tools and techniques:** Gmail, inbox summarisation, prioritisation, reply drafting, tone instructions, Gmail drafts, human approval

---

## ✅ Prerequisites

Before starting, make sure you have:

- Lab 01 complete.
- Lab 02 complete.
- Lab 03 complete.
- Gemini Spark connected to Gmail.
- Several recent, non-confidential emails.
- At least two emails that would reasonably require a reply.

> **Tip:** If your inbox doesn't contain suitable messages, ask the trainer for the workshop sample data.

---

# 🚀 Steps

## Step 1 — Turn your inbox into a to-do list

Instead of reading every email one by one, ask Spark to identify what actually needs your attention.

Give it this instruction:

```text
Review my unread emails from today that are related to
training activities.

Group them into:

1. Urgent
2. Needs a reply
3. FYI

For each email, show:
- Sender
- Subject
- What they need from me

Do not reply to, archive, delete, or modify any emails.
```

Run the task.

---

## Step 2 — Check the priorities

Read the resulting digest.

Ask yourself:

- Did Spark identify the important emails?
- Is anything marked urgent that shouldn't be?
- Did it miss an email that actually needs a response?
- Does the summary tell you what action is required?

The word **"urgent"** can mean different things to different people.

For example, your definition might be:

> An email is urgent if it requires action today or could affect an upcoming training session.

If Spark's priorities aren't useful, refine the instruction:

```text
For this task, consider an email urgent only if:
- it requires action today, or
- it could affect a training session happening within the next 48 hours.

Re-run the prioritisation.
Do not modify any emails.
```

Review the new result.

---

## Step 3 — Teach Spark how you communicate

Now we need to solve a different problem.

A technically correct email can still sound completely wrong.

Think about how you normally write emails.

Give Spark a short description of your style.

For example:

```text
My email style is:

- Warm but professional.
- Short and direct.
- Plain English.
- I answer the specific question first.
- I avoid unnecessary formal language.

I usually open with "Hi <name>," and sign off with
"Thanks, <YOUR NAME>".

Use this style when drafting replies for me.
```

You can change this to match your own communication style.

> **Don't try to describe your entire personality.**
>
> Give the agent enough information to reproduce how you actually write.

---

## Step 4 — Draft the replies

Return to the emails Spark identified as **Needs a reply**.

Ask it to prepare the responses.

```text
Draft replies to the emails you identified as "Needs a reply".

Use the email style I just provided.

Answer the specific request in each email.
Use only information available in the email and my connected Workspace.

Save the responses as Gmail drafts.

Do not send anything.
```

Run the task.

---

## Step 5 — Review the drafts

Open the drafts in Gmail.

For each one, check:

### Accuracy

- Did Spark understand the actual request?
- Are the dates, names, and details correct?
- Did it invent anything?

### Tone

- Does it sound like something you would actually send?
- Is it too formal?
- Is it too wordy?
- Does it sound like an AI wrote it?

### Completeness

- Did it answer the actual question?
- Did it miss an important detail?
- Does the recipient know what happens next?

Remember:

> **Draft ≠ Send.**

The agent prepared the work.

You are still responsible for the final message.

---

## Step 6 — Improve the drafts

If a draft isn't quite right, don't immediately rewrite the whole thing yourself.

Try giving Spark feedback.

For example:

```text
Make this reply shorter and more direct.

Keep the answer to the recipient's question,
but remove unnecessary explanation.

Do not change the factual information.
```

Or:

```text
The tone is too formal.

Rewrite it to sound more conversational and natural,
while keeping the same meaning.
```

Compare the revised version with the original.

---

## Step 7 — Approve only what you're happy with

Now decide what actually gets sent.

You can:

- Send a reply you have reviewed and approved.
- Continue editing a draft.
- Leave a draft for later.
- Discard a draft that isn't useful.

Do not send anything simply because Spark suggested it.

> **The agent can prepare the response. The decision to communicate is still yours.**

---

## Step 8 — Verify

After sending your approved replies, check Gmail.

Confirm:

- Only the replies you approved were sent.
- The recipients are correct.
- The final messages contain the information you intended.
- Any messages you weren't ready to send remain as drafts.

You've now completed your first repeatable agent workflow:

```text
INBOX
  ↓
PRIORITISE
  ↓
SUMMARISE
  ↓
DRAFT
  ↓
REVIEW
  ↓
APPROVE
  ↓
SEND
```

---

# 🧠 What Makes This an Automation?

Notice that we didn't simply ask:

> "What emails do I have?"

We gave Spark a **workflow**.

The same sequence can be repeated:

```text
Every time I need to process my inbox:

1. Find relevant emails.
2. Prioritise them.
3. Summarise what needs action.
4. Draft responses.
5. Let me review them.
6. Send only what I approve.
```

That's the important shift.

You're no longer asking the agent to perform a single action.

You're describing a **repeatable process**.

---

# ✅ Success Criteria

You're ready for the next lab when you can show:

- [ ] A prioritised inbox digest.
- [ ] A clear definition of what counts as urgent.
- [ ] Your own email style instruction.
- [ ] At least two reply drafts.
- [ ] Drafts reviewed for accuracy and tone.
- [ ] At least one reply approved and sent.
- [ ] Any unapproved replies remain unsent.
- [ ] You can describe the workflow Spark followed.

---

# 🧯 Troubleshooting

### Spark marked the wrong emails as urgent

Your definition of urgent is probably too vague.

Tell Spark exactly what qualifies.

For example:

```text
Only classify an email as urgent if it requires action today
or could affect a training session happening within 48 hours.
```

Then run the prioritisation again.

### The reply doesn't sound like me

Your style instruction may be too generic.

Instead of:

```text
Write professionally.
```

try:

```text
Write in short paragraphs.
Use plain English.
Get to the answer quickly.
Avoid phrases like "I hope this email finds you well."
Keep the tone warm but conversational.
```

You can also give Spark a short example of your own writing.

### The draft answered the wrong question

Tell Spark to focus on the actual request:

```text
Re-read the original email.

Identify the specific request the sender is making,
then rewrite the draft so it directly answers that request.

Do not invent information that isn't available.
```

### Spark tried to send the email

Stop and review your instructions.

Use explicit boundaries:

```text
Save as a draft only.
Do not send.
Ask for my approval before sending anything.
```

Keep approval controls enabled.

### The draft contains information you don't recognise

Don't send it.

Ask Spark where the information came from, or remove it.

For example:

```text
Identify which information in this draft came from
the original email and which came from my Workspace.

Do not change the draft yet.
```

---

# 🚀 Challenge

Let's test whether Spark can adapt its writing style.

Choose one email that needs a reply and ask for **two versions**:

```text
Draft two versions of the reply.

Version 1:
A one-line acknowledgement that confirms I received the request.

Version 2:
A complete reply that addresses the request in detail.

Use my established email style.

Save both as drafts.
Do not send anything.
```

Compare them.

### Bonus question

Which version would you actually send?

And more importantly:

> **Would you want the agent to decide which version to send automatically?**

Why or why not?

---

# 🤔 Reflection

You've just built your first repeatable agent workflow.

Think about the experience:

> **Which part of the workflow saved you the most time?**

Then consider:

> **Where did you still want human judgment?**

And finally:

> **What would make you comfortable letting this workflow run regularly without watching every single step?**

---

## 🎉 Done!

You've gone from:

**"Help me with my email."**

to:

**"Here is my inbox workflow. Prepare the work, show me what you're going to do, and let me approve the final action."**

That's the agent mindset.

Next, we're going to take the agent beyond Gmail and let it **create and work with actual Workspace content.**

# **Lab 05 — Docs, Sheets & Slides: Make Something 🚀**
