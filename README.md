# gitignore

# 🛡️ Global .gitignore Standards
### Front-End Architecture | Hassan Biswas — UI/UX & Digital Experiences

This repository serves as the **Single Source of Truth** for my project hygiene and repository standards. It is designed for high-performance web development, ensuring that only SEO-friendly, optimized source code (HTML, CSS, JS) is tracked.

---
.
├── .github/
│       └── workflows/
│              └── gitignore-sync.yml    # The auto-sync logic created
├── assets/                   
│     ├── css/
│     │     └── style.css     # Pre-filled with HSL(240, 80%, 50%)
│     ├── js/
│           └── main.js       # Pre-filled with Date cache-busting
│   
├── index.html         # SEO-optimized entry point
├── .gitignore         # Gold Standard file
└── README.md          # The brand documentation

---

## 🚀 Purpose & Logic
I use this repository to maintain a "set-and-forget" automation workflow. By centralizing my `.gitignore` logic here, I ensure:
*   **Zero Maintenance:** All my repositories sync with this file automatically once a month.
*   **Performance:** Prevents bloated repositories by ignoring heavy build artifacts and system junk.
*   **Fallback Security:** Proactively ignores sensitive environment variables (`.env`) and keys.
*   **Device Optimization:** Specifically configured to handle mobile development artifacts from **Oppo A53 (Android)**.

## 🛠️ Integrated Technologies
*   **Languages:** HTML, CSS (HSL Standards), JavaScript
*   **Platforms:** GitHub Actions, Android (Termux/Mobile Dev)
*   **Design Tools:** Figma, Framer, Webflow

---

## 🔄 Automation Workflow
The `.gitignore` in my other repositories is kept up-to-date via a **Monthly Schedule** (`0 0 1 * *`) using GitHub Actions.

```yaml
# Logic Preservation snippet used in workflows:
- name: 🔄 Fetch Gold Standard
  run: curl -sSL [https://raw.githubusercontent.com/hassanbiswas/gitignore/main/.gitignore](https://raw.githubusercontent.com/hassanbiswas/gitignore/main/.gitignore) -o .gitignore
