## Aircraft Vault – Implementation Plan

### 🔨 Step-by-Step Build Sequence

#### 1. Setup & Scaffolding
- [ ] Initialize Vite + React + TypeScript project
- [ ] Install Tailwind CSS + shadcn/ui components
- [ ] Set up Supabase project (auth, storage, DB)

#### 2. Auth & Access
- [ ] Build login page (email + password)
- [ ] Optional: add Google OAuth via Supabase
- [ ] Route protection logic (unauthenticated → login)

#### 3. Vault Dashboard
- [ ] Layout: “My Aircraft Vault” with folder grid
- [ ] Add default folders on first login (Logbooks, etc.)
- [ ] CTA buttons: “+ Upload File”, “+ Create Folder”

#### 4. File Upload Flow
- [ ] Enable drag-and-drop + file picker
- [ ] Save files to Supabase storage with folder reference
- [ ] Preview PDF, image, and doc files

#### 5. Folder & File Management
- [ ] CRUD for folders (rename, delete, move)
- [ ] Show files within folders; sortable grid
- [ ] Add "empty folder" friendly states

#### 6. Sharing System
- [ ] Generate shareable public URLs for files/folders
- [ ] Toggle: password-protect + expiration date
- [ ] Public viewer UI (read-only, no login)

#### 7. Mobile Optimization
- [ ] Responsive layout: single-column mode on mobile
- [ ] Sticky bottom bar: quick upload, new folder

#### 8. Optional AI Assistant (Vault Copilot)
- [ ] Add background job to auto-tag/categorize based on filename/content
- [ ] UI: “Suggest folder” prompt on upload
- [ ] Toggle assistant in settings

### 📆 Timeline with Checkpoints (6 Weeks)

- **Week 1**: Project setup + auth
- **Week 2**: Vault dashboard + folder structure
- **Week 3**: File upload + preview
- **Week 4**: Sharing system + public viewer
- **Week 5**: Mobile polish + drag/drop
- **Week 6**: Vault Copilot prototype + QA

### 👥 Team Roles & Rituals

#### Roles
- **Frontend Dev**: Vault UI, upload flow, responsive design
- **Backend Dev**: Supabase config, file storage, share logic
- **PM/Founder**: Test flights, feedback, microcopy tuning
- **Designer (optional)**: Polish folder UI, icons, animations

#### Recommended Rituals
- 🧪 **Bi-weekly usability test**: 3 new users; test upload + share flow
- 📋 **Weekly demo day**: Internal walkthrough of current build
- 🔄 **Friday retro**: What felt clunky? What felt pro?

### 🧩 Optional Integrations & Stretch Goals
- [ ] FAA Doc Sync (import from FAA registry)
- [ ] Stripe: premium tier with audit logs + multiple aircraft
- [ ] PDF watermarking for broker views
- [ ] Offline mode (PWA with cached vault)
