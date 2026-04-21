# facilitron-tickets

Internal tools and resources for the Facilitron Tickets white-label platform (built on VBO Tickets).

https://bbaldocchi.github.io/facilitron-tickets/

---

## What is in this repo

| File | Description |
|------|-------------|
| `facilitron-master-template-qa.html` | Interactive QA checklist for regression testing the master template |
| `facilitron-master-template-qa.css` | Stylesheet companion to the QA checklist |

More files will be added as the intern project progresses, including the master template files themselves (header.html, footer.html, styles.css, ticket.html).

---

## QA Checklist

The QA checklist is a standalone HTML tool an intern or team member can open in any browser to run a regression test against the master template after changes are made.

**Live URL:** https://bbaldocchi.github.io/facilitron-tickets/facilitron-master-template-qa.html

### What it covers

- Brand and colors (logo, CSS variables, Facilitron palette)
- Header (icons, cart, sticky behavior, mobile hamburger)
- Hero banner (background, overlay, responsive text)
- Filter bar and toolbar
- Event cards (grid, hover, sold-out state)
- Event detail page (two-column layout, ticket selector)
- Footer and powered-by banner
- Mobile ticket template (ticket.html)
- Responsive breakpoints (375px through 1440px)
- CSS health (no special characters, no @import, file size)
- VBO integration (proxy URL, admin field saves)

### How to use it

1. Open the live URL above in a browser
2. Fill in your name, the client instance, date, and template version at the top
3. Work through each section -- click P (pass), F (fail), or N/A for each item
4. Add notes in the notes field for anything that needs follow-up
5. Click Export Report when done -- downloads a plain text summary you can share

Progress saves automatically to your browser between sessions.

### How to log a bug

If you find a failure during QA, open a GitHub Issue in this repo:

1. Click the Issues tab at the top of this page
2. Click New Issue
3. Title it: [QA] Brief description of the problem
4. In the body, paste the relevant line from your exported report and add steps to reproduce
5. Assign it to the appropriate person and add the label `bug`

---

## Platform Notes

- The ticketing platform is VBO Tickets, white-labeled as Facilitron Tickets
- All front-end customization goes through two fields in the VBO admin: Custom Header HTML and Custom CSS
- The CSS field has a byte size limit -- always verify the file saves without error after edits
- No @import statements in CSS (VBO blocks them) -- fonts load via link tag in the HTML field or fall back to Arial
- No special characters in any file (no em dashes, smart quotes, curly apostrophes) -- plain ASCII only

---

## Contacts

For questions about the platform or this repo, reach out to the Facilitron Tickets team on Slack.
