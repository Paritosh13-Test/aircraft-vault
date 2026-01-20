## Aircraft Vault – Task Tracker

This document tracks all features required to build the Aircraft Vault application. Each task is grouped by theme and ordered for step-by-step execution. Subtasks may include frontend, backend, or design work.

---

### ✅ Project Setup

- [ ] Initialize Vite + TypeScript + Tailwind project
- [ ] Install shadcn/ui and setup base components
- [ ] Connect to Supabase project (auth + storage + DB)

---

### 🔐 Authentication & Access

- [ ] Build login screen (email + password)
- [ ] Optional: Add Google OAuth via Supabase
- [ ] Redirect unauthenticated users to login

---

### 🗂️ Vault Dashboard

- [ ] Create `/vault` page layout with top bar
- [ ] Add default folders: Logbooks, Maintenance, STCs, Other
- [ ] Implement file/folder grid display
- [ ] CTA buttons: “+ Upload File”, “+ Create Folder”
- [ ] Mobile layout with sticky upload bar

---

### 📤 File Upload & Preview

- [ ] Support drag-and-drop and file picker
- [ ] Upload files to Supabase storage
- [ ] Store folder metadata with each file
- [ ] Show file preview (PDF, image, doc)
- [ ] Show upload success animation

---

### 📁 Folder Management

- [ ] Create folder flow with modal
- [ ] Rename/delete/move folders
- [ ] Display empty folder states

---

### 🔗 Secure Sharing

- [ ] Generate public or password-protected share links
- [ ] Store link access settings (password, expiration)
- [ ] Create `/share/:id` read-only viewer layout
- [ ] Ensure links work with no login

---

### 📱 Mobile Optimization

- [ ] Single-column layout on small screens
- [ ] Sticky bottom bar for “Upload” and “New Folder”
- [ ] Tap-to-preview file flow

---

### 🧠 Optional: Vault Copilot AI

- [ ] Background function: tag or categorize files
- [ ] Suggest folder UI on upload
- [ ] Toggle AI on/off from settings

---

### ✅ Stretch Goals

- [ ] FAA Registry sync
- [ ] Stripe payments for premium features
- [ ] Audit log system
- [ ] Offline/PWA mode

---

### 📌 Tracking Notes

- Mark tasks as ✅ once implemented
- Reference other docs in `/docs/` as needed
- Feel free to add nested subtasks under any item
