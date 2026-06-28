# Domain 2: Object Manager & Lightning App Builder (20%)

> Source: Trailhead
> Confidence: 4/5
> Status: Core concepts covered — Standard/Custom Objects, Object Relationships, Schema Builder (in progress)

---

## Optimize Customer Data with Standard & Custom Objects

Custom objects can be used to create objects to optimize business needs as per its nature and needs.

### Start with the Data Model

In Salesforce CRM, think of **Objects** the way you'd think of a database table:
- **Object** = a table
- **Fields** = columns
- **Records** = rows

So instead of an Account spreadsheet or a table, you have an **Account Object** with fields, and a bunch of identically structured records.

### Types of Objects

- Standard Objects
- Custom Objects
- External Objects
- Platform Events
- Big Objects

### Standard vs Custom Objects

**Standard Objects** are objects that come built-in with Salesforce. Common business objects like **Accounts, Contacts, Leads, and Opportunities** are all standard objects.

**Custom Objects** are objects you create to store information specific to your company or industry.

> Objects are containers for your information, but they also give you special functionality.
>
> **Example:** When you create a custom object, the platform automatically builds things like the page layout for the user interface.

---

## Daily Dose of Salesforce CRM (Quick Reference)

- **Account** → a Company
- **Contact** → a Person (a contact you have to communicate with, related to the deal)

**When it's B2B:**
- The Account is created in the company's name
- The Contact is the point of contact (a person)

### List Views
- You can access **Kanban view** to simply drag and drop opportunity stages — easy to move deals from one stage to another.

### Reports and Dashboards
- (To expand further as covered)

---

## Object Relationships

### Lookup Relationship
- A **loose link** between two objects — each is independent.
- Custom objects = built using **one or more** Lookup or Master-Detail relationships, plus your org's specific needs.
- Standard objects = built-in (e.g. Account, Contact).

### Master-Detail Relationship
- A **tight link** between two objects.
- **Parent → Child**: Delete the parent → child is also deleted (it doesn't survive on its own).
- Child inherits the **parent's sharing/security settings** too.

### Lookup vs Master-Detail — Quick Test

| | Master-Detail | Lookup |
|---|---|---|
| Delete parent | Child is **deleted** (cascade delete) | Child **survives** — the lookup field just goes empty |
| Existence | Child depends on parent | Child exists independently |
| Sharing | Child inherits parent's sharing | Child has its own sharing rules |

**Quick test:** *"Can the child exist on its own?"*
- **Yes** → Lookup
- **No** → Master-Detail

### Why might you choose Lookup over Master-Detail even when there's a clear "parent-child" feel to the data?
- You need the child to **survive** when the parent gets deleted.
- You need **independent sharing rules** (child shouldn't automatically inherit the parent's visibility).

---

## Q&A Self-Check (from notes)

**Q1. What's the core difference between a Standard Object and a Custom Object?**
A. Standard Objects are Salesforce's built-in objects (e.g. Account, Contact). Custom Objects are ones you build for your own org's specific needs.

**Q2. Name two Salesforce standard object types and give one example use of each.**
A. *(Account → tracks a company; Contact → tracks a person at that company)*

**Q3. Name the two main relationship types in Salesforce and briefly describe each.**
A.
1. **Lookup Relationship** — Loose link. Two objects, each independent of each other.
2. **Master-Detail Relationship** — Tight link. Child has no meaning/existence without a parent. Delete parent → child deleted too; child inherits parent's sharing/security settings.

**Q4. What happens to child records when:**
- a Master-Detail parent record is deleted → **Child records are deleted too** (cascade delete).
- a Lookup parent record is deleted → **Child records survive**; the lookup field on the child just goes empty.

**Q5. Why might you choose a Lookup relationship over Master-Detail even when there's a clear "parent-child" feel to the data?**
A. When you need the child to survive even if the parent is deleted, or when you need independent sharing rules (i.e. the child shouldn't automatically inherit the parent's visibility settings).

---

## Notes / Things to revisit
- [ ] Schema Builder — marked "in progress," need to come back and add visual/hands-on notes once covered.
- [ ] Add notes on Hierarchical and Many-to-Many (junction object) relationship types — only Lookup and Master-Detail covered so far.
