Absolutely — here is the **clean, copyable Markdown version** of your CODECRAFT participant guide. I’ve preserved the content while formatting headings, checklists, code blocks, tables, and structure for easy copying into a `.md` file.

````
# CODECRAFT 🚀

## Build. Personalize. Deploy.

**Participant Guide • React + Vite + Tailwind CSS + GitHub + Vercel**

---

## What You Will Build

Create your own developer portfolio from scratch, personalize it, push it to GitHub, and deploy it as a live website using Vercel.

### Workshop Flow

**Create → Understand → Copy Code → Personalize → Test → GitHub → Vercel**

---

# Before You Start

- [ ] VS Code installed
- [ ] Node.js installed
- [ ] Git installed
- [ ] GitHub account created
- [ ] Vercel account ready (sign in with GitHub)
- [ ] Profile photo ready
- [ ] Your skills, projects and achievements ready

> Keep this guide open beside VS Code so you can copy commands and code easily.

---

# PART 1 — CREATE YOUR REACT PROJECT

Open **VS Code → Terminal** and run:

```bash
npm create vite@latest codecraft-portfolio
````

 Select:

 - [ ] Framework → React
- [ ] Variant → JavaScript

 Then run:

```
cd codecraft-portfolio
npm install
npm run dev
```

 Open the **localhost** link shown in the terminal.

---

 # PART 2 — CREATE THE PROJECT STRUCTURE

 Create the project and files manually.

 This helps you understand how a React project is organized.

```
src/
├── components/
│   ├── Navbar.jsx
│   ├── Hero.jsx
│   ├── About.jsx
│   ├── Skills.jsx
│   ├── Projects.jsx
│   ├── Achievements.jsx
│   └── Contact.jsx
├── data/
│   └── portfolioData.js
├── App.jsx
└── main.jsx

public/
└── images/
    └── profile.jpg
```

 Put your profile photo inside:

```
public/images/
```

 If you use another filename, update the image path in the code.

---

 # PART 3 — TAILWIND CSS

 Use the Tailwind setup demonstrated by the workshop facilitator.

 > The exact command can vary by Tailwind version.

 **Do not continue until Tailwind classes work in the browser.**

---

 # PART 4 — ADD YOUR PORTFOLIO DATA

 Open:

```
src/data/portfolioData.js
```

 Paste the code supplied by the facilitator, then replace the sample values.

 - [ ] Name
- [ ] Role / title
- [ ] Short bio
- [ ] Skills
- [ ] Projects
- [ ] Achievements
- [ ] GitHub / LinkedIn / contact links

 > **Important:** Do not leave placeholder text such as `"Your Name"` in the final portfolio.

---

 # PART 5 — BUILD THE COMPONENTS

 For each component:

 **Create the file manually → Copy the provided code → Save → Check the browser → Fix any error before continuing.**

 - [ ] `Navbar.jsx` — Navigation
- [ ] `Hero.jsx` — Introduction, profile image and CTA
- [ ] `About.jsx` — Background / introduction
- [ ] `Skills.jsx` — Skills and technologies
- [ ] `Projects.jsx` — Projects and links
- [ ] `Achievements.jsx` — Hackathons, certifications and awards
- [ ] `Contact.jsx` — Contact and social links

---

 # PART 6 — CONNECT EVERYTHING

 Open:

```
src/App.jsx
```

 Paste the code supplied by the facilitator to import and arrange your components.

 Save the file and confirm that the complete portfolio appears.

---

 # PART 7 — PERSONALIZE YOUR PORTFOLIO

 Now make the website yours.

 ## Personalization Checklist

 - [ ] Replace name
- [ ] Replace role / title
- [ ] Write your own bio
- [ ] Add profile photo
- [ ] Add real skills
- [ ] Add 1–3 real projects
- [ ] Add project descriptions and technologies
- [ ] Add GitHub links
- [ ] Add achievements / certifications / hackathons
- [ ] Add LinkedIn, GitHub and contact information
- [ ] Remove all placeholder content

 ### Quality Rule

 > **Genuine work is better than invented projects or achievements.**

---

 # PART 8 — TEST YOUR WEBSITE

 Check the following:

 - [ ] Navbar links work
- [ ] All sections appear
- [ ] Profile image appears
- [ ] Name and bio are correct
- [ ] Projects are correct
- [ ] Social links are correct
- [ ] No obvious errors
- [ ] Layout looks good

 ## Create a Production Build

 Run:

```
npm run build
```

 If the build succeeds, continue to GitHub.

---

 # PART 9 — CREATE YOUR GITHUB REPOSITORY

 On GitHub, create a **new EMPTY repository**.

 For example:

```
codecraft-portfolio
```

 > Do not initialize it with another README, `.gitignore` or license if following these commands.

 Run:

```
git init
git add .
git commit -m "My CodeCraft portfolio"
git branch -M main
```

 Copy **YOUR repository URL** and run:

```
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main
```

 Refresh GitHub and confirm your files are visible.

---

 # PART 10 — DEPLOY WITH VERCEL 🚀

 - [ ] Open Vercel and sign in with GitHub
- [ ] Choose **Add New Project**
- [ ] Find your portfolio repository
- [ ] Click **Import**
- [ ] Check the detected settings
- [ ] Click **Deploy**

 ## Standard Vite Settings

 For a standard Vite project, the settings are normally:

 | Setting | Value |
| --- | --- |
| Framework | Vite |
| Build Command | `npm run build` |
| Output Directory | `dist` |

> If Vercel detects these automatically, keep the defaults unless the facilitator instructs otherwise.

---

 # PART 11 — YOUR LIVE PORTFOLIO

 When deployment finishes, Vercel gives you a public URL.

 - [ ] Open the live URL
- [ ] Test every section
- [ ] Test social links
- [ ] Open it on your phone
- [ ] Save the live URL
- [ ] Use it later on your resume / LinkedIn

---

 # 🎉 Congratulations!

 You built and deployed your portfolio.

---

 # QUICK COMMANDS

```
npm install
npm run dev
npm run build

git init
git add .
git commit -m "My CodeCraft portfolio"
git branch -M main
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main
```

---

 # TROUBLESHOOTING

 ## `npm is not recognized`

 Install/reinstall Node.js, restart VS Code, and try again.

---

 ## `git is not recognized`

 Install Git and restart VS Code/your terminal.

---

 ## Cannot find `package.json`

 You are likely in the wrong folder.

 Enter:

```
cd codecraft-portfolio
```

---

 ## Image is not showing

 Check:

```
public/images/
```

 and verify the image path, for example:

```
/images/profile.jpg
```

---

 ## Page is blank / error

 Check the terminal and browser console for:

 - Missing imports
- Missing brackets
- Missing commas
- Wrong filenames
- Incorrect file paths

---

 ## GitHub push is rejected

 Check that the remote URL points to your own empty repository.

---

 ## Vercel build fails

 Run the build locally:

```
npm run build
```

 Fix the reported error before redeploying.

---

 # FINAL CODECRAFT CHECKLIST

 - [ ] Portfolio created from scratch
- [ ] Components created
- [ ] Information personalized
- [ ] Profile photo added
- [ ] Projects added
- [ ] Git initialized
- [ ] GitHub repository created
- [ ] Code pushed to GitHub
- [ ] Production build successful
- [ ] Portfolio deployed on Vercel
- [ ] Live URL tested on phone
- [ ] Live URL saved

---

 # CODECRAFT 🚀

 **Build. Learn. Create.**

```

```