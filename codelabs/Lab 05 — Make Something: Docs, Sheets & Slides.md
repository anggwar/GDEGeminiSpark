# Lab 05 — Make Something: Docs, Sheets & Slides 📄📊📽️

> **Connected project:** In Lab 04, you built your first repeatable workflow for Gmail. Now we're going to make Spark produce actual Workspace artifacts — and make those artifacts work together.

## 🎯 Goal

Use Gemini Spark to transform information into useful Workspace content.

You'll have Spark:

- Create a Google Doc from a training brief.
- Turn unstructured information into a structured Google Sheet.
- Create a short Google Slides presentation from the same training information.
- Review and refine each output.

The key idea:

> **An agent doesn't just answer. It can turn information into work products.**

**Estimated time:** 15–20 minutes

---

## 🏫 Scenario — Build the Training Package

Your next internal training session is almost ready.

You already have the basic information:

- What the session is about.
- Who it's for.
- What participants will learn.
- What needs to happen before the session.
- Who is involved.

Now you need to turn that information into the things people actually use.

You need:

1. A **session brief** for the training team.
2. A **participant tracker** to keep the logistics organised.
3. A **short presentation** for the session.

Normally, that means creating three different files and copying information between them.

Let's see what Spark can do.

---

## 🛠️ What You'll Build

By the end of this lab, you'll have:

- A Google Doc containing a structured training session brief.
- A Google Sheet containing structured participant or session data.
- A short Google Slides presentation based on the training brief.
- At least one refinement made to each artifact.

**Tools and techniques:** Google Docs, Google Sheets, Google Slides, content generation, structured extraction, cross-application workflows, review and refinement

---

## ✅ Prerequisites

Before starting, make sure you have:

- Lab 01 complete.
- Lab 02 complete.
- Lab 03 complete.
- Lab 04 complete.
- Gemini Spark connected to Google Workspace.
- A small amount of non-confidential training information to work with.

> **Tip:** You can use your own training scenario or the workshop sample data provided by the trainer.

---

# 🚀 Steps

## Step 1 — Create the training brief

Start with the document that describes the session.

Give Spark this instruction:

```text
CONTEXT:
I am preparing an internal employee training session.

The session is called "Working Smarter with AI".

JOB:
Create a training session brief in Google Docs.

OUTPUT:
Create a 1-page document with these sections:

1. Session Overview
2. Learning Objectives
3. Preparation
4. Session Agenda
5. Follow-up

Use short paragraphs and bullet points.
Keep the document practical and easy for another coordinator
to understand.

BOUNDARIES:
Use only the information I provide or information available
in my connected Workspace.
Do not invent dates, names, or commitments.
```

Run the task.

---

## Step 2 — Review the Doc

Open the resulting Google Doc.

Check:

- Is the structure correct?
- Are the learning objectives clear?
- Is the agenda useful?
- Is anything missing?
- Did Spark invent information?

Don't immediately rewrite the document yourself.

Instead, identify **one section that could be better**.

For example:

```text
The Session Agenda section is too vague.

Rewrite it as a table with:
- Time
- Activity
- Purpose

Keep the rest of the document unchanged.
```

Review the updated version.

---

## Step 3 — Turn information into a Sheet

Now let's take information that isn't neatly structured.

Imagine you received participant information in different formats.

Use a small sample such as:

```text
Andi — Finance — attended — needs certificate
Siti — Marketing — registered — dietary preference: vegetarian
Budi — IT — attended — needs certificate
Rina — HR — cancelled
Dimas — Operations — registered — no special requirements
```

Ask Spark to turn it into structured data:

```text
Turn the participant notes below into a Google Sheet.

Use these columns in exactly this order:

Name | Department | Status | Follow-up | Notes

Keep each participant on one row.
Do not invent missing information.

Participant notes:

Andi — Finance — attended — needs certificate
Siti — Marketing — registered — dietary preference: vegetarian
Budi — IT — attended — needs certificate
Rina — HR — cancelled
Dimas — Operations — registered — no special requirements
```

Run the task.

---

## Step 4 — Check the data

Open the Google Sheet.

Check every row.

Look for:

- Names in the correct column.
- Departments in the correct column.
- Status values interpreted correctly.
- Follow-up actions captured.
- Notes preserved.

This is an important distinction.

A generated document can look convincing while still containing incorrect information.

A spreadsheet makes mistakes much easier to spot.

### If something is wrong

Don't manually fix everything.

Try improving the instruction.

For example:

```text
For the Status column, use only:
Registered, Attended, or Cancelled.

For the Follow-up column:
- Use "Certificate" when the notes say the participant needs a certificate.
- Leave blank when no follow-up is required.

Recreate the Sheet using these rules.
```

Review it again.

---

## Step 5 — Create the presentation

Now let's create something for the actual training session.

Ask Spark to use the training brief you created earlier.

```text
Create a Google Slides presentation based on my
"Working Smarter with AI" training session brief.

Create 5 slides:

1. Title
2. Why We're Here
3. Learning Objectives
4. Session Agenda
5. Takeaways

Keep each slide concise.

Use a maximum of 4 bullet points per slide.
Do not use paragraphs.

Base the content on the training brief.
Do not introduce new facts or topics.
```

Run the task.

---

## Step 6 — Review the Slides

Open the presentation.

Check each slide for:

### Content

- Does it match the training brief?
- Are the important points included?
- Did Spark introduce anything that wasn't in the source?

### Structure

- Is there too much text?
- Are the bullets actually useful?
- Does each slide have one clear purpose?

### Consistency

Compare the Slides deck with your Doc.

Ask:

> **If someone read the Doc and then opened the Slides, would they recognise the same training session?**

If not, refine the deck.

For example:

```text
The Learning Objectives slide is too wordy.

Reduce it to 3 concise bullet points.
Keep the meaning consistent with the training brief.
Do not add new objectives.
```

---

## Step 7 — Look at the bigger picture

You've now created three different Workspace artifacts:

```text
             TRAINING INFORMATION
                     │
          ┌──────────┼──────────┐
          ↓          ↓          ↓
        DOC        SHEET      SLIDES
      Session     Structured   Training
       Brief        Data      Presentation
```

But you didn't create each one completely from scratch.

You gave the agent information and asked it to transform that information into different formats.

That's one of the useful characteristics of an agent working across Workspace.

---

## Step 8 — Verify the outputs

Before you move on, check all three files.

### Google Docs

- [ ] Correct structure.
- [ ] Information is accurate.
- [ ] At least one section refined.

### Google Sheets

- [ ] Correct columns.
- [ ] Data is in the correct rows.
- [ ] No information was invented.
- [ ] At least one instruction refinement tested.

### Google Slides

- [ ] Correct number of slides.
- [ ] Content matches the training brief.
- [ ] Slides are concise.
- [ ] At least one slide refined.

---

# 🧠 The Generate → Review → Refine Loop

You've now repeated the same basic pattern across three different applications:

```text
GENERATE
   ↓
REVIEW
   ↓
FIND SOMETHING WRONG
   ↓
REFINE
   ↓
REVIEW AGAIN
```

This is an important agent habit.

Don't expect:

> **First prompt → Perfect result**

Instead:

> **First result → Review → Feedback → Better result**

The human isn't removed from the workflow.

The human becomes the **editor, reviewer, and decision-maker**.

---

# 🔗 Challenge — Keep Everything Consistent

Let's make things slightly harder.

Imagine the training session has changed.

The session is now **90 minutes instead of 60 minutes**.

Ask Spark:

```text
The "Working Smarter with AI" training session has been
extended from 60 minutes to 90 minutes.

Review the training brief and identify which parts of the
Doc and Slides may need to change.

Do not modify anything yet.

Show me the proposed changes first.
```

Review the proposal.

Notice what the agent can do:

It doesn't just create content.

It can help you reason about **what else might be affected when information changes**.

### Bonus

If you're comfortable, approve the changes and then verify the updated Doc and Slides manually.

---

# 🧯 Troubleshooting

### The Doc is too long

Be specific about the desired size.

For example:

```text
Keep the document to approximately one page.
Use short paragraphs and bullet points.
Do not add additional sections.
```

### The Sheet columns are wrong

State the exact column order and provide an example.

For example:

```text
Use exactly these columns:

Name | Department | Status | Follow-up | Notes

Do not create additional columns.
```

### Spark invented information

Tell it explicitly:

```text
Do not infer or invent missing information.

If a value is unavailable, leave it blank
and tell me which information is missing.
```

### The Slides are cluttered

Reduce the content.

Try:

```text
Keep each slide to a maximum of 4 bullet points.
Each bullet should be no more than 12 words.
Do not use paragraphs.
```

### The Slides don't match the Doc

Tell Spark what the source of truth is:

```text
Use the training brief as the source of truth.

Do not introduce information that isn't present
in the training brief.
```

---

# 🚀 Challenge — One Source, Multiple Outputs

You've already created three artifacts.

Now try to think about the workflow as a system.

Ask Spark:

```text
Review my training session brief, participant Sheet,
and Slides presentation.

Identify any inconsistencies between the three files.

Check:
- Session name
- Learning objectives
- Agenda
- Participant information
- Dates or times

Do not modify anything.

Return a list of inconsistencies only.
```

This time, you're not asking Spark to **create** something.

You're asking it to **review multiple sources and find relationships between them**.

That's another step toward agentic work.

---

# 🤔 Reflection

You've now used Spark to create and refine multiple Workspace artifacts.

Think about the experience:

> **Which output benefited most from using an agent — the Doc, Sheet, or Slides? Why?**

Then consider:

> **Where did you still need human judgment?**

And finally:

> **If the source information changes, how much work would you normally need to do to update all three outputs manually?**

---

## 🎉 Done!

You've gone from:

**One prompt → One answer**

to:

**Information → Multiple artifacts → Review → Refinement**

Your agent can now work across your Workspace instead of living inside a single chat window.

But there's still a problem.

You've created some really useful instructions.

What if you could **teach Spark one of those workflows once and reuse it whenever you need it?**

That's next.

# **Lab 06 — Build Your Own Skill 🧠✨**
