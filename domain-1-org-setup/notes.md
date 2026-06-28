# Domain 1: Configuration & Setup (20%)

> Source: Udemy — *Salesforce Admin Exam* by Francis Pindar
> Status: In progress

---

## Classic UI vs Lightning UI

- It's better to know **both** Classic UI and Lightning UI — the underlying data is the same in both; it's just a different visualization of the same data.
- Some features are only available in their respective version (Classic-only or Lightning-only features exist).
- **Lightning Dashboards cannot be viewed in Classic**, but Classic dashboards/reports *can* be viewed in Lightning.

### Quick comparison

| | Classic UI | Lightning UI |
|---|---|---|
| Data | Same underlying data | Same underlying data |
| Dashboards | Visible in Lightning ✅ | **Not** visible in Classic ❌ |
| Feature availability | Some features Classic-only | Some features Lightning-only |

---

## Salesforce Branding & UI Customization

**Key question: What can you customize?**

### As a User
- Density Settings
- Top Navigation Bar
- Chatter Branding

### As an Administrator / Developer
- Default Density Settings
- Org-wide Themes & Branding
- Report & Chart Picklist Colors
- App & Navigation Layouts
- Record Page Layouts
- My Domain
- Email Templates
- Mobile Branding

---

## Density Settings

- As an admin, the **Search setup** bar appears when you get to **Density Setting** in the user interface.
- The user can change the **density** by choosing the default setting for users, or users can customize it for themselves in their own personal settings.
- The user can also change the **Profile icon** from the top-right corner — compact.

### Comfy vs Compact
- You can only have **one theme active** at a time (can't run two themes simultaneously).
- This default setting applies to the **entire Salesforce org**.

---

## Themes & Branding (Setup)

**Path:** Setup → Themes and Branding

- This is where you set **org-wide** themes and branding — it affects **all users**, not just the admin.
- These brands don't work on **mobile** — they're a **desktop-only** customization.

### Custom Themes
- Salesforce orgs that use **multiple default options for themes** can also add their own **custom theme**.
- With **Salesforce Themes** (premium), you only have access to **see** the default theme — you don't get to **change** the **default theme** to a **custom one** unless you have the right license.
- If you are using your own **Lightning Experience** licence for your user, **Now you can use the Chatter setting** in the **Salesforce Setup** — but the entire **Salesforce Org** Themes won't change for everyone, only for your own view.

### Chatter Branding
- You are using the **Chatter** external — it has a **logo** and a **standard theme**.
- **With** the **standard theme**, we get a **default option** for the Chatter logo, and **you can** change your own **login page** instead.

---

## Lightning Chrome Extension

- This is the extension Salesforce created as a way of **testing different UI features on users**.
- This can be done through the **Setup menu**.

### Topics covered (User vs Admin/Dev)

| Topic | Who |
|---|---|
| Density Setting | User & Admin |
| Top Navigation Bar | User |
| Lightning Chrome Extension | User |
| Default Density Settings | Admin / Dev |
| Org-wide Themes & Branding | Admin / Dev |

---

## Salesforce Background (Quick Facts)

- Salesforce was founded on **March 8, 1999** by **Marc Benioff, Parker Harris, Dave Moellenhoff, and Frank Dominguez**.
- Current CEO: **Marc Benioff**
- Current CTO: **Parker Harris**
- **2015** — Salesforce **Lightning** was launched.

### Salesforce User Types (Interface)

| Lightning UI | Mobile / Tab | Classic UI |
|---|---|---|
| Lightning Features | Common Features | Classic Features |

**Core platform layers:**
1. Business Processes & Tooling
2. Database

---

## Notes / Things to revisit
- [ ] Need clearer distinction between org-wide Theme settings vs per-user Chatter branding — notes got a little tangled here, worth re-checking on Trailhead.
- [ ] My Domain — need dedicated notes (currently just listed as a topic, no detail yet).
