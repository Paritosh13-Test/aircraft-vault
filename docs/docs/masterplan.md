## Aircraft Vault – Masterplan

### ✈️ Elevator Pitch
Aircraft Vault is a secure, aviation-grade document vault for aircraft owners. It organizes essential files like logbooks, STCs, and maintenance records in a clean, minimal UI—built for trust, precision, and effortless sharing.

### 🚨 Problem & Mission
Aircraft owners juggle critical documents across email threads, paper folders, and scattered cloud drives. There's no central, secure, aviation-native tool for organizing and sharing them. Aircraft Vault solves this with a vault built like an aircraft system: minimal, robust, and quietly confident.

### 👥 Target Audience
- **Private aircraft owners & pilots** managing their own paperwork
- **Aviation mechanics & brokers** needing read-only access to specific aircraft files
- **Small charter operators** handling internal file distribution

### 🧩 Core Features
- **Login / Landing**: Clear, secure CTA—"Access My Vault"
- **Dashboard**: Folder-style UI with upload & drag-drop
- **File Upload + Preview**: Supports PDF, images, docs; real-time previews
- **Default Folders**: Logbooks, Maintenance Records, STCs, Other
- **Sharing Links**: Public or password-protected with read-only mode
- **Mobile-Ready**: Sticky upload buttons + responsive layout

### 🛠 Tech Stack (Why It Fits)
- **Frontend**: Vite + React + Tailwind + shadcn/ui → Fast, modern, minimal
- **Backend/DB**: Supabase → Auth, storage, and real-time DB in one
- **Storage**: Supabase buckets or Lovable Cloud → Secure, structured access
- **Auth**: Email/password (Google optional) → Familiar but safe

### 🧱 Conceptual Data Model (ERD Sketch in Words)
- **User**
  - id, name, email, auth_provider
- **Aircraft**
  - id, user_id, tail_number, make, model
- **Folder**
  - id, aircraft_id, name (Logbooks, etc.)
- **File**
  - id, folder_id, name, type, URL, uploaded_at
- **ShareLink**
  - id, file_id or folder_id, public_url, is_password_protected, expires_at

### 🎨 UI Design Principles
- Minimalist layout with aviation-grade confidence
- High contrast, neutral tones for focus
- Folder-first structure reduces decision fatigue
- Subtle hover states and calm motion express trust
- Sticky actions (upload, create folder) = 3-click simplicity

### 🔒 Security & Compliance
- Supabase auth with secure role-based rules
- Files stored with access-limited URLs
- Sharing links expire or require password
- Future SOC2 compliance considerations if scaled commercially

### 🗺️ Phased Roadmap

#### ✅ MVP
- Email/password auth
- File upload, foldering, sharing
- Mobile-friendly UI

#### 🚀 V1
- Vault Copilot AI assistant (categorize uploads)
- Google login
- Audit logs & activity tracking

#### ✨ V2
- Multi-aircraft support per account
- Offline access (via PWA or cache)
- Advanced permissions (viewer/editor)

### ⚠️ Risks & Mitigations
- **Low engagement** → Add default folders & calm onboarding
- **File misuse** → Password-protect sharing + expiration logic
- **Tech stack sprawl** → Stick to Supabase-first stack

### 🌱 Future Expansion Ideas
- FAA compliance mode (for certified logs)
- Version control for key file types
- Watermarked previews for brokers
- “Vault Transfer” for aircraft sales

