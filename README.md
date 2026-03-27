# 📟 SCSS6027_FIREBASE_SYSTEM

### [ SYSTEM_ID: TICKET_MANAGEMENT_CONSOLE ]
This repository is the independent successor to the Firebase-hosted Ticket database for SCSS6027. It provides a secure, retro-terminal interface for managing system alerts and user communications.

---

### 📂 DATABASE_INDEX
- **Primary Data:** `/database/tickets.json`
- **Schema Fields:** 
  - `TicketNumber` (Integer)
  - `Name` (String)
  - `EmailAddress` (String)
  - `Description` (String)
  - `Status` (Open/Closed/Pending)
  - `Created` (ISO-Timestamp)
  - `Updated` (ISO-Timestamp)

---

### ⌨️ SYSTEM_COMMANDS (TMS_SPECIFIC)
| Command | Action |
|:--- |:--- |
| `ls` | List all tickets (Overview mode). |
| `cat [id]` | Display full description of a specific ticket. |
| `status [id] [new_status]` | Update a ticket from "Open" to "Closed". |
| `search [email]` | Find all tickets linked to a specific user. |
| `new` | Initiate a new ticket entry sequence. |

---

### 🛠 LOG_ENTRY
- **2026-03-22:** System migration from Google Cloud to SCSS6027/FIREBASE initiated.
- **2026-03-22:** Schema defined based on legacy Firestore records (Ref: Duck Grobbelaar).
- **STATUS:** INITIALIZING DATABASE...
