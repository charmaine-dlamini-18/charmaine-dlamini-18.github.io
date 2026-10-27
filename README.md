<style>
:root {
  --navy:#0B2545; --navy-2:#12385A; --teal:#0E9F8E; --teal-dark:#0B7C70;
  --mint:#EAF8F6; --purple:#6C63FF; --amber:#E88B2A; --ink:#1F3A4D;
  --muted:#5B7285; --line:#DCE7EE; --card:#FFFFFF; --bg:#F6FAFC;
}
html { scroll-behavior:smooth; }
body { color:var(--ink); background:linear-gradient(180deg,#F6FAFC 0%,#FFFFFF 340px); padding:16px; }
.markdown-body { max-width:1080px; margin:auto; }
h1, h2, h3, h4 { color:var(--navy); line-height:1.25; }
h1 { letter-spacing:.3px; }
h2 { border-bottom:2px solid var(--line); padding-bottom:.5rem; margin-top:2.6rem; }
h3 { margin-top:1.8rem; }
h4 { margin-top:1.4rem; }
p, li { line-height:1.7; }
a { color:var(--teal-dark); font-weight:600; text-decoration:none; }
a:hover { color:var(--purple); text-decoration:underline; }
hr { height:2px; border:0; background:linear-gradient(90deg,var(--teal),var(--purple),transparent); margin:2rem 0; opacity:.65; }
table { display:table; width:100%; border-collapse:collapse; margin:1.1rem 0 1.6rem; border-radius:10px; overflow:hidden; }
th { background:var(--navy); color:#fff; font-weight:600; }
th, td { padding:11px 13px; border:1px solid var(--line); text-align:left; vertical-align:top; }
tr:nth-child(even) td { background:#F4F9FB; }
tr:hover td { background:#EDF7F6; }
img { max-width:100%; height:auto; border-radius:10px; }
blockquote { border-left:5px solid var(--teal); background:var(--mint); padding:12px 18px; border-radius:0 10px 10px 0; margin:1.2rem 0; }
[id] { scroll-margin-top:24px; }

.portfolio-hero { position:relative; overflow:hidden; background:radial-gradient(120% 120% at 10% 0%, rgba(108,99,255,.55) 0%, transparent 45%), radial-gradient(120% 120% at 90% 10%, rgba(14,159,142,.55) 0%, transparent 45%), linear-gradient(135deg,#0B2545 0%,#124E66 55%,#2E3A8C 100%); color:#fff; padding:46px 24px 40px; border-radius:24px; text-align:center; box-shadow:0 18px 40px rgba(11,37,69,.22); }
.portfolio-hero::before { content:""; position:absolute; inset:-40% -10% auto -10%; height:70%; background:radial-gradient(circle,rgba(255,255,255,.18),transparent 60%); pointer-events:none; }
.portfolio-hero > * { position:relative; z-index:1; }
.portfolio-hero h1 { color:#fff; border:0; margin:18px 0 6px; font-size:2.2rem; letter-spacing:2px; }
.portfolio-hero h3 { color:#CFEFEA; margin:0 0 14px; font-weight:500; }
.portfolio-hero p { color:#EAF4FF; margin:.4rem auto; max-width:760px; }
.hero-tags { display:flex; flex-wrap:wrap; gap:8px; justify-content:center; margin:14px 0 6px; }
.hero-tags span { background:rgba(255,255,255,.14); border:1px solid rgba(255,255,255,.3); color:#fff; padding:6px 12px; border-radius:999px; font-size:.85rem; }
.welcome-top { text-align:center; margin:6px 0 18px; }
.welcome-top h2 { border:0; margin:0; padding:0; font-size:1.7rem; letter-spacing:.5px; }

.portfolio-nav { display:grid; grid-template-columns:repeat(auto-fit,minmax(210px,1fr)); gap:14px; margin:22px 0; }
.portfolio-nav a { display:block; background:#fff; border:1px solid var(--line); border-left:5px solid var(--teal); padding:15px 17px; border-radius:14px; text-decoration:none; color:var(--navy); box-shadow:0 3px 10px rgba(16,42,67,.05); transition:transform .16s ease, box-shadow .16s ease, border-color .16s ease; }
.portfolio-nav a:hover { transform:translateY(-3px); box-shadow:0 12px 24px rgba(16,42,67,.14); color:var(--purple); border-left-color:var(--purple); text-decoration:none; }
.portfolio-nav small { color:var(--muted); display:block; margin-top:3px; font-weight:400; }

.section-banner { background:linear-gradient(135deg,#0B2545,#124E66); color:#fff; border-radius:16px; padding:18px 22px; margin:28px 0 18px; box-shadow:0 10px 24px rgba(11,37,69,.14); }
.section-banner h2 { color:#fff !important; border:0; margin:0; padding:0; font-size:1.5rem; }
.section-banner h1 { color:#fff !important; border:0; margin:0; padding:0; font-size:1.6rem; }
.section-banner.teal { background:linear-gradient(135deg,#0B7C70,#0E9F8E); }
.section-banner.purple { background:linear-gradient(135deg,#4538A8,#6C63FF); }
.section-banner.stories { background:linear-gradient(135deg,#5B2A86,#9B59B6); }
.section-banner.amber { background:linear-gradient(135deg,#A65E12,#E88B2A); }
.section-banner.blue { background:linear-gradient(135deg,#174A7E,#2878C8); }

.note { background:var(--mint); border-left:6px solid var(--teal); padding:16px 20px; border-radius:0 12px 12px 0; margin:16px 0; }
.note h3 { margin-top:0; color:#0B6E64; }

.contact-grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:12px; margin:14px 0; }
.contact-card { display:block; background:#fff; border:1px solid var(--line); border-radius:14px; padding:14px 16px; text-decoration:none; color:var(--navy); box-shadow:0 3px 10px rgba(16,42,67,.05); transition:transform .16s ease, box-shadow .16s ease; }
.contact-card:hover { transform:translateY(-2px); box-shadow:0 10px 20px rgba(16,42,67,.12); text-decoration:none; color:var(--purple); }
.contact-card .label { display:block; font-size:.78rem; text-transform:uppercase; letter-spacing:.08em; color:var(--muted); font-weight:600; margin-bottom:4px; }
.contact-card .value { font-weight:600; word-break:break-word; }

.timeline { border-left:3px solid var(--line); margin:14px 0 6px 8px; padding-left:22px; }
.timeline-item { position:relative; margin:0 0 18px; }
.timeline-item::before { content:""; position:absolute; left:-31px; top:5px; width:12px; height:12px; border-radius:50%; background:var(--teal); box-shadow:0 0 0 4px #E6F6F4; }
.timeline-item h4 { margin:0 0 2px; }
.timeline-item p { margin:2px 0; color:var(--muted); }

.project-card { background:var(--card); border:1px solid var(--line); border-radius:16px; padding:18px 20px; margin:16px 0; box-shadow:0 4px 14px rgba(16,42,67,.06); transition:transform .16s ease, box-shadow .16s ease; }
.project-card:hover { transform:translateY(-2px); box-shadow:0 12px 24px rgba(16,42,67,.12); }
.project-card h4 { margin:0 0 8px; font-size:1.08rem; }
.project-card p { margin:.4rem 0; }
.project-card ul { margin:.6rem 0 .3rem; padding-left:1.2rem; }
.project-card li { margin:.3rem 0; }
.pill { display:inline-block; vertical-align:middle; background:var(--mint); color:var(--teal-dark); border:1px solid #BEE7E2; font-size:.72rem; font-weight:600; padding:2px 10px; border-radius:999px; margin-left:8px; }
.tech-tags { display:flex; flex-wrap:wrap; gap:6px; margin-top:10px; }
.tech-tags span { background:#F1FAF9; color:#0B6E64; border:1px solid #CBEBE7; font-size:.76rem; padding:3px 9px; border-radius:6px; }

.skills { display:grid; grid-template-columns:repeat(auto-fit,minmax(240px,1fr)); gap:14px; margin:14px 0; }
.skill-group { background:#fff; border:1px solid var(--line); border-top:4px solid var(--teal); border-radius:14px; padding:14px 16px; box-shadow:0 3px 10px rgba(16,42,67,.05); }
.skill-group h4 { margin:0 0 10px; }
.chips { display:flex; flex-wrap:wrap; gap:7px; }
.chips span { background:#F1FAF9; color:#0B6E64; border:1px solid #CBEBE7; font-size:.8rem; padding:4px 10px; border-radius:999px; }

.gallery { display:grid; grid-template-columns:repeat(auto-fit,minmax(280px,1fr)); gap:14px; margin:16px 0; }
.gallery figure { margin:0; background:#fff; border:1px solid var(--line); border-radius:14px; padding:10px; box-shadow:0 3px 10px rgba(16,42,67,.05); }
.gallery img { display:block; width:100%; border-radius:10px; }
.gallery figcaption { text-align:center; color:var(--muted); font-size:.82rem; padding:8px 4px 2px; }

.video-frame { background:#0B2545; border-radius:18px; padding:12px; margin:16px 0; box-shadow:0 12px 26px rgba(11,37,69,.18); }
.video-frame video { display:block; width:100%; border-radius:10px; background:#000; }

.back-to-top { position:fixed; right:18px; bottom:18px; z-index:99; width:44px; height:44px; display:flex; align-items:center; justify-content:center; background:var(--navy); color:#fff; border-radius:50%; text-decoration:none; font-size:1.1rem; box-shadow:0 6px 18px rgba(11,37,69,.3); }
.back-to-top:hover { background:var(--purple); color:#fff; text-decoration:none; }

@media (max-width:640px) {
  body { padding:10px; }
  .portfolio-hero { padding:30px 16px 26px; border-radius:18px; }
  .portfolio-hero h1 { font-size:1.55rem; letter-spacing:1px; }
  .portfolio-hero h3 { font-size:1rem; }
  .welcome-top h2 { font-size:1.35rem; }
  .portfolio-nav { grid-template-columns:1fr; }
  th, td { padding:8px; font-size:.9rem; }
}
</style>

<a id="top"></a>

<div class="welcome-top">
  <h2>Welcome to my Portfolio</h2>
</div>

<div class="note">
  <h3 id="career-overview">🚀 Career Overview</h3>
  <p>I am a motivated and dedicated Information Technology final year student majoring in Applications Development, aspiring to become a Backend Developer. I have a strong foundation in software development and problem-solving, with practical skills in Java, Python, web technologies, APIs, and database concepts gained through academic and personal projects. I am committed to continuous learning and professional growth, seeking an entry-level position, internship, or learnership where I can apply my technical and analytical skills to contribute to high-quality software solutions.</p>
</div>

---

## 🧭 Quick Navigation

Use these shortcuts to jump directly to any section of my portfolio.

<div class="portfolio-nav">
  <a href="#cv-and-professional-profile">👩🏽‍💻 <strong>CV &amp; Professional Profile</strong><br><small>Contact, education and career overview</small></a>
  <a href="#technical-skills">🧰 <strong>Technical Skills</strong><br><small>Languages, frameworks and tools</small></a>
  <a href="#work-experience">🚀 <strong>Academic &amp; Personal Projects</strong><br><small>Applications and project experience</small></a>
  <a href="#mock-video-interview">🎥 <strong>Mock Interview</strong><br><small>Recorded interview</small></a>
  <a href="#agile-team-charter--laundrypickuppro">🤝 <strong>Agile Team Charter</strong><br><small>Team vision and agreements</small></a>
  <a href="#user-stories-and-tasks--laundrypickuppro">📝 <strong>User Stories &amp; Tasks</strong><br><small>Work across ten sprints</small></a>
  <a href="#product-backlog">📋 <strong>Product Backlog</strong><br><small>Features and Trello board</small></a>
  <a href="#sprint-backlog">🔄 <strong>Sprint Backlog</strong><br><small>Sprint tasks and screenshots</small></a>
  <a href="#agile-logbooks">📚 <strong>Agile Logbooks</strong><br><small>Progress records and reflections</small></a>
  <a href="#references">📇 <strong>References</strong><br><small>Professional references</small></a>
</div>

---

<h2 id="cv-and-professional-profile">CV and Professional Profile</h2>

<h3 id="contact">📞 Contact</h3>

<div class="contact-grid">
  <a class="contact-card" href="tel:0712025518"><span class="label">Phone</span><span class="value">071 202 5518</span></a>
  <a class="contact-card" href="mailto:222056401@mycput.ac.za"><span class="label">Email</span><span class="value">222056401@mycput.ac.za</span></a>
  <a class="contact-card" href="https://www.linkedin.com/in/charmaine-dlamini"><span class="label">LinkedIn</span><span class="value">charmaine-dlamini</span></a>
  <a class="contact-card" href="https://github.com/charmaine-dlamini-18"><span class="label">GitHub</span><span class="value">charmaine-dlamini-18</span></a>
</div>

📍 Woodstock, Cape Town

---

<h3 id="education">🎓 Education</h3>

<div class="timeline">
  <div class="timeline-item">
    <h4>Cape Peninsula University of Technology (CPUT)</h4>
    <p>Diploma of ICT in Applications Development · Final Year</p>
  </div>
  <div class="timeline-item">
    <h4>Mlonde High School</h4>
    <p>National Senior Certificate · Matric (Grade 12) · 2021</p>
  </div>
</div>

---

<h3 id="work-experience">💼 Work Experience</h3>

#### Academic &amp; Personal Projects (2024–Present)

<div class="project-card">
  <h4>MediQueue Clinic System <span class="pill">Ongoing</span></h4>
  <p>A clinic management system designed to streamline patient appointments, queue management, and staff workflow.</p>
  <ul>
    <li>Enables patients to book and manage appointments online.</li>
    <li>Provides real-time queue tracking for doctors and receptionists.</li>
    <li>Includes secure patient record management and reporting features.</li>
  </ul>
  <div class="tech-tags"><span>Web Technologies</span><span>OOP</span><span>SQL</span></div>
</div>

<div class="project-card">
  <h4>LaundryPickupPro <span class="pill">Agile Team Project</span></h4>
  <p>A laundry pick-up and drop-off platform for residents in Maitland, Observatory, and Woodstock.</p>
  <ul>
    <li>Enables customers to book services, schedule pickups, and track their orders.</li>
    <li>Includes secure authentication, payments, driver dashboards, and admin management screens.</li>
    <li>Built through ten Agile sprints with user stories, testing, debugging, and deployment.</li>
  </ul>
  <div class="tech-tags"><span>React Native</span><span>Supabase</span><span>Agile</span></div>
</div>

<div class="project-card">
  <h4>Password Vault Application</h4>
  <p>A secure password management tool for storing and retrieving passwords safely.</p>
  <ul>
    <li>Implements encryption and secure storage mechanisms.</li>
    <li>Provides a user-friendly interface for easy password management.</li>
    <li>Applies core software development practices.</li>
  </ul>
</div>

<div class="project-card">
  <h4>Room Tracker Desktop Application</h4>
  <p>A multi-user system to track campus room availability.</p>
  <ul>
    <li>Includes login, signup, and admin panel features.</li>
    <li>Manages client-server communication, network programming, and persistent database storage.</li>
    <li>Applies object-oriented design principles and iterative development.</li>
  </ul>
</div>

<div class="project-card">
  <h4>Student Enrolment System <span class="pill">Java Client–Server</span></h4>
  <p>An enrolment application with admin and student roles and secure authentication.</p>
  <ul>
    <li>Designed a Swing GUI for course management and enrolment.</li>
    <li>Integrated a Derby database using JDBC.</li>
    <li>Built client-server communication using sockets and serialization.</li>
  </ul>
</div>

<div class="project-card">
  <h4>ISbani Youth Development</h4>
  <p>A non-government organisation website designed for youth outreach and community engagement.</p>
  <ul>
    <li>Focused on accessibility and usability.</li>
  </ul>
  <div class="tech-tags"><span>HTML</span><span>CSS</span><span>JavaScript</span></div>
</div>

<div class="project-card">
  <h4>Startup Simulator</h4>
  <p>An engaging business simulator game that challenges players to build and manage a thriving startup.</p>
  <ul>
    <li>Features interactive gameplay and strategic decision-making.</li>
    <li>Includes dynamic interfaces and game logic for realistic simulation.</li>
  </ul>
  <div class="tech-tags"><span>HTML</span><span>CSS</span><span>JavaScript</span></div>
</div>

---

<h3 id="technical-skills">🛠️ Technical Skills</h3>

<div class="skills">
  <div class="skill-group">
    <h4>Languages</h4>
    <div class="chips"><span>Java</span><span>Python</span><span>HTML</span><span>CSS</span><span>JavaScript</span><span>PHP</span><span>SQL / MySQL</span></div>
  </div>
  <div class="skill-group">
    <h4>Frameworks &amp; APIs</h4>
    <div class="chips"><span>FastAPI</span><span>REST API</span><span>Spring Boot</span><span>React Native</span><span>Node.js</span><span>Next.js</span><span>Laravel</span></div>
  </div>
  <div class="skill-group">
    <h4>Tools &amp; IDEs</h4>
    <div class="chips"><span>Apache NetBeans</span><span>IntelliJ</span><span>Figma</span><span>VS Code</span><span>Thonny</span><span>PyCharm</span></div>
  </div>
</div>

---

<h3 id="mock-video-interview">🎥 Mock Video Interview</h3>

<div class="video-frame">
  <video controls preload="metadata">
    <source src="video/Mock-interview-video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

---

### **Reflection on Coding in Markdown**
**Situation:**  
During this project, I was required to create and format my CV using Markdown as part of my GitHub portfolio. I had limited prior experience using Markdown for structuring professional documents.  

**Task:**  
My task was to write a well-structured and readable CV using Markdown syntax while ensuring it was properly displayed on my GitHub Pages site.  

**Action:**  
I learned and applied Markdown syntax such as headings, bullet points, bold text, and links to organise my CV content. I structured sections like education, skills, and experience clearly to improve readability. I also tested how the Markdown rendered on GitHub and adjusted where formatting did not appear as expected.  

**Result:**  
As a result, I was able to create a clean, structured, and professional-looking CV. I improved my understanding of Markdown and how it can be used for documentation. This skill will be useful in future projects, especially when working with README files and technical documentation.  

---

### **Reflection on Using GitHub Pages**
**Situation:**  
As part of this assignment, I was required to publish my portfolio using GitHub Pages. The portfolio included my CV coded in Markdown and my mock interview.  

**Task:**  
My task was to deploy my portfolio online using GitHub Pages and make sure that my CV and mock interview were accessible and displayed correctly.  

**Action:**  
I created a GitHub repository and added my CV written in Markdown as well as the mock interview. I then enabled GitHub Pages to publish the site. During the process, I experienced challenges with getting the content to display correctly and ensuring updates reflected on the live site. I checked my commits, refreshed the page, and ensured everything was properly uploaded.  

**Result:**  
In the end, I successfully published my portfolio and accessed it online. I gained a better understanding of how GitHub Pages works and how to deploy content. This experience improved my confidence in using GitHub and publishing work online.  

---

### **Reflection on Mock Interview**
**Situation:**  
As part of this project, I had to complete a mock interview to simulate a real-life IT job interview. This was my first time doing a recorded interview, and I felt stressed and nervous.  

**Task:**  
My task was to answer interview questions clearly and professionally within a limited time of 2 minutes while demonstrating confidence and communication skills. The questions were divided into behavioural, situational, technical, and general categories, and I had to choose one question from each category and understand what each required before answering.  

**Action:**  
I prepared by reviewing common interview questions and planning my responses. However, during the interview, I struggled with time management and keeping my answers within the 2-minute limit. I also found it difficult to structure my answers clearly under pressure.  

**Result:**  
This experience helped me identify areas for improvement, particularly in confidence, time management, and structuring answers. I now understand the importance of staying calm and organising my thoughts before responding. Although I faced challenges, I feel more prepared for future interviews.

---

<div class="section-banner purple" id="agile-team-charter--laundrypickuppro">
<h2>🤝 Agile Team Charter – LaundryPickupPro</h2>
</div>

[View Agile Team Charter (PDF)](Agile%20Team%20Charter.pdf)

## 1. Team Purpose & Vision

### Why do we exist as a team?

We exist to design and develop a solution that addresses the lack of convenient laundry access for residents in Maitland, Observatory, and Woodstock.

**Team mission:**

To create a reliable and affordable laundry pick-up and drop-off service that saves time, reduces effort, and improves the daily lives of residents. We are solving the problem of inconvenient and inaccessible laundry services for working adults with busy schedules, elderly residents who struggle with physical tasks, and people living in apartments without laundry facilities.

**Success definition:**

We will be successful when our final product is:

- Fully developed and functional.
- The solution clearly addresses the problem people are facing.
- The system is usable, practical and meets user needs.

**Product / Service:**

We are responsible for delivering a laundry pick-up and drop-off service that includes:

- Booking system.
- Laundry collection and delivery process.
- Integration with laundromat owners.
- Affordable prices.
- Convenient scheduling.

---

## 2. Team Members & Roles

### Who is on the team and how do we contribute?

| Name | Role | Key Responsibilities |
|---|---|---|
| Imaan Achmat | Product Owner | Comes up with the main idea, keeps the backlog organised and decides what should be done first. Focuses on making sure the team builds something useful that people need. |
| Sabelo Ceza | Agile Lead | Keeps the team organised, ensures everyone knows what to work on, leads meetings, helps solve problems, and makes sure the team stays on track. |
| Zacharia Dipudi | UI/UX Designer | Makes sure the app is simple and easy to use. Plans user navigation and designs screens before coding starts. |
| Charmaine Dlamini | Developer / Analyst / Tester | Builds the system, helps determine how features should work, tests features, and fixes bugs to ensure the system runs smoothly. |

---

## 3. Ways of Working

### How we work together day to day

### 3.1 Agile Framework

Our team follows the Agile methodology. We use a product backlog to list and prioritise tasks, and a logbook to track task progress, updates, and team contributions.

### 3.2 Ceremonies

| Ceremony | Frequency | Purpose |
|---|---|---|
| Daily Stand-up | Every working day | Share completed work, current tasks, and any challenges or obstacles. |
| Planning | Once a week | Plan upcoming tasks, assign responsibilities, and set priorities for the week. |
| Review / Demo | End of each milestone or sprint | Show completed tasks and gather feedback from team members. |
| Retrospective | After each milestone or sprint | Reflect on what went well, challenges faced, and how the team can improve. |

---

## 4. Working Agreements

### Rules we agree to follow as a team

- We show up prepared and on time.
- We respect timeboxes and deadlines.
- We give constructive feedback respectfully.
- We raise challenges early to avoid delays.
- We commit to continuous improvement.
- We communicate regularly through group chat or meetings.
- We complete assigned tasks before deadlines.
- We support each other when challenges arise.
- We keep project files and documentation updated.
- We check our work after completing tasks to make sure everything aligns.

---

## 5. Communication

### How and when we communicate

**Primary channels:**

- **Microsoft Teams:** Used for regular meetings, quick updates, daily stand-ups, and screen sharing when needed.
- **WhatsApp:** Used for urgent messages and frequent communication.
- **Email:** Used for formal communication, reports, and document sharing.

**Response-time expectations:**

- During core hours (08:00–17:00, Monday–Friday), messages should receive a response within 1–2 hours.
- Urgent messages, including those marked urgent or sent via WhatsApp, should receive a response within 30 minutes.
- Non-urgent communication may receive a response within 12 hours.

**Remote / hybrid norms:**

- Team members should be available online during core hours.
- Cameras should be on during important meetings but are optional for casual check-ins.
- Team members must maintain clear status updates on Teams, such as available, busy, or offline.
- If unavailable, team members should notify the team ahead of time.

---

## 6. Decision-Making

### How decisions are made

- [ ] Consensus
- [ ] Team vote

The team will aim for consensus where possible. If an agreement cannot be reached, a majority vote will be used to make the final decision.

**Escalation path if we're stuck:**

- Discuss the issues as a team.
- Revisit our project goals.
- Seek guidance from our lecturer if needed.

---

## 7. Definition of Done (DoD)

### When is work really "done"?

- When the application is fully developed and working as intended.
- When the application clearly addresses the problem it was designed to solve.
- When the application is usable, practical, and meets user needs.
- When all tests have been completed successfully and the system runs without errors.
- When the project documentation is updated.
- When the Product Owner has approved the work.
- When the system/application is deployed to the agreed environment.
- When there are no critical bugs or issues found.

---

## 8. Core Values & Behaviours

### How we treat each other

- **Respect:** Every team member is treated with dignity. We listen to others' opinions and value everyone's contributions, regardless of their role.
- **Transparency:** We communicate openly and honestly and share information so everyone stays informed about decisions and progress.
- **Accountability:** We take responsibility for completing tasks, meeting deadlines, and owning our successes and failures.
- **Trust:** We trust each other to complete our work, help one another, and create a safe environment where everyone can confidently share ideas.
- **Learning mindset:** We remain open to feedback, improve our skills, and treat challenges and mistakes as opportunities to learn and grow.
- **Collaboration:** We share ideas and support one another to achieve project goals, recognising that combining our strengths leads to better results.

---

## 9. Risks & Constraints

### What could impact our success?

### Known risks

- Team members may miss deadlines due to academic workload.
- Miscommunication between team members may cause confusion.
- Technical issues or bugs may delay development.
- Team members may have conflicting schedules for meetings or collaboration.
- Delayed tasks may affect the overall project timeline and progress.
- Lack of user feedback could affect the quality of the final product.

### Dependencies

- Availability and commitment of all team members.
- Access to reliable internet and development tools, such as IDEs, GitHub, and database tools.
- Access to a working database and hosting platform.
- Timely feedback from users or test participants.
- Lecturer guidance and approval at different stages of the project.

### Constraints (time, budget, tools, skills)

- Limited time due to the academic schedule and other module deadlines.
- No budget, meaning reliance on free tools and platforms.
- Limited access to advanced development tools.
- Varying skill levels within the team, with some members still learning certain technologies.
- Dependence on free hosting or university resources that may have restrictions.

---

## 10. Review & Improvement

### Keeping the charter alive

**Charter reviewed every:**

- [ ] Retrospective

Our team will review and update the charter during retrospectives to ensure it remains relevant and aligned with our project progress.

**Last updated:** 04 May 2026

---

## 11. Goals and Milestones

### SMART Goals

- Develop a user-friendly laundry pick-up and drop-off service platform that allows customers to book services, schedule pickups, and track orders before the end of the project timeline.
- Ensure that our app is affordable and practical for residents by focusing on convenience and accessibility.
- Test the app properly before deployment to make sure all features work correctly and users can navigate the system easily.
- Complete all planned project tasks within the given project timeline and contribute effectively as a team throughout the development process.

### Project Milestones

| Milestone | Description | Target Date |
|---|---|---|
| Project Planning | Define project scope, goals, requirements, and team responsibilities. | Week 1 |
| Requirements Gathering | Conduct research and gather user and business requirements. | Week 2 |
| UI/UX Design | Create wireframes, interface designs, and user navigation flow. | Week 3 |
| Coding/Implementation | Begin developing the core system structure, screens, and basic functionality. | Week 4 |
| Database Design & Setup | Design and create the database structure for customers, bookings, and deliveries. | Week 5 |
| System Integration | Integrate frontend, backend, and database components. | Week 6 |
| Testing & Bug Fixing | Perform functionality testing and resolve identified issues. | Week 7 |
| Final Review & Deployment | Prepare the final system, documentation, and presentation. | Week 8 |

---

## Reflection on Agile Team Charter

**Situation:**

As part of the LaundryPickupPro project, our team needed a clear agreement on how we would work together, communicate, share responsibilities, and complete our project tasks.

**Task:**

My responsibility was to contribute to the development process while helping ensure that the team's working agreements, risks, and constraints were clearly documented.

**Action:**

I contributed to defining the team's working agreements and identifying risks and constraints that could affect our progress. We also documented our Agile practices, communication channels, milestones, and expectations for completing and reviewing tasks.

**Result:**

The Agile Team Charter provided a shared understanding of team responsibilities, communication expectations, project goals, and ways of working. It helped us organise our work, identify possible challenges, and maintain a common direction throughout the project.

The Agile Team Charter also helped me better understand Agile practices, accountability, communication, and the importance of planning and testing in software development. This experience showed me how a well-organised team can work together towards delivering a functional application within a given timeline.

---


<div class="section-banner stories" id="user-stories-and-tasks--laundrypickuppro">
<h1>📝 User Stories and Tasks – LaundryPickupPro</h1>
</div>

---

## Sprint 1

### Sprint 1 – Day 1: Problem Definition

**User Story:**

As a member of the team, I want to clearly define the problem our service aims to solve so that we can build a solution that addresses our target customers' needs and provides value to the business.

**Due date:** May 18, 10:44 PM

**Tasks:**
- Identify the problem – Charmaine Dlamini
- Problem objectives – Zacharia Dipudi
- Problem scope – Wendy Bayise
- Identify key problem areas – Imaan Achmat
- Identify target audience – Sabelo Ceza

---

### Sprint 1 – Day 2: Agile Team Charter

**User Story:**

As a member of the team, I want to create an Agile Team Charter so that everyone understands the project's purpose, vision, roles, responsibilities, and team commitments.

**Due date:** May 19, 8:44 AM

**Tasks:**
- Purpose and vision – Sabelo Ceza
- Core values and behaviours – Imaan Achmat
- Definition of Done – Wendy Bayise
- Role assignment – Charmaine Dlamini
- Team commitments – Zacharia Dipudi

---

### Sprint 1 – Day 3: Communication Plan

**User Story:**

As a member of the team, I want to create a communication plan so that everyone knows how, when, and where we will communicate, collaborate, and share project information as a group.

**Due date:** May 20, 8:44 AM

**Tasks:**
- Identify communication tools – Charmaine Dlamini
- Document communication plan – Wendy Bayise
- Communication responsibilities – Zacharia Dipudi
- Establish communication schedule – Imaan Achmat
- Establish feedback process – Sabelo Ceza

---

### Sprint 1 – Day 4: Conduct User Research

**User Story:**

As a member of the team, I want to conduct user research so that we can understand the needs of our customers and target market and develop a service that meets their expectations.

**Customer User Story:**

As a potential customer, I want to complete a survey questionnaire so that I can share my laundry needs, preferences, and expectations to help improve the service.

**Due date:** May 21, 8:44 AM

**Tasks:**
- Prepare research questions – Imaan Achmat
- Create survey questionnaire – Sabelo Ceza
- Distribute survey – Zacharia Dipudi
- Define user requirements – Charmaine Dlamini
- Compile research report – Wendy Bayise

---

### Sprint 1 – Day 5: Summary of Findings

**User Story:**

As a member of the team, I want to analyse, summarise, and organise the research findings so that we can identify user needs and improve our service.

**Due date:** May 22, 8:44 AM

**Tasks:**
- Identify user needs – Zacharia Dipudi
- Analyse survey responses – Charmaine Dlamini
- Review research results – Imaan Achmat
- Organise collected data – Sabelo Ceza
- Summarise key findings – Wendy Bayise

---

## Sprint 2

### Sprint 2 – Day 1: Competitor Analysis

**User Story:**

As a business owner, I want to analyse competitors and define the value proposition so that the service can compete effectively in the market.

**Due date:** May 25, 5:00 PM

**Tasks:**
- Identify competitors – Wendy Bayise
- Competitor comparison – Charmaine Dlamini
- Analyse strengths and weaknesses – Imaan Achmat
- Identify market gaps – Sabelo Ceza
- Document findings – Zacharia Dipudi

---

### Sprint 2 – Day 2: Project Feasibility

**User Story:**

As a business owner, I want to identify the required resources, estimate project costs, and evaluate the project's feasibility so that I can determine whether the laundry pickup and drop-off service is practical, affordable, and viable to implement.

**Due date:** May 26, 9:00 AM

**Tasks:**
- Identify the required resources – Wendy Bayise
- Estimate product costs – Charmaine Dlamini
- Evaluate project viability – Zacharia Dipudi
- Document feasibility findings – Sabelo Ceza
- Review feasibility results – Imaan Achmat

---

### Sprint 2 – Day 3: Project Risk Analysis

**User Story:**

As a business owner, I want to identify and assess potential project risks so that I can develop strategies to reduce potential problems and make informed decisions.

**Due date:** May 27, 8:44 AM

**Tasks:**
- Market risk – Imaan Achmat
- Financial risk – Wendy Bayise
- Operational risk – Zacharia Dipudi
- Technical risk – Sabelo Ceza
- Document risk mitigation plan – Charmaine Dlamini

---

### Sprint 2 – Day 4: Marketing Strategy

**User Story:**

As a business owner, I want to create a marketing strategy so that more people know about our service.

**Due date:** May 28, 8:44 AM

**Tasks:**
- Create marketing plan – Charmaine Dlamini
- Choose marketing channels – Zacharia Dipudi
- Set marketing budget – Sabelo Ceza
- Plan promotional campaigns – Wendy Bayise
- Research marketing methods and channels – Imaan Achmat

---

### Sprint 2 – Day 5: Value Proposition

**User Story:**

As a business owner, I want to define the value proposition so that our service stands out from competitors and attracts more customers.

**Due date:** May 29, 9:00 AM

**Tasks:**
- Define the business's unique value – Imaan Achmat
- Emotional benefit – Zacharia Dipudi
- Functional benefit – Sabelo Ceza
- Financial/time-saving benefit – Charmaine Dlamini
- Document findings – Wendy Bayise

---

### Sprint 2 – Day 6: Requirements Document (Functional and Non-Functional)

**User Story:**

As a business owner, I want to define and document the functional and non-functional requirements so that the development team understands what needs to be built.

**Due date:** May 30, 9:00 AM

**Tasks:**
- Identify functional and non-functional requirements – Wendy Bayise
- Validate all requirements – Charmaine Dlamini
- Prioritise requirements – Imaan Achmat
- Compile and review findings – Zacharia Dipudi
- Finalise requirements document – Sabelo Ceza

---

## Sprint 3

### Sprint 3 – Day 1: Work Breakdown Structure (WBS)

**User Story:**

As a project manager, I want to create a Work Breakdown Structure so that the project is organised into manageable tasks and completed efficiently.

**Due date:** June 1, 9:00 AM

**Tasks:**
- Identify major project deliverables – Charmaine Dlamini
- Identify project milestones – Sabelo Ceza
- Break deliverables into smaller tasks – Sabelo Ceza
- Categorise tasks – Zacharia Dipudi
- Identify task dependencies – Imaan Achmat
- Assign responsibilities – Imaan Achmat
- Set task durations – Wendy Bayise
- Review WBS – Zacharia Dipudi and Wendy Bayise
- Finalise WBS – Charmaine Dlamini

---

### Sprint 3 – Day 2: Sprint Plans

**User Story:**

As a Scrum Master, I want to create sprint plans so that the team clearly understands the sprint goals and the tasks to be completed.

**Due date:** June 2, 9:00 AM

**Tasks:**
- Define sprint goals – Sabelo Ceza
- Create sprint backlog – Zacharia Dipudi
- Prioritise sprint tasks – Charmaine Dlamini
- Assess team capacity – Imaan Achmat
- Review and finalise sprint plan – Wendy Bayise

---

### Sprint 3 – Day 3: User Stories

**User Story:**

As a project manager, I want to create user stories so that the team clearly understands the project requirements and deliverables.

**Due date:** June 4, 9:00 AM

**Tasks:**
- Identify system users – Imaan Achmat
- Write user stories – Wendy Bayise
- Define acceptance criteria – Sabelo Ceza
- Review user stories – Charmaine Dlamini
- Double-check and finalise user stories – Zacharia Dipudi

---

### Sprint 3 – Day 4: UML Diagrams

**User Story:**

As a software developer, I want to create UML diagrams so that I can clearly understand the system's structure and functionality before development begins.

**Due date:** June 8, 9:00 AM

**Tasks:**
- Draw use case diagram – Sabelo Ceza
- Draw activity diagram – Charmaine Dlamini
- Draw sequence diagram – Wendy Bayise
- Draw class diagram – Imaan Achmat
- Review and finalise UML diagrams – Zacharia Dipudi

---

### Sprint 3 – Day 5: Progress Report

**User Story:**

As a business owner, I want to review a progress report so that I can monitor the project's progress and make changes if needed.

**Due date:** June 9, 9:00 AM

**Tasks:**
- Record sprint achievements – Sabelo Ceza
- Summarise completed tasks – Zacharia Dipudi
- Identify challenges – Wendy Bayise
- Document solutions – Charmaine Dlamini
- Update project progress and finalise progress report – Imaan Achmat

---

## Sprint 4

### Sprint 4 – Day 1: PowerPoint Presentation Slides

**User Story:**

As a member of the team, I want to prepare a business overview PowerPoint presentation so that we can clearly present our business idea to the lecturer.

**Due date:** July 14, 9:00 AM

**Tasks:**
- Gather all the required content and information – Zacharia Dipudi
- Create presentation slides – Sabelo Ceza
- Explain key features – Wendy Bayise
- Review and finalise content – Charmaine Dlamini
- Finalise presentation slides – Imaan Achmat

---

### Sprint 4 – Day 2: Business Overview and Problem Statement

**User Story:**

As a member of this team, I want to create a business overview and problem statement so that everyone understands our project.

**Due date:** July 15, 7:00 PM

**Tasks:**
- Research business background – Sabelo Ceza
- Define the business overview – Charmaine Dlamini
- Identify the problem statement – Imaan Achmat
- Identify target audience – Wendy Bayise
- Review and refine content – Zacharia Dipudi

---

### Sprint 4 – Day 3: Presentation Delivery

**User Story:**

As a member of the team, I want to deliver the business overview presentation so that the lecturer understands our business and provides feedback.

**Due date:** July 16, 8:44 AM

**Tasks:**
- Assign presenters – Sabelo Ceza
- Schedule rehearsal – Charmaine Dlamini
- Practise presentation – Imaan Achmat and Wendy Bayise
- Make final improvements – Zacharia Dipudi
- Present to the lecturer – Imaan Achmat and Wendy Bayise

---

### Sprint 4 – Day 4: Presentation Update

**User Story:**

As a member of the team, I want to update the PowerPoint presentation so that we can improve it based on the lecturer's feedback.

**Due date:** July 17, 9:00 AM

**Tasks:**
- Review presentation content – Wendy Bayise
- Collect team feedback – Imaan Achmat
- Update presentation slides – Sabelo Ceza
- Review and finalise presentation – Charmaine Dlamini
- Presentation submission – Zacharia Dipudi, Charmaine Dlamini, Imaan Achmat, Wendy Bayise, and Sabelo Ceza

---

## Sprint 5

### Sprint 5 – Day 1: Trello Board Setup and Management

**User Story:**

As a Scrum Master, I want to set up and manage the Trello board so that the team can track sprint progress and manage tasks effectively.

**Due date:** July 21, 10:23 PM

**Tasks:**
- Organise the project into clear tasks and subtasks – Sabelo Ceza
- Group tasks into the correct stages of the project – Imaan Achmat
- Add deadlines, priorities, and task details – Wendy Bayise
- Track the progress of each task and update its status – Charmaine Dlamini
- Review the board regularly and improve the task plan when needed – Zacharia Dipudi

---

### Sprint 5 – Day 2: Application Features

**User Story:**

As a Product Owner, I want to define the application features so that the development team has a clear understanding of the functionality to implement.

**Due date:** July 24, 10:23 PM

**Tasks:**
- Brainstorm core features – Charmaine Dlamini
- Define feature requirements – Wendy Bayise
- Prioritise features – Zacharia Dipudi
- List optional features – Imaan Achmat
- Review and finalise feature list – Sabelo Ceza

---

### Sprint 5 – Day 3: Low-Fidelity Wireframes

**Development Team User Story:**

As a member of the team, I want to create the application's low-fidelity wireframes so that the team has a clear visual representation of the system's layout and user interface before development begins.

**Target Audience/Customer User Story:**

As a working professional, I want to use an easy-to-navigate laundry pickup and delivery application so that I can book and manage my laundry services quickly and conveniently without disrupting my busy schedule.

**Due date:** July 28, 10:23 PM

**Tasks:**
- Identify required application screens – Charmaine Dlamini
- Sketch low-fidelity wireframes – Zacharia Dipudi
- Define screen layout – Sabelo Ceza
- Review wireframes – Imaan Achmat
- Update low-fidelity wireframes based on team feedback – Wendy Bayise

---

### Sprint 5 – Day 4: High-Fidelity User Interface Design (UI/UX)

**User Story:**

As a UI/UX designer, I want to create a simple and attractive high-fidelity application design so that users can easily use the application.

**Due date:** July 29, 10:23 PM

**Tasks:**
- Select colour scheme, fonts, and icons – Wendy Bayise
- Design detailed user interface screens – Charmaine Dlamini
- Create consistent design style – Zacharia Dipudi
- Review UI designs – Imaan Achmat
- Improve user experience – Sabelo Ceza

---

## Sprint 6

### Sprint 6 – Day 1: Interactive Figma Prototype

**Team Member User Story:**

As a team member, I want to create a working prototype so that we can show how the application will work and look before we start building it.

**Customer User Story:**

As a customer, I want to try a prototype of the application so that I can check if it is simple and easy to use before it is implemented.

**Due date:** July 31, 10:23 PM

**Tasks:**
- Create clickable prototype – Sabelo Ceza
- Add screen interactions – Charmaine Dlamini
- Test the prototype flow – Wendy Bayise
- Collect feedback – Imaan Achmat
- Improve prototype based on feedback – Zacharia Dipudi

---

### Sprint 6 – Day 2: Prototype Testing

**User Story:**

As a member of this team, I want to test the prototype so that we can identify and fix any usability issues before development.

**Due date:** August 1, 3:50 PM

**Tasks:**
- Test screen navigation – Sabelo Ceza
- Test interactive elements – Charmaine Dlamini
- Identify usability issues – Wendy Bayise
- Collect team feedback – Imaan Achmat
- Record testing results – Zacharia Dipudi

---

### Sprint 6 – Day 3: Prototype Demonstration

**User Story:**

As a member of this team, I want to demonstrate this prototype so that users can review the design and provide feedback.

**Due date:** August 2, 3:50 PM

**Tasks:**
- Prepare prototype walkthrough – Sabelo Ceza
- Demonstrate application features – Charmaine Dlamini
- Explain user flow – Wendy Bayise
- Gather lecturer feedback – Zacharia Dipudi
- Record improvement suggestions – Imaan Achmat

---

### Sprint 6 – Day 4: Prototype Improvements

**Team Member User Story:**

As a member of this team, I want to improve the prototype based on feedback so that the application is ready for the next stage of development.

**Customer User Story:**

As a customer, I want an easy-to-use and visually appealing application so that I can complete my tasks quickly and without confusion.

**Due date:** August 3, 3:50 PM

**Tasks:**
- Apply lecturer feedback – Sabelo Ceza
- Improve screen navigation – Wendy Bayise
- Fix prototype issues – Charmaine Dlamini
- Improve user experience – Zacharia Dipudi
- Finalise prototype – Imaan Achmat

---

## Sprint 7

### Sprint 7 – Day 1: Database Planning

**Database Administrator User Story:**

As a database administrator, I want to plan the database structure so that the application stores and manages data efficiently, securely, and accurately.

**Customer User Story:**

As a customer, I want my personal information and laundry orders to be stored securely so that I can trust the application with my details.

**Due date:** August 4, 9:00 AM

**Tasks:**
- List database tables with attributes – Wendy Bayise
- Identify entities and relationships – Imaan Achmat
- Create ERD/tables – Zacharia Dipudi
- Define primary and foreign keys – Sabelo Ceza
- Document database planning requirements – Charmaine Dlamini

---

### Sprint 7 – Day 2: Authentication Planning

**User Story:**

As a resident (customer), I want to log in securely so that my personal information and orders are protected.

**Due date:** August 5, 9:00 AM

**Tasks:**
- Identify authentication requirements – Wendy Bayise
- Define password and account security rules – Charmaine Dlamini
- Define user roles and access levels – Zacharia Dipudi
- Research and select authentication method – Imaan Achmat
- Review and finalise authentication plan – Sabelo Ceza

---

### Sprint 7 – Day 3: Security Planning

**User Story:**

As a system analyst, I want to plan the application's security measures so that user data and system resources are protected from unauthorised access and potential security threats.

**Due date:** August 6, 9:00 AM

**Tasks:**
- Security requirements – Zacharia Dipudi
- Plan user account and personal data security – Wendy Bayise
- Plan backup and recovery – Imaan Achmat
- Plan secure payment handling – Sabelo Ceza
- Review and finalise security plan – Charmaine Dlamini

---

### Sprint 7 – Day 4: Database Review and Finalisation

**User Story:**

As a database administrator, I want to review and finalise the database design so that it is accurate, complete, and ready for implementation.

**Due date:** August 7, 9:00 AM

**Tasks:**
- Review the database schema – Charmaine Dlamini
- Review ERD/tables – Zacharia Dipudi
- Verify table relationships and constraints – Imaan Achmat
- Apply team feedback and make improvements – Sabelo Ceza
- Finalise database design – Wendy Bayise

---

## Sprint 8

### Sprint 8 – Day 1: Project and GitHub Setup

**User Story:**

As a team member, I want to set up the project and GitHub repository so that the team can collaborate efficiently and maintain version control throughout the project.

**Due date:** August 7, 10:00 PM

**Tasks:**
- Project and GitHub repository creation – Charmaine Dlamini
- Set up Supabase backend integration – Sabelo Ceza
- Project structure and navigation setup – Imaan Achmat
- Project documentation – Zacharia Dipudi
- Application configuration and dependency installation – Wendy Bayise

---

### Sprint 8 – Day 2: Screen Design

**User Story:**

As a software developer, I want to design the application screens so that users have a consistent, intuitive, and visually appealing interface to interact with the system.

**Due date:** August 10, 9:00 AM

**Tasks:**
- Registration and login screen – Charmaine Dlamini
- Landing screen – Wendy Bayise
- User home screen – Imaan Achmat
- Pickup and delivery address screen – Zacharia Dipudi
- Profile screen – Sabelo Ceza

---

### Sprint 8 – Day 3: Screen Design

**User Story:**

As a customer, I want well-designed application screens so that I can easily navigate the system and complete my laundry bookings without confusion.

**Due date:** August 14, 9:00 AM

**Tasks:**
- Forgot password and reset screen – Charmaine Dlamini
- Booking screen and functionality – Imaan Achmat
- Order details and confirmation screen – Zacharia Dipudi
- Order history screen – Wendy Bayise
- Edit profile screen – Sabelo Ceza

---

### Sprint 8 – Day 4: Screen Design

**Driver User Story:**

As a driver, I want a dashboard that displays my assigned pickups and deliveries so that I can efficiently manage my daily routes and update order statuses.

**Customer User Story:**

As a customer, I want to make secure payments through the application so that my payment information is protected and my booking is completed safely.

**Due date:** August 17, 9:00 AM

**Tasks:**
- Payment screen and functionality – Zacharia Dipudi
- Live order tracking screen and functionality – Imaan Achmat
- Notifications screen and functionality – Wendy Bayise
- Help and support screen and functionality – Charmaine Dlamini
- Driver dashboard – Sabelo Ceza

---

### Sprint 8 – Day 5: Screen Design

**User Story:**

As an administrator, I want clear and organised management screens so that I can manage customer accounts, orders, and deliveries efficiently while assisting users when needed.

**Due date:** August 19, 9:00 AM

**Tasks:**
- Admin dashboard – Charmaine Dlamini
- Customer management screen and functionality – Imaan Achmat
- Driver management screen and functionality – Wendy Bayise
- Order management screen and functionality – Zacharia Dipudi
- Navigation/route screen and functionality – Sabelo Ceza

---

## Sprint 9

### Sprint 9 – Day 1: Unit Testing

**User Story:**

As a software tester, I want to perform unit testing on individual application components so that defects can be identified early and each component functions correctly before integration.

**Due date:** August 24, 9:00 AM

**Tasks:**
- Conduct unit testing – Zacharia Dipudi
- Payment testing – Sabelo Ceza
- Test user authentication – Charmaine Dlamini
- Test database operations – Sabelo Ceza
- Record test results – Imaan Achmat
- Identify and fix bugs – Wendy Bayise and Imaan Achmat
- Test navigation between screens – Charmaine Dlamini
- User acceptance testing – Wendy Bayise
- Test across multiple devices – Zacharia Dipudi

---

### Sprint 9 – Day 2: System Testing

**User Story:**

As a tester, I want to test all the application features so that I can find and fix problems before the application is released.

**Due date:** August 26, 10:00 PM

**Tasks:**
- Prepare test environment – Zacharia Dipudi
- Create system and integration test cases – Imaan Achmat
- Test user authentication and authorisation – Charmaine Dlamini
- Test frontend and Supabase integration – Sabelo Ceza
- Log and fix defects – Wendy Bayise

---

### Sprint 9 – Day 3: Database Testing

**User Story:**

As a database administrator, I want to test the database so that data is stored, retrieved, and managed accurately, securely, and efficiently.

**Due date:** August 28, 11:00 PM

**Tasks:**
- Test real-time features – Zacharia Dipudi
- Test data validation – Wendy Bayise
- Verify security policies – Sabelo Ceza
- Test API endpoints – Imaan Achmat
- Document test results – Charmaine Dlamini

---

### Sprint 9 – Day 4: Debugging

**User Story:**

As a software developer, I want to debug the application so that errors are identified and resolved, ensuring the system functions correctly and efficiently.

**Due date:** September 1, 9:00 AM

**Tasks:**
- Identify bugs – Imaan Achmat
- Fix code issues – Sabelo Ceza
- Debug database errors – Charmaine Dlamini
- Debug API integration – Wendy Bayise
- Update bug log – Zacharia Dipudi

---

### Sprint 9 – Day 5: Final Testing

**Software Tester User Story:**

As a software tester, I want to perform final testing so that the application is fully functional, meets all requirements, and is ready for deployment.

**Customer User Story:**

As a customer, I want to use a fully tested application so that I can book, track, and manage my laundry orders without problems.

**Due date:** September 4, 11:00 PM

**Tasks:**
- Perform end-to-end testing – Charmaine Dlamini
- Verify all features – Zacharia Dipudi
- Verify database operations – Sabelo Ceza
- Test performance – Wendy Bayise
- Perform user acceptance testing (UAT) – Imaan Achmat
- Confirm deployment readiness – Sabelo Ceza
- Prepare final test report – Wendy Bayise

---

## Sprint 10

### Sprint 10 – Day 1: Project Documentation

**User Story:**

As a software developer, I want to prepare the system documentation so that the system's architecture, functionality, and technical implementation are clearly documented for maintenance and future development.

**Due date:** September 4, 9:00 AM

**Tasks:**
- Document system overview and project objectives – Wendy Bayise
- Document the system architecture – Sabelo Ceza
- Document the database structure and API endpoints – Zacharia Dipudi
- Combine the documents – Charmaine Dlamini
- Review and finalise all project documentation – Imaan Achmat

---

### Sprint 10 – Day 2: System Deployment

**Software Developer User Story:**

As a software developer, I want to deploy the system so that the application is available to users in a secure, stable, and production-ready environment.

**Customer User Story:**

As a customer, I want the application to be available online so that I can book and manage my laundry orders anytime and anywhere.

**Due date:** September 7, 9:00 AM

**Tasks:**
- Set up the production database – Wendy Bayise
- Configure security settings and environment variables – Imaan Achmat
- Configure the production/server environment – Zacharia Dipudi
- Deploy the application to the server – Sabelo Ceza
- Verify that the deployed system is working correctly – Charmaine Dlamini

---

### Sprint 10 – Day 3: Review and Improvement

**User Story:**

As a resident, I want to provide feedback on the application so that future improvements address my needs and enhance my experience.

**Due date:** September 16, 9:00 AM

**Tasks:**
- Gather feedback from users – Imaan Achmat
- Identify bugs and performance issues – Charmaine Dlamini
- Implement improvements and bug fixes – Zacharia Dipudi
- Update documentation based on the improvements – Sabelo Ceza

---

### **Reflection on User Stories and Tasks**

**Situation:**

During the development of LaundryPickupPro, our team created user stories and tasks across ten sprints. This helped us organise the project into smaller activities, from defining the business problem and conducting user research to designing the application, planning the database, testing, and deployment.

**Task:**

My responsibility was to contribute to the user stories and help organise and complete the tasks assigned to me. These activities included defining user requirements, analysing survey responses, preparing project documentation, prioritising tasks, designing application screens, testing user authentication, debugging database errors, and identifying areas for improvement.

**Action:**

I worked with my team members to break down the project into manageable tasks and assign responsibilities. We used the sprint structure and Trello board to track progress and understand what needed to be completed. I contributed to planning, requirements, screen design, testing, and documentation. I also communicated with team members and worked towards completing my assigned tasks within the deadlines.

**Result:**

Creating user stories and tasks helped our team understand the project requirements and work towards our goals in a more organised way. I learned the importance of breaking a large project into smaller tasks, setting priorities, managing time, and communicating with team members. I also gained a better understanding of how Agile practices support software development, from initial planning to testing and deployment. This experience helped me improve my teamwork, organisation, and problem-solving skills.

---

<div class="section-banner teal" id="product-backlog">
<h2>📋 Product Backlog</h2>
</div>

[View Product Backlog and Sprint Backlog on Trello](https://trello.com/b/D6tnqbrx)

<div class="gallery">
  <figure>
    <a href="images/Product-Backlog1.jpg"><img src="images/Product-Backlog1.jpg" alt="Product Backlog board - part 1" loading="lazy"></a>
    <figcaption>Product Backlog – Board 1</figcaption>
  </figure>
  <figure>
    <a href="images/Product-Backlog2.jpg"><img src="images/Product-Backlog2.jpg" alt="Product Backlog board - part 2" loading="lazy"></a>
    <figcaption>Product Backlog – Board 2</figcaption>
  </figure>
  <figure>
    <a href="images/Product-Backlog3.jpg"><img src="images/Product-Backlog3.jpg" alt="Product Backlog board - part 3" loading="lazy"></a>
    <figcaption>Product Backlog – Board 3</figcaption>
  </figure>
</div>

---

## Reflection on Product Backlog

**Situation:**

During the development of LaundryPickupPro, the product backlog was used to organise the features and requirements needed for the application. It helped the team keep track of the work required to build a laundry pickup and delivery platform.

**Task:**

My responsibility was to contribute to identifying and organising the features needed by users, ensuring that the application addressed their needs and that important requirements were considered during development.

**Action:**

I contributed to identifying the main features of the application and breaking the requirements into manageable items. These included user registration and login, customer and driver functionality, booking management, and other features needed for the pickup and delivery process. The product backlog helped the team prioritise work and understand which features needed attention during each sprint.

**Result:**

Working with the product backlog helped me understand the importance of planning and prioritising features before development. I learned that a well-organised backlog helps a team stay focused, manage requirements, and work towards delivering an application that meets users' needs.

---

<div class="section-banner amber" id="sprint-backlog">
<h2>🔄 Sprint Backlog</h2>
</div>

<div class="gallery">
  <figure>
    <a href="images/Sprint-Backlog1.png"><img src="images/Sprint-Backlog1.png" alt="Sprint Backlog board - part 1" loading="lazy"></a>
    <figcaption>Sprint Backlog – Board 1</figcaption>
  </figure>
  <figure>
    <a href="images/Sprint-Backlog2.png"><img src="images/Sprint-Backlog2.png" alt="Sprint Backlog board - part 2" loading="lazy"></a>
    <figcaption>Sprint Backlog – Board 2</figcaption>
  </figure>
  <figure>
    <a href="images/Sprint-Backlog3.png"><img src="images/Sprint-Backlog3.png" alt="Sprint Backlog board - part 3" loading="lazy"></a>
    <figcaption>Sprint Backlog – Board 3</figcaption>
  </figure>
</div>


---
## Reflection on Sprint Backlog

**Situation:**

During the development of LaundryPickupPro, the sprint backlog was used to organise the tasks selected for each sprint. It helped the team focus on the work that needed to be completed within a specific period.

**Task:**

My responsibility was to work on assigned tasks, manage my progress, and contribute to completing the planned work within each sprint.

**Action:**

I used the sprint tasks to guide my work on the application, including screen development, testing, debugging, documentation, and other development activities. Breaking the work into smaller tasks made it easier to understand what needed to be done and track progress. I also learned the importance of communicating with team members and managing my time while balancing project work with other academic responsibilities.

**Result:**

The sprint backlog helped me understand how large project requirements can be divided into smaller, achievable tasks. I improved my understanding of sprint planning, task tracking, prioritisation, and teamwork. I also learned that regular progress reviews help identify unfinished work and areas that need improvement before moving forward.

---

<div class="section-banner blue" id="agile-logbooks">
<h2>📚 Agile Logbooks</h2>
</div>

The Agile logbooks below document my progress, activities, and contributions to the development of LaundryPickupPro throughout the project.

### Logbook Documents

| Date | Logbook |
|---|---|
| 14 July – 17 July | [View Agile Logbook (PDF)](Logbooks/14July-17July-Agile-Logbook.pdf) |
| 21 July – 24 July | [View Agile Logbook (PDF)](Logbooks/21July-24July-Agile-Logbook.pdf) |
| 28 July – 31 July | [View Agile Logbook (PDF)](Logbooks/28July-31July-Logbook.pdf) |
| 04 August – 07 August | [View Agile Logbook (PDF)](Logbooks/04August-07August-Agile-Logbook.pdf) |
| 11 August – 14 August | [View Agile Logbook (PDF)](Logbooks/11August-14August-Agile-Logbook.pdf) |
| 15 September – 18 September | [View Agile Logbook (PDF)](Logbooks/15Sept-18Sept-Agile-Logbook.pdf) |
| 22 September – 25 September | [View Agile Logbook (PDF)](Logbooks/22Sept-25Sept-Agile-Logbook.pdf) |
| 28 September – 30 September | [View Agile Logbook (PDF)](Logbooks/28Sept-30Sept-Agile-Logbook.pdf) |

---

### Reflection on Agile Logbooks

**Situation:**  
During the development of LaundryPickupPro, I maintained Agile logbooks to record my activities, progress, and contributions throughout the project. The logbooks covered different stages of development, including screen design, frontend development, backend work, and deployment.

**Task:**  
My responsibility was to document the work completed during each period, keep track of my progress, and identify challenges that affected my ability to complete tasks.

**Action:**  
I recorded my development activities, documented completed tasks, and reflected on challenges such as managing my time while balancing project work with other academic responsibilities. I also used the logbooks to review my progress and identify tasks that needed further attention.

**Result:**  
Maintaining the logbooks helped me become more organised and aware of my progress. I improved my understanding of Agile practices, documentation, accountability, and continuous improvement. I also learned the importance of keeping accurate records to communicate progress and reflect on my contributions to a software development project.

---

<div class="section-banner" id="references">
<h2>📇 References</h2>
</div>

<div class="contact-grid">
  <div class="contact-card">
    <span class="label">CPUT Lecturer</span>
    <span class="value">Mrs Rebecca Bure</span>
    <p>📞 <a href="tel:0747054403">074 705 4403</a><br>✉️ <a href="mailto:burer@cput.ac.za">burer@cput.ac.za</a></p>
  </div>
  <div class="contact-card">
    <span class="label">Mentor · MzingweTec</span>
    <span class="value">Nhlanhla Nqoko</span>
    <p>📞 <a href="tel:0606181985">060 618 1985</a><br>✉️ <a href="mailto:nhlanhlanqoko1@gmail.com">nhlanhlanqoko1@gmail.com</a></p>
  </div>
</div>

<a href="#top" class="back-to-top" title="Back to top" aria-label="Back to top">↑</a>
