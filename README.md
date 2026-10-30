# 🕒 Electron.js Desktop Clock

A lightweight desktop clock application built with **Electron.js**, HTML, CSS, and JavaScript as a first exploration into desktop application development.

---

## 📂 Project Structure

```text
learning-electronjs/
├── dist/             # Compiled/packaged application output (.exe)
├── node_modules/     # Project dependencies
├── src/              # Source assets (including images)
│   └── images/
├── .gitignore        # Ignored files for Git
├── index.html        # Main user interface markup
├── main.js           # Electron main process script
├── package-lock.json # Dependency lock file
├── package.json      # Project metadata and dependencies
├── README.md         # Project documentation
└── style.css         # Styling and dark theme animations
```

--- 

## 📥 Getting Started & Installation

To run this project locally on your machine, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/inabits/learning-electronjs.git
cd learning-electronjs
```

2. Install Node.js:

Ensure you have Node.js installed on your system (which includes npm).

3. Install dependencies:

```bash
npm install
```

4. Run the application:

```bash
npx electron .
```

---

## 📦 Building the Executable (.exe)

To package this application into a standalone Windows executable (`.exe`), you can use `electron-packager`. Run the following command in your terminal:

```bash
npx electron-packager . clock --platform=win32 --arch=x64 --out=dist
```

This command packages the current directory (`.`) naming the application `clock`, targets the Windows platform (`win32`) with a 64-bit architecture (`x64`), and outputs the result into the `dist/` folder.

---

## 💡 Challenges & Learnings

As my first time building a desktop application with **Electron.js**, this project came with a few unique hurdles:

- **Understanding the Main vs. Renderer Process:** Shifting from standard web development to Electron required wrapping my head around how the Node.js backend (`main.js`) communicates with the browser window (`index.html`).
- **Window Lifecycle Management:** Learning how to properly instantiate the `BrowserWindow`, handle app events (`window-all-closed`, `activate`), and manage application startup flows.
- **Packaging and Distribution:** Figuring out how to configure build tools like `electron-packager` to correctly bundle web assets and dependencies into a standalone executable file.

---

## 👩‍💻 Author

Bianca Inazumi
