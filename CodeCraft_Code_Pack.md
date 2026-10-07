# CODECRAFT — CODE PACK

 **Copy → Paste → Save → Check → Personalize**

 ## How to Use This Code Pack

 For every file:

 1. Create the file in the location shown.
2. Copy the complete code.
3. Paste it.
4. Save it.
5. Check the browser.

 **Do not type the code manually.**

 Replace only the clearly marked personal placeholders. Keep the component names and import paths exactly as shown.

---

 ## 1\. `src/data/portfolioData.js`

 **Create:** `src → data → portfolioData.js`

```
export const portfolioData = {
  name: "Your Name",
  role: "Computer Science Student",
  bio: "Write a short introduction about yourself. Mention what you enjoy building and what you are learning.",

  skills: [
    "JavaScript",
    "React",
    "Python",
    "HTML",
    "CSS",
    "Git & GitHub",
  ],

  projects: [
    {
      title: "Project One",
      description: "Briefly describe what you built and what problem it solves.",
      tech: ["React", "JavaScript"],
      github: "https://github.com/yourusername/project-one",
    },
    {
      title: "Project Two",
      description: "Briefly describe your second project.",
      tech: ["Python", "HTML", "CSS"],
      github: "https://github.com/yourusername/project-two",
    },
  ],

  achievements: [
    "Participated in a hackathon",
    "Completed a technical certification",
    "Add your achievement here",
  ],

  github: "https://github.com/yourusername",
  linkedin: "https://www.linkedin.com/in/yourusername/",
  email: "your@email.com",
}
```

 ### PERSONALIZE

 Replace:

 - Name
- Role
- Bio
- Skills
- Projects
- Achievements
- GitHub
- LinkedIn
- Email

 with your own details.

---

 ## 2\. `src/components/Navbar.jsx`

 **Create:** `src → components → Navbar.jsx`

```
function Navbar() {
  return (
    <nav className="fixed top-0 z-50 w-full border-b border-white/10 bg-gray-950/80 backdrop-blur-md">
      <div className="mx-auto flex max-w-6xl items-center justify-between px-6 py-4">
        <a href="#home" className="text-xl font-bold text-white">
          Portfolio<span className="text-blue-400">.</span>
        </a>

        <div className="hidden gap-6 text-sm text-gray-300 sm:flex">
          <a href="#home" className="transition hover:text-blue-400">Home</a>
          <a href="#about" className="transition hover:text-blue-400">About</a>
          <a href="#skills" className="transition hover:text-blue-400">Skills</a>
          <a href="#projects" className="transition hover:text-blue-400">Projects</a>
          <a href="#achievements" className="transition hover:text-blue-400">Achievements</a>
          <a href="#contact" className="transition hover:text-blue-400">Contact</a>
        </div>
      </div>
    </nav>
  )
}

export default Navbar
```

---

 ## 3\. `src/components/Hero.jsx`

 **Create:** `src → components → Hero.jsx`

```
import { portfolioData } from "../data/portfolioData"

function Hero() {
  return (
    <section
      id="home"
      className="relative flex min-h-screen items-center overflow-hidden bg-gray-950 px-6 pt-20"
    >
      <div className="absolute left-1/4 top-1/4 h-72 w-72 rounded-full bg-blue-500/20 blur-3xl" />
      <div className="absolute bottom-1/4 right-1/4 h-72 w-72 rounded-full bg-purple-500/20 blur-3xl" />

      <div className="relative z-10 mx-auto grid max-w-6xl items-center gap-12 md:grid-cols-2">
        <div>
          <p className="mb-4 text-lg font-medium text-blue-400">
            👋 Hello, I'm
          </p>

          <h1 className="text-5xl font-bold tracking-tight text-white sm:text-6xl lg:text-7xl">
            {portfolioData.name}
          </h1>

          <h2 className="mt-4 text-2xl font-semibold text-gray-300 sm:text-3xl">
            {portfolioData.role}
          </h2>

          <p className="mt-6 max-w-xl text-lg leading-8 text-gray-400">
            {portfolioData.bio}
          </p>

          <div className="mt-8 flex flex-wrap gap-4">
            <a
              href="#projects"
              className="rounded-full bg-blue-500 px-6 py-3 font-medium text-white transition hover:bg-blue-600"
            >
              View My Projects →
            </a>

            <a
              href={portfolioData.github}
              target="_blank"
              rel="noreferrer"
              className="rounded-full border border-white/20 px-6 py-3 font-medium text-gray-200 transition hover:border-blue-400 hover:text-blue-400"
            >
              GitHub ↗
            </a>
          </div>

          <div className="mt-10 flex flex-wrap gap-6 text-sm text-gray-400">
            <span>💻 Developer</span>
            <span>🚀 Problem Solver</span>
            <span>📚 Lifelong Learner</span>
          </div>
        </div>

        <div className="flex justify-center">
          <div className="h-64 w-64 overflow-hidden rounded-full border-4 border-blue-400/30 shadow-2xl sm:h-80 sm:w-80">
            <img
              src="/images/profile.jpg"
              alt={`${portfolioData.name} profile`}
              className="h-full w-full object-cover"
            />
          </div>
        </div>
      </div>
    </section>
  )
}

export default Hero
```

---

 ## 4\. `src/components/About.jsx`

 **Create:** `src → components → About.jsx`

```
import { portfolioData } from "../data/portfolioData"

function About() {
  return (
    <section id="about" className="bg-gray-900 px-6 py-24">
      <div className="mx-auto max-w-4xl">
        <p className="text-sm font-semibold uppercase tracking-widest text-blue-400">
          About Me
        </p>

        <h2 className="mt-3 text-4xl font-bold text-white">
          A little about me
        </h2>

        <p className="mt-6 text-lg leading-8 text-gray-400">
          {portfolioData.bio}
        </p>
      </div>
    </section>
  )
}

export default About
```

---

 ## 5\. `src/components/Skills.jsx`

 **Create:** `src → components → Skills.jsx`

```
import { portfolioData } from "../data/portfolioData"

function Skills() {
  return (
    <section id="skills" className="bg-gray-950 px-6 py-24">
      <div className="mx-auto max-w-6xl">
        <p className="text-sm font-semibold uppercase tracking-widest text-blue-400">
          Skills
        </p>

        <h2 className="mt-3 text-4xl font-bold text-white">
          Technologies I work with
        </h2>

        <div className="mt-10 flex flex-wrap gap-4">
          {portfolioData.skills.map((skill) => (
            <span
              key={skill}
              className="rounded-full border border-white/10 bg-white/5 px-5 py-3 text-gray-200"
            >
              {skill}
            </span>
          ))}
        </div>
      </div>
    </section>
  )
}

export default Skills
```

---

 ## 6\. `src/components/Projects.jsx`

 **Create:** `src → components → Projects.jsx`

```
import { portfolioData } from "../data/portfolioData"

function Projects() {
  return (
    <section id="projects" className="bg-gray-900 px-6 py-24">
      <div className="mx-auto max-w-6xl">
        <p className="text-sm font-semibold uppercase tracking-widest text-blue-400">
          Projects
        </p>

        <h2 className="mt-3 text-4xl font-bold text-white">
          Things I've built
        </h2>

        <div className="mt-10 grid gap-6 md:grid-cols-2">
          {portfolioData.projects.map((project) => (
            <article
              key={project.title}
              className="rounded-2xl border border-white/10 bg-gray-950 p-6"
            >
              <h3 className="text-2xl font-semibold text-white">
                {project.title}
              </h3>

              <p className="mt-4 leading-7 text-gray-400">
                {project.description}
              </p>

              <div className="mt-5 flex flex-wrap gap-2">
                {project.tech.map((technology) => (
                  <span
                    key={technology}
                    className="rounded-full bg-blue-500/10 px-3 py-1 text-sm text-blue-300"
                  >
                    {technology}
                  </span>
                ))}
              </div>

              <a
                href={project.github}
                target="_blank"
                rel="noreferrer"
                className="mt-6 inline-block font-medium text-blue-400 hover:text-blue-300"
              >
                View on GitHub →
              </a>
            </article>
          ))}
        </div>
      </div>
    </section>
  )
}

export default Projects
```

---

 ## 7\. `src/components/Achievements.jsx`

 **Create:** `src → components → Achievements.jsx`

```
import { portfolioData } from "../data/portfolioData"

function Achievements() {
  return (
    <section id="achievements" className="bg-gray-950 px-6 py-24">
      <div className="mx-auto max-w-6xl">
        <p className="text-sm font-semibold uppercase tracking-widest text-blue-400">
          Achievements
        </p>

        <h2 className="mt-3 text-4xl font-bold text-white">
          Milestones & achievements
        </h2>

        <div className="mt-10 grid gap-4">
          {portfolioData.achievements.map((achievement, index) => (
            <div
              key={index}
              className="rounded-2xl border border-white/10 bg-white/5 p-5 text-gray-300"
            >
              🏆 {achievement}
            </div>
          ))}
        </div>
      </div>
    </section>
  )
}

export default Achievements
```

---

 ## 8\. `src/components/Contact.jsx`

 **Create:** `src → components → Contact.jsx`

```
import { portfolioData } from "../data/portfolioData"

function Contact() {
  return (
    <section id="contact" className="bg-gray-900 px-6 py-24">
      <div className="mx-auto max-w-4xl text-center">
        <p className="text-sm font-semibold uppercase tracking-widest text-blue-400">
          Contact
        </p>

        <h2 className="mt-3 text-4xl font-bold text-white">
          Let's connect
        </h2>

        <p className="mx-auto mt-6 max-w-2xl text-lg text-gray-400">
          Interested in connecting or collaborating? Find me online.
        </p>

        <div className="mt-8 flex flex-wrap justify-center gap-4">
          <a
            href={`mailto:${portfolioData.email}`}
            className="rounded-full bg-blue-500 px-6 py-3 font-medium text-white hover:bg-blue-600"
          >
            Email Me
          </a>

          <a
            href={portfolioData.linkedin}
            target="_blank"
            rel="noreferrer"
            className="rounded-full border border-white/20 px-6 py-3 font-medium text-gray-200 hover:border-blue-400 hover:text-blue-400"
          >
            LinkedIn ↗
          </a>

          <a
            href={portfolioData.github}
            target="_blank"
            rel="noreferrer"
            className="rounded-full border border-white/20 px-6 py-3 font-medium text-gray-200 hover:border-blue-400 hover:text-blue-400"
          >
            GitHub ↗
          </a>
        </div>
      </div>
    </section>
  )
}

export default Contact
```

---

 ## 9\. `src/App.jsx`

 Replace the contents of `src/App.jsx` with:

```
import Navbar from "./components/Navbar"
import Hero from "./components/Hero"
import About from "./components/About"
import Skills from "./components/Skills"
import Projects from "./components/Projects"
import Achievements from "./components/Achievements"
import Contact from "./components/Contact"

function App() {
  return (
    <div className="min-h-screen bg-gray-950">
      <Navbar />
      <Hero />
      <About />
      <Skills />
      <Projects />
      <Achievements />
      <Contact />
    </div>
  )
}

export default App
```

---

 ## 10\. `src/main.jsx`

 Usually Vite's `main.jsx` is already correct. Make sure it looks like this:

```
import { StrictMode } from "react"
import { createRoot } from "react-dom/client"
import "./index.css"
import App from "./App.jsx"

createRoot(document.getElementById("root")).render(
  <StrictMode>
    <App />
  </StrictMode>,
)
```

---

 ## 11\. `src/index.css`

 Keep your Tailwind setup from the workshop.

 If the facilitator's setup uses a different `index.css`, follow the live setup instructions.

 **Important:** Tailwind utility classes must be available.

---

 ## 12\. FINAL CHECK

 Save every file and check the browser.

 Run:

```
npm run dev
```

 If something breaks, **stop and fix the error before moving on.**

 When the portfolio looks correct, run:

```
npm run build
```

---

 ## 13\. GITHUB COMMANDS

 Run the following commands:

```
git init
git add .
git commit -m "My CodeCraft portfolio"
git branch -M main
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main
```

 Replace:

```
YOUR_GITHUB_REPOSITORY_URL
```

 with your actual GitHub repository URL.

---

 ## 14\. VERCEL DEPLOYMENT

 1. Go to **Vercel**.
2. Sign in with GitHub.
3. Select **Add New Project**.
4. Import your repository.
5. Deploy.

 For a normal Vite project:

```
Build Command: npm run build
Output Directory: dist
```

---

 # Important Workshop Rule

 > **If you see an error, do not keep copying the next file. Stop, read the error, and ask the facilitator for help.**

 Everyone should reach the same working checkpoint before the workshop moves forward.