# Content Marketing Workflow
## Complete Notion Template Guide

---

# Getting Started

Welcome! This guide walks you through building your Content Marketing Workflow in Notion — completely free.

**What you need:**
- A free Notion account (notion.so)
- This guide (you're reading it)
- About 25 minutes

---

# Step 1: Create Your Notion Account

1. Go to **notion.so**
2. Click **"Sign up"**
3. Enter your email or use Google/Apple login
4. Verify your email

---

# Step 2: Create the Main Page

1. In Notion, click **"+"** in the sidebar
2. Select **"Page"**
3. Name it: **"Content Marketing Workflow"**

---

# Step 3: Create the Ideas Database

1. On your page, type `/` and type **"Database - Inline"**
2. Rename it: **"Ideas Bank"**

**Properties:**
- **Idea** → Title
- **Source** → Select (Brainstorm, Competitor, Audience Request, Trending, Other)
- **Category** → Multi-select (Educational, Entertaining, Promotional, Behind-the-scenes)
- **Platform** → Multi-select (YouTube, TikTok, Instagram, Blog, Newsletter, Podcast)
- **Status** → Select (Saved, In Progress, Scheduled, Published)
- **Priority** → Select (High, Medium, Low)
- **Notes** → Text
- **Research Links** → URL
- **Created** → Created time

---

# Step 4: Create the Calendar Database

1. Type `/` → **"Database - Full page"**
2. Name it **"Content Calendar"**

**Properties:**
- **Content Title** → Title
- **Platform** → Multi-select (YouTube, TikTok, Instagram, Blog, Newsletter, Podcast)
- **Type** → Select (Video, Post, Article, Email, Reel, Story, Newsletter)
- **Status** → Select (Idea, Researching, Writing, Recording, Editing, Scheduled, Published)
- **Publish Date** → Date
- **Publish Time** → Text
- **Assigned To** → Person (for teams)
- **Assets Needed** → Text
- **Thumbnail** → File
- **Link** → URL
- **Notes** → Text

**Create these Views:**
- **Calendar View** → Group by "Publish Date"
- **Board View** → Group by "Status"
- **Gallery View** → Filter by Platform

---

# Step 5: Create the Research Database

1. Create a new database → name it **"Research Library"**

**Properties:**
- **Topic** → Title
- **Type** → Select (Competitor Analysis, Trending Topic, Pain Point, Keyword Cluster)
- **Source** → URL
- **Notes** → Text
- **Tags** → Multi-select

---

# Step 6: Create the Analytics Database

1. Create a new database → name it **"Analytics Tracker"**

**Properties:**
- **Platform** → Select (YouTube, TikTok, Instagram, Blog, Newsletter)
- **Metric** → Select (Views, Likes, Comments, Shares, Clicks, Subscribers)
- **Value** → Number
- **Date** → Date
- **Notes** → Text

---

# Step 7: Create Your Dashboard

On your main **Content Marketing Workflow** page:

1. Add a **Gallery view** of the Ideas Bank (click "Add a view" → Gallery)
2. Add a **Calendar view** of the Content Calendar
3. Add a **Board view** of the Content Calendar grouped by Status

**Add callouts with quick stats:**
- Count of ideas: `length(database("Ideas Bank"))`
- Scheduled this month: `filter(prop("Status") == "Scheduled").length()`
- Published: `filter(prop("Status") == "Published").length()`

---

# Step 8: Add Platform Guidelines

On your main page, create sections for each platform:

## YouTube Best Practices
- **Posting times:** Thursday-Saturday, 3PM-6PM EST
- **Titles:** How-to + result | [Number] ways to [benefit]
- **Thumbnails:** Bold text, bright colors, face expression
- **Description:** First 3 lines are key, include timestamps
- **Hashtags:** #Shorts #Topic #Niche

## TikTok Best Practices
- **Posting times:** Daily, 6AM-10AM and 7PM-11PM
- **Hooks:** First 3 seconds must grab attention
- **Audio:** Use trending sounds + original
- **Captions:** Include for scroll-without-sound
- **Hashtags:** #fyp #ForYou #Topic

## Instagram Best Practices
- **Posting times:** Daily, 11AM-1PM and 7PM-9PM
- **Carousels:** 10 slides max, educational first
- **Reels:** Use trending audio, 15-30 seconds
- **Stories:** Daily engagement, use polls/quizzes
- **Hashtags:** 3-5 relevant, 1 niche

## Blog Best Practices
- **Posting frequency:** 2x/week minimum
- **Structure:** H2s every 300 words, intro < 150 words
- **SEO:** Target keyword in title, first 100 words, H2s
- **CTA:** 1-2 relevant links to your offer

---

# Step 9: Add Production Checklist

Create a template page for content pieces:

1. Type `/` → **"Template button"**
2. Name it **"Content Piece"**
3. Add these checkboxes:
   - [ ] Topic approved
   - [ ] Research complete
   - [ ] Outline done
   - [ ] First draft complete
   - [ ] Review/edits done
   - [ ] Assets gathered
   - [ ] Scheduled
   - [ ] Published
   - [ ] Analytics checked

---

# Step 10: Make It Public

1. Click **"Share"** in the top right
2. Toggle **"Share to web"** ON
3. **Copy the link** — this is your template link!

**This is the link you give Gumroad buyers.**

---

# Quick Reference: Database Properties Summary

## Ideas Bank
| Property | Type | Options |
|----------|------|---------|
| Idea | Title | — |
| Source | Select | Brainstorm, Competitor, Audience Request, Trending, Other |
| Category | Multi-select | Educational, Entertaining, Promotional, Behind-the-scenes |
| Platform | Multi-select | YouTube, TikTok, Instagram, Blog, Newsletter, Podcast |
| Status | Select | Saved, In Progress, Scheduled, Published |
| Priority | Select | High, Medium, Low |
| Notes | Text | — |
| Research Links | URL | — |

## Content Calendar
| Property | Type | Options |
|----------|------|---------|
| Content Title | Title | — |
| Platform | Multi-select | YouTube, TikTok, Instagram, Blog, Newsletter, Podcast |
| Type | Select | Video, Post, Article, Email, Reel, Story |
| Status | Select | Idea, Researching, Writing, Recording, Editing, Scheduled, Published |
| Publish Date | Date | — |
| Publish Time | Text | — |
| Assets Needed | Text | — |
| Link | URL | — |

## Research Library
| Property | Type | Options |
|----------|------|---------|
| Topic | Title | — |
| Type | Select | Competitor Analysis, Trending Topic, Pain Point |
| Source | URL | — |
| Notes | Text | — |

## Analytics Tracker
| Property | Type | Options |
|----------|------|---------|
| Platform | Select | YouTube, TikTok, Instagram, Blog |
| Metric | Select | Views, Likes, Comments, Shares, Clicks |
| Value | Number | — |
| Date | Date | — |

---

# Workflow: How to Use This System

## Weekly Routine:
1. **Monday:** Review Ideas Bank, schedule 5-7 for the week
2. **Tuesday-Thursday:** Work through production pipeline
3. **Friday:** Schedule content for next week, check analytics

## Content Creation Flow:
1. Add idea to Ideas Bank
2. Move to Calendar → set publish date
3. Progress through Status: Researching → Writing → Editing → Scheduled
4. Mark Published → log in Analytics

---

# Troubleshooting

**Q: How do I add platforms to the multi-select?**
A: Click on the platform property → "Edit property" → add options in the list.

**Q: Can I track multiple platforms for one content piece?**
A: Yes — "Platform" is multi-select, so you can check multiple platforms for one piece.

**Q: How do I see what's due this week?**
A: Create a Calendar view of the Content Calendar, filter by "Publish Date" is within next 7 days.

---

# You're Ready!

Now you have a complete Content Marketing Workflow system. Share the public link with your Gumroad buyers and they're all set.

**For Gumroad buyers:**
Simply share your template link and they'll duplicate it into their own Notion account for free.

---

*Template by Dale's Products*  
*Questions? Reach out through Gumroad*