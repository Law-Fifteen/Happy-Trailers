# Happy Trailers Field Guide LMS
## Product Design & Development Framework (v1.0)

---

# Vision

The Happy Trailers Field Guide is **not** intended to be an eLearning platform.

It is intended to become a **guided field companion** that teaches salespeople and managers *how experienced operators think.*

The learning philosophy is based on four principles:

- Learn in small pieces.
- Learn by doing.
- Understand *why*, not just *what*.
- Make it extremely easy to revisit information later.

Think less:

> "Corporate LMS"

Think more:

> "Interactive Field Handbook"

---

# Primary Goals

The application should:

- feel premium
- launch instantly
- work offline
- require zero installation
- be portable
- remain a single HTML file

---

# Design Language

## Theme

Modern Industrial

Premium

Minimal

Professional

---

## Colors

Primary Background

```
#241E20
```

Primary Accent

```
#D71920
```

Secondary Background

```
#2E282A
```

Completed Accent

```
Soft Green
#5FB878
```

Light Mode Background

```
#E6E6E6
```

Glass Panels

```
rgba(255,255,255,.08)
backdrop-filter: blur(18px)
```

---

## Visual Style

- Glassmorphism
- Rounded corners (16-20px)
- Soft shadows
- Frosted panels
- Animated gradients
- Subtle bokeh background
- Smooth transitions
- Zero harsh edges

Everything should feel:

> Calm
>
> Premium
>
> Organized

---

# Startup Experience

## Initial Launch

Display only:

Centered Happy Trailers Logo
https://www.happytrailers.com/wp-content/uploads/2025/03/Happy-Trailers-logo.webp

Background:

```
#E6E6E6
```

Logo fades in.

After approximately 1.5 seconds:

Login panel fades upward.

---

# Login Window

Centered Card

Contains:

Username

Password

Request Access

Login

---

Request Access

Launches

```
mailto:MorganAmbrose@proton.me
```

---

Successful Login

Transition

Fade

Background changes

Light

↓

Dark Theme

Sidebar slides in.

Dashboard loads.

---

# Authentication

Current version

Three local users.

Later versions

Authentication API

JWT

OAuth

etc.

The current credential implementation should only serve as a placeholder during development. It should be replaceable with a proper authentication provider without changing the surrounding UI or application flow.

---

# Main Layout

```
┌─────────────────────────────────────────────────────────┐
│ Header                                                  │
├────────────┬────────────────────────────────────────────┤
│            │                                            │
│ Sidebar    │               Content                      │
│            │                                            │
│            │                                            │
│            │                                            │
│            │                                            │
└────────────┴────────────────────────────────────────────┘
```

Sidebar

≈280px

Scrollable

Invisible Scroll Bars

Content

Fluid

Responsive

---

# Header

Contains

Logo

Search

Progress %

Theme Toggle

Profile

---

# Sidebar Structure

```
Dashboard

Chapter 1

Chapter 2

Chapter 3

Chapter 4
    ICP
        Residential
            Buying Motivations
            Discovery
            ...
        Contractor
        Agriculture
        ...

Chapter 5

Chapter 6
    Discovery
    Qualification
    Presentation
    Closing
    ...

Chapter 7

Chapter 8

Chapter 9

Chapter 10

Chapter 11

Chapter 12

──────────────

Ideal Customer Profiles

Case Studies

Common Mistakes

Common Objections

If This Then That

What Great Reps Notice

Key Takeaways

Manager Coaching Guide
```

Expandable.

Infinite nesting.

---

# Navigation

Each section becomes a "learning card."

Cards display

Title

Reading Time

Completion

Navigation

```
← Previous

Next →
```

Keyboard shortcuts

Left Arrow

Right Arrow

Space

---

# Learning Philosophy

Never overwhelm.

Each page teaches

ONE concept.

Example

NOT

```
Discovery
Qualification
Presentation
Closing
```

Instead

```
Discovery

↓

One page

↓

Discovery Questions

↓

One page

↓

Common Mistakes

↓

One page

↓

Great Reps Notice

↓

One page
```

---

# Learning Card Structure

Every concept follows

```
Concept

↓

Explanation

↓

Why It Matters

↓

Example

↓

Common Mistakes

↓

What Great Reps Notice

↓

Key Takeaway
```

Every page feels complete.

---

# Progress Tracking

Completion tracked

Per page

Per subsection

Per chapter

Entire handbook

Completed

Soft green outline

Sidebar checkmark

Dashboard updates

---

# Dashboard

Not simply

"Resume"

Instead

A living homepage.

---

Hero

Continue Learning

```
Resume Chapter 4.2

Continue →
```

---

Below

Insight Carousel

Rotating cards

Examples

```
Common Mistake

↓

Discovery isn't interrogation...
```

---

Another

```
Great Reps Notice

↓

Contractors rarely discuss
future growth...
```

---

Another

```
If This...

↓

Customer says...

↓

Then...
```

---

Only completed content appears.

---

# Knowledge Library

Separate from progression.

Sidebar items

Always searchable.

Contains

All

Common Mistakes

All

Case Studies

All

Objections

etc.

Regardless of chapter.

Acts like

Knowledge Base

---

# Search

Global

Instant

Searches

Headings

Keywords

Objections

ICP

Examples

Manager Notes

Returns

Matching cards.

---

# Smart Tags

Every page receives metadata.

Example

```
Chapter

ICP

Sales

Discovery

Contractor

Commercial

Objection

Service

Manager

Leadership
```

Allows

Dynamic filtering.

---

# Arrow Rendering

Whenever handbook contains

```
↓

→

←

⇒
```

Convert

Into

Animated flow diagrams.

Example

```
Discovery

↓

Qualification

↓

Presentation

↓

Close
```

Should render

Visually.

Not as plain text.

---

# Interactive Components

Expandable Callouts

```
Why?

▼
```

Click

Expands explanation.

---

Decision Trees

```
Customer Says...

↓

Choose Response

↓

Outcome
```

---

Process Maps

```
Lead

↓

Discovery

↓

Recommendation

↓

Close

↓

Service
```

Animated.

---

Comparison Tables

```
Weak Rep

vs

Great Rep
```

---

# Section Types

The renderer should recognize

Automatically

Concept

Checklist

Framework

Decision Tree

Flowchart

Callout

Table

Quote

Case Study

Warning

Tip

Manager Coaching

Key Takeaway

without manual HTML.

Markdown should drive rendering.

---

# Manager Mode (Future)

Hidden toggle

Adds

Manager Notes

Coaching prompts

Observation checklists

Roleplay exercises

Hiring notes

---

# Light/Dark Mode

Toggle

Instant transition.

Remember preference.

---

# Animations

Small.

Fast.

Professional.

Examples

Sidebar

Slides.

Cards

Fade.

Dropdowns

Smooth.

Hover

Soft elevation.

Completion

Green pulse.

Nothing flashy.

---

# Accessibility

Keyboard navigation

Responsive typography

Adjustable font size

Reduced motion support

High contrast compatibility

---

# Future Features (Roadmap)

## Phase 2

- Notes per page
- Highlighting
- Bookmark pages
- Favorite insights
- Recently viewed

---

## Phase 3

- Interactive quizzes
- Scenario simulations
- Manager assignments
- Coaching reviews

---

## Phase 4

- Multi-company support
- Downloadable playbooks
- Analytics dashboard
- User profiles
- Sync across devices

---

# Technical Architecture

## Rendering Engine

Markdown-first.

Every lesson begins as Markdown.

Renderer transforms into interactive cards.

------

# Overall Experience Goal

The application should feel like a hybrid of:

- Apple Human Interface Guidelines
- Notion
- Linear
- Arc Browser
- Obsidian

It should never resemble a traditional corporate LMS.

Instead, it should feel like a modern operating system for learning—a tool that an experienced salesperson or manager wants to keep open throughout the day because it makes them more effective in real customer conversations.