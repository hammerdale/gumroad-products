# Sales Pipeline Manager
## Complete Notion Template Guide

---

# Getting Started

Welcome! This guide walks you through building your Sales Pipeline Manager in Notion — completely free.

**What you need:**
- A free Notion account (notion.so)
- This guide (you're reading it)
- About 20 minutes

---

# Step 1: Create Your Notion Account

1. Go to **notion.so**
2. Click **"Sign up"**
3. Enter your email or use Google/Apple login
4. Verify your email

That's it — free account ready.

---

# Step 2: Create the Main Page

1. In Notion, click **"+"** in the sidebar
2. Select **"Page"** (or press `/` and type "Page")
3. Name it: **"Sales Pipeline Manager"**

---

# Step 3: Create the Leads Database

1. On your page, type `/` and type **"Database - Inline"**
2. Click it — you'll see a table appear
3. Rename the database: **"Leads"**

**Add these columns (properties):**
- **Name** → Title (default)
- **Email** → Email
- **Phone** → Phone Number  
- **Company** → Text
- **Lead Source** → Select (options: Referral, Cold Outreach, Ads, Website, Other)
- **Status** → Select (options: New, Contacted, Qualified, Proposal Sent, Won, Lost)
- **Estimated Value** → Number → Currency ($)
- **Notes** → Text
- **Created Date** → Created time

**How to add properties:**
- Click the **"+"** next to column headers
- Select the property type
- Configure options

---

# Step 4: Create the Deals Database

1. Type `/` and type **"Database - Full page"**
2. Name it **"Deals"**

**Properties:**
- **Deal Name** → Title
- **Lead** → Relation (link to Leads database)
- **Client** → Relation (we'll create this later)
- **Value** → Number → Currency
- **Stage** → Select (Discovery, Demo, Proposal, Negotiation, Closed Won, Closed Lost)
- **Probability** → Number → %
- **Expected Close** → Date
- **Next Action** → Text
- **Notes** → Text
- **Created** → Created time

---

# Step 5: Create the Clients Database

1. Create another database full page
2. Name it **"Clients"**

**Properties:**
- **Name** → Title
- **Email** → Email
- **Company** → Text
- **Phone** → Phone Number
- **Total Revenue** → Number → Currency (formula: sum of all deals with this client that are "Closed Won")
- **First Purchase** → Date
- **Notes** → Text

*Tip: To link closed deals to clients, go to your Deals database and change the "Client" property to show deals that are "Closed Won".*

---

# Step 6: Create Follow-ups Database

1. Create a new database → name it **"Follow-ups"**

**Properties:**
- **Task** → Title
- **Related Lead/Deal** → Relation (link to both Leads and Deals)
- **Due Date** → Date
- **Type** → Select (Call, Email, Meeting, Other)
- **Status** → Select (Pending, Done, Snoozed)
- **Notes** → Text

---

# Step 7: Create the Dashboard

Go back to your main **Sales Pipeline Manager** page:

1. Create a **"Board"** view of your Deals database (click "Add a view" → Board)
2. Create a **"Gallery"** view of your Leads database
3. Add these **formula blocks** for metrics:

**Total Pipeline Value:**
```
prop("Value")
```

**Won Deals Total:**
```
filter(prop("Stage") == "Closed Won").sum(prop("Value"))
```

**Lead Count:**
```
length(filter(prop("Status") != "Lost"))
```

---

# Step 8: Add Email Templates Section

On your main page, create a new section called **"Scripts & Resources"**:

1. Click **"+"** → select **"Callout"** or **"Toggle"**
2. Label it **"Email Templates"**
3. Inside, add these content blocks:

**Follow-up Email:**
```
Subject: Following up on [topic]

Hi [Name],

I wanted to follow up on our last conversation about [topic].

[Insert personalized detail from your notes]

Are you available for a quick call this week? 

Best,
[Your Name]
```

**Proposal Email:**
```
Subject: Proposal for [Service]

Hi [Name],

Based on our discussion, I've put together a proposal for [service].

[Link to proposal or attach PDF]

Let me know if you have any questions!

Best,
[Your Name]
```

---

# Step 9: Make It Public

1. Click the **"Share"** button in the top right
2. Click **"Invite"**
3. Change to **"Share to web"**
4. Toggle **"Share to web"** ON
5. **Copy the link** — this is your template link!

**This is the link you give Gumroad buyers.**

---

# Quick Reference: Database Properties Summary

## Leads Database
| Property | Type | Options |
|----------|------|---------|
| Name | Title | — |
| Email | Email | — |
| Phone | Phone | — |
| Company | Text | — |
| Lead Source | Select | Referral, Cold Outreach, Ads, Website, Other |
| Status | Select | New, Contacted, Qualified, Proposal Sent, Won, Lost |
| Estimated Value | Number | Currency |
| Notes | Text | — |

## Deals Database
| Property | Type | Options |
|----------|------|---------|
| Deal Name | Title | — |
| Lead | Relation | → Leads |
| Client | Relation | → Clients |
| Value | Number | Currency |
| Stage | Select | Discovery, Demo, Proposal, Negotiation, Closed Won, Closed Lost |
| Probability | Number | % |
| Expected Close | Date | — |
| Next Action | Text | — |
| Notes | Text | — |

## Clients Database
| Property | Type | Options |
|----------|------|---------|
| Name | Title | — |
| Email | Email | — |
| Company | Text | — |
| Phone | Phone | — |
| Total Revenue | Formula | — |
| Notes | Text | — |

## Follow-ups Database
| Property | Type | Options |
|----------|------|---------|
| Task | Title | — |
| Related Lead/Deal | Relation | → Leads, Deals |
| Due Date | Date | — |
| Type | Select | Call, Email, Meeting, Other |
| Status | Select | Pending, Done, Snoozed |
| Notes | Text | — |

---

# Troubleshooting

**Q: I don't see the property options**
A: Click on the property name → select "Edit property" → you can change the type or options there.

**Q: How do I link a deal to a lead?**
A: In the Deals database, find the "Lead" property and click → select the lead from your Leads database.

**Q: Can I change property types later?**
A: Some yes, some no. It's easier to delete and recreate than to change types.

---

# You're Ready!

Now you have a fully functional Sales Pipeline Manager in Notion. Share the public link with your Gumroad buyers and they're all set.

**For Gumroad buyers:**
Simply share your template link and they'll duplicate it into their own Notion account for free.

---

*Template by Dale's Products*  
*Questions? Reach out through Gumroad*