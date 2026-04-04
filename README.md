# UCEMS - University Club Event Management System

A web-based event management system for Universiti Malaysia Terengganu (UMT) to streamline event proposal submissions, approvals, and reporting.

---

## For New Team Members (Start Here)

Follow these steps **one by one** to get the project running on your laptop.

### Step 1: Install Required Software

You need to install **two things** before you can start:

1. **Git** - for downloading and syncing the project code
   - Download: https://git-scm.com/downloads
   - During installation, just click **Next** for everything (use all default settings)
   - After installing, restart your laptop

2. **Node.js** - for running the app
   - Download: https://nodejs.org (click the **LTS** version, the one on the left)
   - During installation, just click **Next** for everything
   - After installing, restart your laptop

### Step 2: Verify Installation

Open **Command Prompt** (Windows) or **Terminal** (Mac):
- On Windows: Press `Windows key`, type `cmd`, press Enter
- On Mac: Press `Cmd + Space`, type `Terminal`, press Enter

Type these commands one by one and press Enter after each:

```
git --version
```
You should see something like `git version 2.x.x`. If you see an error, reinstall Git.

```
node --version
```
You should see something like `v20.x.x`. If you see an error, reinstall Node.js.

### Step 3: Choose Where to Save the Project

In the same Command Prompt / Terminal, navigate to where you want to save the project. For example, to save it on your Desktop:

**Windows:**
```
cd %USERPROFILE%\Desktop
```

**Mac:**
```
cd ~/Desktop
```

### Step 4: Clone (Download) the Project

Run this command to download the project to your laptop:

```
git clone https://github.com/aidil2105/UCEMS.git
```

Wait for it to finish. You should see a new folder called `UCEMS` on your Desktop.

### Step 5: Open the Project Folder

```
cd UCEMS
```

### Step 6: Install Project Dependencies

```
npm install
```

This will take 1-2 minutes. Wait until it finishes. You'll see a `node_modules` folder appear.

### Step 7: Run the App

```
npm run dev
```

You should see something like:

```
VITE ready in 1000 ms

  -> Local:   http://localhost:3000/
```

Open your browser and go to the URL shown (e.g. `http://localhost:3000/`). You should see the UCEMS app!

To **stop** the server, press `Ctrl + C` in the terminal.

---

## Daily Workflow (After First Setup)

### Pulling Latest Changes (Getting Updates)

Before you start working, **always** pull the latest code:

```
cd Desktop/UCEMS
git pull
```

If you see `Already up to date.` — you're good, no new changes.

If new files were pulled, run this again to install any new dependencies:

```
npm install
```

Then start the app:

```
npm run dev
```

---

## Troubleshooting

### "npm is not recognized"
- Restart your laptop after installing Node.js

### "git is not recognized"
- Restart your laptop after installing Git

### "Port 3000 is already in use"
- Another app is using that port. Run this instead:
  ```
  npx vite --port 5173
  ```

### The page is blank or shows errors
- Stop the server (`Ctrl + C`), then run:
  ```
  npm install
  npm run dev
  ```

### "I messed up the code and want to reset"
- This will undo ALL your local changes and match the online version:
  ```
  git checkout .
  ```

---

## Tech Stack

- **Frontend:** React + TypeScript
- **Styling:** Tailwind CSS
- **Charts:** Recharts
- **Icons:** Lucide React
- **Build Tool:** Vite
