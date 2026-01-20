## Aircraft Vault – App Flow, Pages & Roles

### 🗺️ Site Map (Top-Level Pages)

- `/login` – Login / access screen
- `/vault` – Main dashboard (My Aircraft Vault)
- `/upload` – File picker / drag-drop interface (modal or inline)
- `/share/:id` – Public view-only share page
- `/settings` – Optional (user or Vault Copilot settings)

---

### 🎯 Purpose of Each Page

- **Login**: Authenticate securely and land directly in the vault
- **Vault Dashboard**: Show aircraft folders + files with upload options
- **Upload Modal**: Drop/upload files, assign to folders
- **Share View**: Clean, read-only interface for viewers—no login needed
- **Settings**: Manage sharing defaults, enable/disable Copilot AI

---

### 👥 User Roles & Access Levels

#### 1. **Owner**
- Full access: upload, edit, delete, share
- Manages folders, files, and share settings
- Optional: link multiple aircraft (future)

#### 2. **Viewer (via link)**
- Read-only access to specific files/folders
- No login required
- Can’t upload or edit

#### 3. **Copilot Assistant (AI)**
- Non-human role
- Can suggest file categories
- Always optional and passive

---

### 🧭 Primary User Journeys (Max 3 Steps)

#### 1. Upload & Organize
1. Log in
2. Drag/drop or select files
3. Assign to a folder (or let Copilot suggest)

#### 2. Share with a Mechanic or Broker
1. Click “Share” on file/folder
2. Choose public or password-protected
3. Copy link and send

#### 3. Quick File Lookup on Mobile
1. Open vault on phone
2. Tap folder
3. Preview file instantly
