# Cosmicgram Frontend ✨

The user interface for **Cosmicgram**—an AI-powered, safe social media environment. It features a modern, responsive layout, real-time safety badges, and deep integrations with the **Prahari AI Shield** to automatically enforce community standards right as posts are created.

> 🔗 **Looking for the AI Backend?**
> The backend logic (FastAPI, Python, MuRIL, CLIP) lives in its own dedicated repository. 
> [**Click here to view the Cosmicgram Backend Repository**](https://github.com/YOUR_GITHUB_USERNAME/cosmicgram-backend)


---

## 🎨 Features & UI
-   🔒 **Real-Time Safety Previews**: Visual feed badges indicating the AI's classification ("Hateful", "NSFW", or "Safe").
-   🚀 **Lightning Fast Feed**: Optimized React components built with Vite and TailwindCSS.
-   📱 **Fully Responsive**: Adapts flawlessly from mobile browsers to ultra-wide desktop monitors.
-   🛡️ **Prahari Integration**: The "Create Post" screen immediately queries the Prahari Backend before publishing, giving users immediate feedback via the Warning Modal if their content is flagged.

---

## 📸 Screenshots

*(Replace the paths below with your actual screenshot images once deployed)*

| Home Feed (Safe/Flagged Posts) | Post Creation (Prahari Shield Active) |
| :----------------------- | :--------------------------- |
| `![Feed Screenshot](public/feed.png)` | `![Creator Screenshot](public/create_post.png)` |

---

## 🛠️ Tech Stack

-   **Framework**: React 18
-   **Build Tool**: Vite
-   **Styling**: TailwindCSS & Radix UI Primitives (via shadcn/ui)
-   **Routing**: React Router DOM
-   **Icons**: Lucide React
-   **State & Animation**: Framer Motion

---

## 💻 Local Setup & Installation

### 1. Install Dependencies
install the necessary Node modules:
```bash
npm install
# or
bun install
```

### 2. Configure Environment variables
Create a `.env` file in the root of the `frontend/` directory:
```env
# Point this to your local backend when testing
VITE_API_URL=http://localhost:8000
```

### 3. Start the Development Server
```bash
npm run dev
# or
bun run dev
```

Your app will be running dynamically on `http://localhost:5173`. Any changes will Hot-Module-Reload instantly.

---

## ☁️ Deployment (Vercel)
See the root `deployment_guide.md` for full instructions on configuring Vercel and linking it to your Railway backend instance. Ensure you set the `Root Directory` in Vercel to `frontend`.
