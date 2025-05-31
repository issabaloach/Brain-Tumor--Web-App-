
# 🤝 Contributing Guide – Brain Tumor Detection (Frontend - Next.js)

---

## 🧠 Overview

This is the **frontend** of a Final Year Project (FYP) for a Brain Tumor Detection system. It is built using **Next.js**, styled using **Tailwind CSS** and either **ShadCN UI** or **Ant Design (antd)**. It communicates with a backend ML API for tumor predictions.

---

## 📁 Folder Structure

```
brain-tumor-detector-frontend/
├── public/                    # Static files (logo, icons, default images)
├── styles/                    # Global CSS (Tailwind or custom)
├── components/                # Reusable UI components
│   ├── ui/                    # UI elements (ShadCN or AntD-based)
│   │   ├── UploadMRI.jsx
│   │   ├── PredictResult.jsx
│   │   ├── LoadingSpinner.jsx
│   │   ├── Sidebar.jsx
│   │   ├── Header.jsx
│   │   └── Button.jsx
│   ├── layout/                # Layout wrappers
│   │   └── MainLayout.jsx
│   ├── history/               # Components for history feature
│   │   └── HistoryTable.jsx
│   └── auth/                  # Optional: login/register forms
│       └── LoginForm.jsx
├── pages/                     # Next.js pages
│   ├── index.js               # Upload page
│   ├── result.js              # Show prediction result
│   ├── history.js             # View past predictions
│   ├── _app.js                # App wrapper (global CSS/layout)
│   └── api/
│       └── predict.js         # Client API route for ML backend
├── lib/                       # Utility functions
│   └── apiClient.js
├── assets/                    # Icons, images
├── .env.local                 # Environment variables
├── next.config.js             # Next.js config
├── tailwind.config.js         # Tailwind config (if using ShadCN)
├── package.json
└── README.md
```

---

## 🔧 UI Component Libraries

This project supports **either** of the following UI libraries:

### ✅ ShadCN UI
- Tailwind-based component system
- Uses `npx shadcn-ui@latest init` to install
- Great for modern, accessible UIs

### ✅ Ant Design (AntD)
- Install with `npm install antd @ant-design/icons`
- Includes ready-to-use components like Upload, Card, Table, etc.

we can choose one, or mix responsibly.

---

## 📄 Documentation Links

- 📘 `README.md` – Contains setup guide, features, and deployment info
- 📘 `.env.local` – Used to store the backend API URL (`NEXT_PUBLIC_API_URL`)
- 📘 `apiClient.js` – Centralized API handling

---

## 🚀 Getting Started

```bash
git clone https://github.com/issabaloach/Brain-Tumor--Web-App-
cd brain-tumor-detector-frontend
npm install
npm run dev
```

Set the backend URL in `.env.local`:
```env
NEXT_PUBLIC_API_URL=http://localhost:5000/predict
```

---

## 🧪 Testing & Dev Notes

- All image uploads must be `.png`, `.jpg`, or `.jpeg`
- Be sure the backend ML model is **running and accessible**
- Use `console.log()` responsibly for debugging
- Ensure UI responsiveness (desktop/mobile)

---

## 💡 Contribution Rules

- Use meaningful component names
- Keep styles clean and consistent
- Write reusable and modular code
- Document your changes clearly in PRs or commits

---

## 🙌 Thanks for your time to look after our FYP (Brain Tumor Detection Web App)
