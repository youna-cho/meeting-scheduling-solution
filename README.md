# Meeting Scheduling Recommendation Product

A meeting scheduling product that recommends suitable meeting times by combining participant availability, preferred times, and priority.

**[View Live Demo →](https://meeting-scheduling-prod.netlify.app/)**

---

## Overview

- **Role:** Product Manager / Product Designer
- **Type:** Solo Project
- **Period:** Jul 2026
- **Output:** Functional web prototype
- **Tools:** Figma · Claude Design · Claude Code · Netlify

---

## Problem

Most scheduling tools focus on when participants are available.

However, a time someone **can attend** is not always the time they **prefer**, and some participants may be more important to the meeting than others.

---

## Research

- Analyzed **4 meeting scheduling products across 5 criteria**
- Conducted **5 user interviews** with organizers and participants

The research highlighted the need to distinguish **availability from preference**.

---

## Key Insight

### Availability ≠ Preference

Participants can indicate whether each time is:

- **Preferred**
- **Available**
- **Unavailable / Unmarked**

This allows the organizer to understand not only when people can attend, but which times work better for them.

---

## Product Approach

The recommendation combines:

### Participant Priority
- Required participant: weight **2**
- Optional participant: weight **1**

### Time Preference
- Preferred: score **1**
- Available: score **0.5**
- Unavailable / Unmarked: score **0**

The product compares candidate times using both participant priority and preference.

---

## Key Product Decisions

### 1. Separate Available and Preferred
Availability and preference are collected separately so all available times are not treated equally.

### 2. Distinguish Required and Optional Participants
Required participants receive greater weight when comparing meeting times.

### 3. Recommend, Not Automatically Decide
The product recommends stronger options while keeping the final decision with the organizer.

### 4. Provide Fallback Options
When no time works perfectly for everyone, the product surfaces the strongest alternatives.

---

## User Flow

**Organizer**

Create Meeting → Add Participants → Set Required / Optional → Add Candidate Times → Share Link → Review Responses → Check Recommendations → Confirm Meeting

**Participant**

Open Link → Review Candidate Times → Mark Preferred / Available / Unavailable → Submit

---

## Prototype

The high-fidelity design was developed into a functional web prototype.

**[Open Live Prototype →](https://meeting-scheduling-prod.netlify.app/)**

---

## Limitations

- User interviews were conducted with **5 participants**
- Recommendation weights are rule-based and require further validation
- The prototype has not yet been evaluated with large-scale behavioral data

---

## Next Steps

- Conduct usability testing with more users
- Measure recommendation acceptance rate
- Analyze when organizers override recommendations
- Refine recommendation weights based on real usage

---

## Live Demo

**[Try the Meeting Scheduling Recommendation Product →](https://meeting-scheduling-prod.netlify.app/)**
