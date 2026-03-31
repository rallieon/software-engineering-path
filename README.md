# From Teacher to Software Engineer: A Learning Plan

## Why I Wrote This

We talked a bit ago about your transition into engineering, and I wanted to put some thoughts together while it was fresh.

One thing I feel strongly about with people starting in software today: AI tools make it possible to build things incredibly fast, which is great. But in order to actually be successful long-term, I think there's a foundational layer that needs to be learned. Without it, you can get things working but you won't always understand *why* they work, or know what to do when they don't.

I put this plan together as a rough path through what I think that foundational layer looks like.

Keep using AI tools — but use them as a tutor, not a crutch. When Claude or Copilot writes code, don't just accept it. Read every line. Ask "why this and not that?" The engineers I see getting the most out of AI tools are the ones who understand what the tools are actually doing. The fundamentals in this plan are what make those tools 10x more powerful in your hands.

And remember — the goal isn't to learn everything. It's to learn enough to be dangerous, then keep learning on the job. The most pragmatic thing you can do is start building, get comfortable being wrong, ask for feedback early, and never pretend you know something you don't. That honesty is what earns trust on an engineering team, and it's a habit worth building from day one.

I'm around if you get stuck or want to talk through any of this. And if you ever want to dig into something in depth — system design, a concept that's not clicking, whatever — I'm happy to sit down for a few hours over coffee or beers and work through it together.

---

## What I Think Makes a Good Engineer

Before getting into the plan itself, I want to share how I think about this. The best engineers I've worked with are not the ones who write the cleverest code. They're the ones who are pragmatic — they pick the simplest solution that actually works, they're honest about tradeoffs, and they can communicate clearly with people who aren't engineers. There's a great article by John Allspaw called ["On Being A Senior Engineer"](https://www.kitchensoap.com/2012/10/25/on-being-a-senior-engineer/) that captures this better than I can. His core point is that technical skill is necessary but not sufficient. What separates the engineers people want to work with is maturity: seeking out feedback instead of avoiding it, making tradeoffs explicit instead of hiding them, doing the unglamorous work without complaint, and lifting the people around you instead of just yourself. One line from it that stuck with me: *"The degree to which other people want to work with you is a direct indication of how successful you'll be in your career as an engineer."*

I'd encourage you to read that article at some point — it's not technical, and a lot of it will resonate with your teaching background. But the reason I'm mentioning it here is that this plan isn't just about learning to code. It's about building the habits and thinking patterns that make someone genuinely good at this job. Pragmatism is the thread that runs through all of it: choosing the right tool over the fancy tool, knowing when something is good enough to ship, being upfront about what you don't know, and always asking "does this actually solve the problem?"

## What This Plan Covers

I've organized this around two main goals:

1. **Learning to program in TypeScript.** I picked TypeScript because it's everywhere — frontend, backend, cloud functions — and the job market for it is massive. More importantly, its type system forces you to think precisely about data, which is a habit that pays off in every area of engineering.

2. **Learning system design.** This is the one that most self-taught engineers skip, and it's the one that matters most as you grow. System design is how you figure out the architecture of real software — when someone says "build me something that handles 10 million users," system design is how you decide what pieces you need (databases, servers, caches, message queues), how they connect, and what tradeoffs you're making. It's the difference between code that works on your laptop and understanding how products like Instagram or Slack are actually built. It's also a major focus of engineering interviews at every level.

The plan moves through five phases: understanding how computers work, learning to code, picking up the tools engineers use daily, building CS fundamentals, and then going deep on system design. Each phase builds on the last.

**Total timeline:** roughly 6-8 months at 10-15 hours per week. Adjust based on your pace — there's no rush here.

## A Note on Your Background

For what it's worth, one of the best programmers I know has a degree in biology. In fact, most of the best people I work with have non-traditional backgrounds. A CS degree is one path, but it's not the only one — and teaching experience is a real asset in this field. The best engineers I've worked with are the ones who can explain systems clearly, write good documentation, break down complexity for others, and think about sequencing and tradeoffs. That's literally what teachers do every day. You're not starting from zero — you're starting from a different kind of expertise, and it's one that's genuinely rare in engineering.

---

## Phase 0: How Computers Actually Work (1-2 weeks)

Before getting into code, I'd recommend spending a couple weeks building a mental model of what's actually happening when software runs. The goal isn't to go deep — it's just to make sure nothing feels like magic. This is a pragmatic choice: you could skip this and start coding immediately, but every concept later in this plan will land better if you have even a rough picture of how the pieces connect.

**What to cover:**
- How the internet works (DNS, HTTP, client/server)
- What a server is, what a database is, how they talk to each other
- What an API is — I usually explain it as a menu at a restaurant: you make a request, the kitchen (server) prepares it, and you get something back

**Resources:**
- **YouTube:** [Harvard CS50 — Lecture 0](https://www.youtube.com/watch?v=3LPJfIKxwWc) and continue through Lectures 1-4. David Malan is one of the best CS educators out there. No need to do the problem sets, just watch and absorb.
- **YouTube:** [Fireship — Computer Networking in 100 Seconds](https://www.youtube.com/c/Fireship) (short, visual, fast — search his channel for networking/internet videos)
- **YouTube:** [ByteByteGo](https://www.youtube.com/@ByteByteGo) — search for their HTTP and networking explainers

**Milestone:** You can explain to someone what happens when they type a URL into a browser and hit enter.

---

## Phase 1: Programming Fundamentals with TypeScript (6-8 weeks)

I'm recommending TypeScript as a first language for the reasons I mentioned above — it's widely used, it's in demand, and its type system builds good habits early.

### Week 1-2: JavaScript Basics
TypeScript is JavaScript with types added on top, so I'd start with plain JavaScript first.

**What to cover:**
- Variables, data types (string, number, boolean, array, object)
- Functions, conditionals (if/else), loops
- Console.log everything — treat it like a lab notebook

**Resources:**
- **Interactive course:** [The Odin Project — Foundations](https://www.theodinproject.com/paths/foundations) (free, project-based, one of the best beginner resources out there)
- **YouTube:** [JavaScript Tutorial for Beginners — Programming with Mosh](https://www.youtube.com/watch?v=W6NZfCO5SIk) (1hr crash course to get oriented)
- **Free online book:** [Eloquent JavaScript](https://eloquentjavascript.net/) — chapters 1-6 (read alongside the videos)
- **Practice:** [Exercism.org — JavaScript track](https://exercism.org/tracks/javascript) — free, with mentorship built in

### Week 3-4: Deeper JavaScript
**What to cover:**
- Objects and arrays in depth (destructuring, spread, map/filter/reduce)
- Async/await and Promises (how JavaScript handles waiting for things like network requests)
- Modules and imports
- Error handling (try/catch)

**Resources:**
- **YouTube:** [JavaScript Promises In 10 Minutes — Web Dev Simplified](https://www.youtube.com/watch?v=DHvZLI7Db8E)
- **YouTube:** Search "async await" on [Web Dev Simplified's channel](https://www.youtube.com/@WebDevSimplified)
- **Free online book:** Continue [Eloquent JavaScript](https://eloquentjavascript.net/) chapters 7-11
- **Practice:** Build a simple CLI todo app that saves to a JSON file

### Week 5-6: TypeScript Layer
**What to cover:**
- Types, interfaces, enums
- Generics (at a basic level)
- Why types matter (catching bugs before code even runs)
- tsconfig basics

**Resources:**
- **Docs:** [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/) — go section by section, this is the official guide
- **YouTube:** [TypeScript Tutorial — Net Ninja](https://www.youtube.com/playlist?list=PL4cUxeGkcC9gUgr39Q_yD6v-bSyMwKPUI) (playlist, ~2hrs total)
- **Practice:** Convert your todo app from JS to TS. This is where the "aha" moment usually happens — you'll see types catch real mistakes.

### Week 7-8: Build Something Real
- Build a REST API using Express.js + TypeScript
- Connect it to a database (start with SQLite or PostgreSQL)
- CRUD operations (Create, Read, Update, Delete) for a resource that interests you — lesson plans, book reviews, whatever

**Resources:**
- **YouTube:** [Build a REST API with Node.js, Express, and TypeScript — TomDoesTech](https://www.youtube.com/watch?v=BWUi6BS9T5Y)
- **Docs:** [Express.js — Getting Started](https://expressjs.com/en/starter/installing.html)

**Milestone:** You have a working API that stores and retrieves data, and you can explain what each line of code does.

**A note on pragmatism here:** Resist the urge to make this project perfect. Ship something that works, even if it's ugly. One of the biggest traps in engineering is over-polishing something that nobody is using yet. The best engineers I know have a bias toward "good enough to learn from" over "architecturally pristine." You can always improve it later — and you will, once you know more.

---

## Phase 2: Developer Tooling & Workflow (2-3 weeks)

This is the "how engineers actually work day-to-day" layer. AI tools are great, but you need to understand the environment they operate in. This phase might feel tedious compared to actually building things — and honestly, some of it is. But one of the marks of a mature engineer is doing the unglamorous work without complaint. Git, testing, and environment management aren't exciting, but they're what separate someone who can hack something together from someone a team can rely on.

**What to cover:**
- **Git & GitHub** — version control. This is non-negotiable in any engineering job.
- **Terminal/command line** — basic navigation, running scripts
- **Linux fundamentals** — most servers in the world run Linux, and most engineering tools assume you're comfortable in a Unix-like environment. Even if you're on a Mac (which is Unix-based), you need to understand:
  - File system structure (`/etc`, `/var`, `/home`, how paths work)
  - File permissions (`chmod`, `chown`, what `rwx` means)
  - Processes (`ps`, `top`, `kill` — understanding what's running and how to stop it)
  - SSH (how you connect to remote servers)
  - Basic shell scripting (just enough to automate a few steps, not full programs)
  - `grep`, `find`, `cat`, `tail`, `pipe` (`|`) and redirection (`>`, `>>`) — these are the Swiss army knife of debugging and you'll use them every day
- **Package managers** — npm, what node_modules is
- **Environment setup** — .env files, environment variables
- **Testing basics** — writing a simple test with Vitest or Jest

**Resources:**
- **YouTube:** [Git and GitHub for Beginners — freeCodeCamp](https://www.youtube.com/watch?v=RGOj5yH7evk) (1hr)
- **Docs:** [Pro Git — free online](https://git-scm.com/book/en/v2) — chapters 1-3 only
- **Interactive:** [Command Line Crash Course — The Odin Project](https://www.theodinproject.com/lessons/foundations-command-line-basics)
- **Interactive:** [Linux Survival](https://linuxsurvival.com/) — free browser-based tutorial, no setup required. Covers the basics well.
- **YouTube:** Search "Linux for Hackers" by NetworkChuck — he makes it approachable and covers the practical stuff (file system, permissions, SSH, processes)
- **Docs:** [Linux Journey](https://linuxjourney.com/) — free, self-paced, covers everything from the command line through processes and permissions
- **Articles:** Search "Testing JavaScript" by Kent C. Dodds — free intro material on his site

**Milestone:** You push your API project to GitHub with meaningful commit messages and at least 3 tests. You can SSH into a remote server, navigate the file system, check what processes are running, and read a log file.

---

## Phase 3: Computer Science Fundamentals (4-6 weeks)

You don't need a CS degree. But you do need the mental models that a CS education builds. This is the "base layer" that's probably the gap you're feeling.

### Data Structures & Algorithms (light version)
The goal here isn't competitive programming — it's understanding *why* certain choices are made in system design.

**What to cover:**
- Arrays, linked lists, hash maps, trees, graphs (concepts, not building them from scratch)
- Big O notation (just the intuition: "this is fast, this is slow, here's why")
- Common patterns: searching, sorting, recursion

**Resources:**
- **Book:** *Grokking Algorithms* by Aditya Bhargava — illustrated, visual, written specifically for people without a CS background. This would be my #1 recommendation for this phase.
- **YouTube:** [Data Structures Easy to Advanced — William Fiset / freeCodeCamp](https://www.youtube.com/watch?v=RBSGKlAvoiM) (watch at 1.5x, skip anything that feels too deep)
- **Practice:** [NeetCode.io](https://neetcode.io/) — start with the "Easy" problems in the Blind 75 list. Do 2-3 per week in TypeScript.

### Networking & Databases
**What to cover:**
- TCP/IP, HTTP/HTTPS, REST vs GraphQL
- SQL basics (SELECT, JOIN, WHERE, indexes)
- Relational vs NoSQL databases (when to use which)

**Resources:**
- **YouTube:** [SQL Tutorial — Full Database Course — freeCodeCamp](https://www.youtube.com/watch?v=HXV3zeQKqGY) (the first 2 hours are what matters)

**Milestone:** You can explain what a hash map is and why it's fast. You can write a SQL query that joins two tables.

---

## Phase 4: System Design — The Main Event (8-12 weeks)

This is where everything comes together, and where pragmatism matters most. System design is fundamentally about making tradeoffs under constraints — there is no "correct" answer, only a set of options with different costs. Every choice you make (this database over that one, caching here but not there) has consequences, and the job is to make those tradeoffs *explicit* rather than stumbling into them. This is something Allspaw emphasizes in that article I mentioned: immature engineers discover the corners they cut after things break; mature engineers spell them out at the start of a project and accept them as part of the work. If you think about it, teaching is the same — depth vs breadth, individual vs group, time vs quality. You've been making these kinds of calls for years.

### Foundation (Weeks 1-3)
**What to cover:**
- Client-server architecture
- Load balancers, caching, CDNs
- Horizontal vs vertical scaling
- CAP theorem (at a high level)
- Monolith vs microservices
- **Domain-Driven Design (DDD) — light intro.** DDD is a way of thinking about how to structure software around the actual problem you're solving, not around the technology. The core idea is that before you decide *how* to build something, you need to deeply understand the domain — the business, the users, the language they use. You model your code around that language and those concepts. You don't need to go deep here, but understanding the basics (bounded contexts, ubiquitous language, entities vs value objects) will fundamentally change how you approach designing systems. It's one of the most pragmatic frameworks I've seen — it forces you to ask "what problem are we actually solving?" before writing a line of code.

**Resources:**
- **Book:** *Designing Data-Intensive Applications* ("DDIA") by Martin Kleppmann — this is the system design bible in our industry. Start with chapters 1-3. It's dense but incredibly well-written. I'd recommend reading it slowly, one section per sitting.
- **YouTube:** [ByteByteGo](https://www.youtube.com/@ByteByteGo) (Alex Xu) — short, visual explanations of every major concept. I'd watch these *alongside* DDIA to reinforce what you're reading.
- **DDD:** Search YouTube for "Domain-Driven Design Explained" by Amichai Mantinband — good short intro. For more depth later, *Domain-Driven Design Distilled* by Vaughn Vernon is the most accessible book on the topic, but it's not required at this stage.

### Core Patterns (Weeks 4-6)
**What to cover:**
- Database sharding and replication
- Message queues (Kafka, RabbitMQ concepts)
- Rate limiting
- Consistent hashing
- API design patterns

**Resources:**
- **YouTube:** [System Design playlist — Gaurav Sen](https://www.youtube.com/playlist?list=PLMCXHnjXnTnvo6alSjVkgxV-VH6EPyvoX) — great at building intuition
- **YouTube:** [ByteByteGo](https://www.youtube.com/@ByteByteGo) "System Design Interview" series
- **Book:** Continue DDIA chapters 4-9
- **Practice:** For each concept, draw the architecture on paper. Teaching it to yourself is one of the best ways to learn it.

### Real System Walkthroughs (Weeks 7-10)
**What to cover:**
- Design a URL shortener
- Design a chat system
- Design a notification service
- Design a news feed

**Resources:**
- **YouTube:** "System Design Interview" videos by [Exponent](https://www.youtube.com/@tryexponent) (real interview question walkthroughs)
- **YouTube:** Jordan Has No Life channel — deep dives into DDIA concepts with practical examples
- **Practice:** Pick one system per week. Design it on paper first, then watch/read the "answer" and see how your thinking compares. When you review your design against the reference, don't just look at what's different — ask yourself *what tradeoffs did I make, and can I explain why?* That's the skill. There's rarely a single right answer; there's a well-reasoned answer where you can articulate what you'd gain and what you'd give up.

### Cloud & Infrastructure Awareness (Weeks 10-12)
**What to cover:**
- AWS/GCP basics (what S3, EC2, Lambda, RDS are)
- Containers (Docker basics)
- CI/CD concepts
- Observability (logs, metrics, traces — what they are and why they matter)
- **The Twelve-Factor App.** This is a set of principles for building software that deploys and scales cleanly. It covers things like keeping config out of code, treating logs as streams, making services stateless, and keeping dev/prod environments as similar as possible. It was written by the folks at Heroku and it's become the standard playbook for building modern applications. Read through it once — it's short and practical — and then revisit it when you're deploying your projects. You'll start to see why certain decisions are made the way they are in real codebases.

**Resources:**
- **YouTube:** [Top 50+ AWS Services Explained in 10 Minutes — Fireship](https://www.youtube.com/watch?v=JIbIYCM48to)
- **YouTube:** [Docker in 100 Seconds — Fireship](https://www.youtube.com/watch?v=Gjnup-PuquQ)
- **Docs:** [The Twelve-Factor App](https://12factor.net/) — read the whole thing, it's short. Each factor is one page.
- **Free tier:** Sign up for AWS free tier and deploy your Phase 1 API to it

**Milestone:** You can whiteboard the design of a URL shortener — explaining your database choice, how you'd handle millions of requests, and what tradeoffs you're making.

---

## Phase 5: Portfolio & Job Prep (Ongoing alongside Phases 3-4)

### Build 2-3 Projects
1. **Full-stack app** — React + TypeScript frontend, Node/Express backend, PostgreSQL database, deployed somewhere (Vercel, Railway, or AWS)
2. **System design writeup** — pick a real product, write up how you'd design it from scratch. Publish it on a blog or GitHub README.
3. **Open source contribution** — even a small one shows you can navigate and contribute to an existing codebase

### Interview Prep
When you're ready to start interviewing, these are worth picking up:
- **Book:** *Cracking the Coding Interview* by Gayle Laakmann McDowell — the industry standard for coding interview prep. Good to skim for structure and patterns even if you don't grind every problem.
- **Book:** *System Design Interview* Vol 1 & 2 by Alex Xu — you'll already be using these in Phase 4, but they double as direct interview prep since the format mirrors real interviews.
- **Site:** [NeetCode.io](https://neetcode.io/) for algorithm practice
- **Site:** [GreatFrontEnd.com](https://www.greatfrontend.com/) for frontend-specific prep
- **YouTube:** Mock system design interviews on [Exponent's channel](https://www.youtube.com/@tryexponent)

---

## Weekly Schedule Template

I'd suggest something like this as a weekly structure:

| Day | Focus | Time |
|-----|-------|------|
| Mon-Fri | Core learning (current phase) | 1-2 hrs |
| Sat | Build/practice (coding exercises or project work) | 2-3 hrs |
| Sun | Review + system design reading (DDIA or ByteByteGo) | 1 hr |

Adjust to whatever works for your schedule. Consistency matters more than intensity.

---

## The Book Stack (Summary)

If you only buy three books across this entire plan, make it these:

1. **_Grokking Algorithms_ by Aditya Bhargava** (Phase 3) — covers the CS fundamentals gap in the most accessible way I've seen. Visual, no prerequisites, and it builds the mental models that everything else depends on.
2. **_Designing Data-Intensive Applications_ by Martin Kleppmann** (Phase 4) — this is the system design foundation. Once you have basic programming ability, this is the book that teaches you how real systems actually work. Nothing else comes close.
3. **_System Design Interview_ Vol 1 & 2 by Alex Xu** (Phase 4) — where DDIA teaches you the theory, these walk you through solving real-world problems: "design a URL shortener," "design a chat system," etc. It's a good litmus test for whether the concepts are actually clicking, and it's directly useful for interviews.

Everything else in this plan can be learned from YouTube and free online resources. These are worth buying.

