<p align="center">
  <a href="https://github.com/Sushil25742">
    <img
      src="https://i.ibb.co/Cp12TXmP/Chat-GPT-Image-Jul-1-2026-08-29-15-AM.png"
      alt="Sushil Kumar Sah’s profile banner"
      width="100%"
    />
  </a>
</p>

<h1 align="center">Hi 👋, I’m Sushil Kumar Sah</h1>

<p align="center">
  <strong>Computer Science Student &nbsp;·&nbsp; Aspiring AI Engineer &nbsp;·&nbsp; Nepal 🇳🇵</strong>
</p>

<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3200&pause=1400&color=28B8A0&center=true&vCenter=true&width=680&lines=What+can+a+model+learn+from+its+mistakes%3F;What+makes+an+AI+tool+useful+to+a+student%3F;Which+digital+skills+will+matter+in+Nepal%3F"
    alt="Questions I’m exploring about machine learning, useful AI tools, and digital skills in Nepal"
    width="85%"
  />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/sushil-sah-740a6b416/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge" alt="Connect on LinkedIn" /></a>
  <a href="https://www.kaggle.com/sushil1j"><img src="https://img.shields.io/badge/Kaggle-Explore-087EA4?style=for-the-badge&logo=kaggle&logoColor=white" alt="Visit my Kaggle profile" /></a>
  <a href="https://github.com/Sushil25742?tab=repositories"><img src="https://img.shields.io/badge/GitHub-View_Code-126B60?style=for-the-badge&logo=github&logoColor=white" alt="Browse my repositories" /></a>
</p>

<p align="center">
  <a href="#about-me">About me</a> &nbsp;·&nbsp;
  <a href="#ai-workbench">AI workbench</a> &nbsp;·&nbsp;
  <a href="#toolkit">Toolkit</a> &nbsp;·&nbsp;
  <a href="#experiments">Experiments</a> &nbsp;·&nbsp;
  <a href="#activity">Activity</a> &nbsp;·&nbsp;
  <a href="#connect">Connect</a>
</p>

---

<a name="about-me"></a>

## 👨‍💻 About me

I’m **Sushil**, a computer science student at **Xavier International College in Nepal**. I work with Python, JavaScript, and Java, and I’m learning how to take a machine learning idea from a notebook to an application someone can actually use.

I’m especially interested in the moment a model gets something wrong. Was the example unusual? Was the label unclear? Did I ask the wrong question in the first place? Those questions bring together the parts of computer science I enjoy most: writing code, investigating data, and figuring out what an answer actually means.

| 🎓 Studying | 🧠 Exploring | 🌏 Research interest |
| :--- | :--- | :--- |
| Computer science at Xavier International College | Deep learning, generative AI, and MLOps | Digital skills and employment opportunities for young people in Nepal |

<a name="ai-workbench"></a>

## 🔬 My AI workbench

**Suppose I wanted to build a tool that helps students find relevant internships.** Before choosing a model, I’d want to know what *relevant* means. A listing might match a student’s Python skills perfectly and still be a poor recommendation because the deadline has passed or the role requires experience they don’t have.

Here’s how I’d approach that experiment.

```mermaid
flowchart TD
    A["Ask students what makes a listing useful"] --> B["Label a small set of example listings"]
    B --> C["Try a simple keyword baseline"]
    C --> D{"Where does it go wrong?"}
    D -->|"Wrong skill match"| E["Inspect wording and labels"]
    D -->|"Expired or unsuitable role"| F["Check dates and eligibility"]
    E --> G["Compare revised results on held-out examples"]
    F --> G
    G --> H["Ask students to review the recommendations"]

    classDef research fill:#153F46,stroke:#5DD9BC,color:#FFFFFF
    classDef decision fill:#48351F,stroke:#F5B971,color:#FFFFFF
    classDef evaluation fill:#292F55,stroke:#A6AEFF,color:#FFFFFF
    class A,B,C research
    class D decision
    class E,F,G,H evaluation
```

The comparison I’d care about most is how often a student finds a listing worth applying to in the first five results. That gives me something concrete to improve and a reason to ask students what the ranking missed.

<a name="toolkit"></a>

## 🛠️ Technical toolkit

### Languages

<p>
  <img src="https://skillicons.dev/icons?i=python,js,java,c&theme=dark" alt="Python, JavaScript, Java, and C" />
</p>

**Python** for data and machine learning · **JavaScript** for the web · **Java and C** for core programming and algorithms

### Machine learning, web, and data

<p>
  <img src="https://skillicons.dev/icons?i=tensorflow,pytorch,html,css,nodejs,mysql,firebase&theme=dark" alt="TensorFlow, PyTorch, HTML, CSS, Node.js, MySQL, and Firebase" />
</p>

I’m exploring the connection between these tools: how a prediction produced in Python becomes something a person can see, use, and give feedback on in a web application.

<details>
<summary><strong>☁️ Open my cloud and developer toolbox</strong></summary>

<br />

<img src="https://skillicons.dev/icons?i=aws,azure,gcp,netlify,git,github,figma,vscode&theme=dark&perline=4" alt="AWS, Azure, Google Cloud, Netlify, Git, GitHub, Figma, and VS Code" />

| Area | Tools |
| :--- | :--- |
| Cloud platforms I’m exploring | AWS, Microsoft Azure, Google Cloud |
| Web hosting | Netlify |
| Version control | Git, GitHub |
| Interface design and development | Figma, VS Code |

</details>

<a name="experiments"></a>

## 🧪 Three experiments I’d like to build

Each idea starts with a small enough question to test. Open whichever one interests you.

<details>
<summary><strong>📊 01 · What skills appear in entry-level job listings in Nepal?</strong></summary>

### The question

If a student had one semester to learn a new technical skill, what evidence could help them choose?

### A first version

I’d start with a dated sample of public entry-level listings and record the role, location, and skills each employer mentions. I’d keep **required** and **preferred** skills separate. A student reading the results should be able to tell whether SQL is a requirement for a role or simply a bonus.

### What I’d show

A chart of the most frequently requested skills, a filter by role, and a link back to each original listing. I’d also show the sample size. Ten listings from Kathmandu and a hundred listings from across Nepal answer different questions.

</details>

<details>
<summary><strong>🤖 02 · Can a study assistant point to the paragraph behind its answer?</strong></summary>

### The question

Could a student use a course handout to check an AI-generated explanation for themselves?

### A first version

I’d use one handout, a small set of questions, and a simple interface. Each answer would appear beside the passage used to produce it. I’d include questions the handout cannot answer and check whether the assistant recognizes the missing information.

### What I’d measure

Can a reader find the supporting passage? Does it actually support the answer? How often does the assistant answer confidently when the handout is silent?

</details>

<details>
<summary><strong>☁️ 03 · What changes between a working notebook and a reliable demo?</strong></summary>

### The question

A prediction works on my laptop. What happens when someone submits a blank field, a new category, or an input format I didn’t anticipate?

### A first version

I’d package a small prediction model behind a web form and give it a set of deliberately awkward inputs. For each one, I’d record what the visitor saw and whether they could recover without help.

### What I’d learn

How to validate inputs, keep training and prediction steps consistent, and write an error message that tells someone what they can do next.

</details>

## 🇳🇵 A research question close to home

> **Which digital skills help young people in Nepal move from completing a course to finding an opportunity where they can use what they learned?**

I’d like to look at this question from three perspectives.

| Perspective | What I’d ask |
| :--- | :--- |
| 🎓 **Students** | Which skills have you had a chance to use outside an assignment? |
| 🏫 **Educators** | What kind of project helps you see whether a student can work independently? |
| 💼 **Employers** | What would you need to see in a beginner’s portfolio to invite them for an interview? |

I’d be particularly interested in where the answers differ. A student might be proudest of training a model, while an employer wants to hear how they noticed a data problem. That difference could make for a useful classroom project.

## 💡 A sixty-second ML puzzle

A dataset contains **100 internship listings**. Only **5** are relevant to a particular student. A model marks every listing as *irrelevant* and reports **95% accuracy**.

**Would you trust it to recommend an internship?**

<details>
<summary><strong>Reveal what the score hides ↓</strong></summary>

The model correctly rejected 95 irrelevant listings, so its accuracy really is **95%**. But it missed **all five** relevant listings. Its recall for relevant opportunities is **0 out of 5**.

For a recommendation tool, I’d also look at the first few results a student actually sees. A useful next question is: **Of the five listings we put at the top, how many would this student consider applying to?**

</details>

<a name="activity"></a>

## 📈 On GitHub

<p align="center">
  <a href="https://github.com/Sushil25742">
    <img
      src="https://github-readme-activity-graph.vercel.app/graph?username=Sushil25742&bg_color=0D1924&color=BDDCD8&line=38C6AA&point=F4B778&area=true&area_color=166F68&hide_border=true&custom_title=Contribution%20activity"
      alt="Sushil Kumar Sah’s recent GitHub contribution activity"
      width="100%"
    />
  </a>
</p>

<p align="center">
  <a href="https://github.com/Sushil25742?tab=repositories"><strong>Browse my repositories ↗</strong></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/Sushil25742?tab=stars">See what I’m bookmarking ↗</a>
</p>

## 📚 Learning shelf

A few places to start if you’re exploring similar topics.

| If you want to… | Start here |
| :--- | :--- |
| Practice Python and data analysis in short exercises | [Kaggle Learn](https://www.kaggle.com/learn) |
| Follow a neural network from tensors through training and saving | [PyTorch · Learn the Basics](https://docs.pytorch.org/tutorials/beginner/basics/intro.html) |
| Understand how data leakage can make a model look better than it is | [scikit-learn · Common Pitfalls](https://scikit-learn.org/stable/common_pitfalls.html) |
| Explore tokenizers, transformers, and language models | [Hugging Face · LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) |

<a name="connect"></a>

## 🌐 Let’s connect

If you’re a student in Nepal, **what’s one digital skill you wish you’d learned earlier, and where would you have used it?** I’d be interested in hearing your answer. I’d also love to exchange ideas about beginner-friendly ML projects, useful datasets, and ways to make research accessible to students.

<p align="center">
  <a href="https://www.linkedin.com/in/sushil-sah-740a6b416/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square" alt="LinkedIn" /></a>
  <a href="https://www.kaggle.com/sushil1j"><img src="https://img.shields.io/badge/Kaggle-087EA4?style=flat-square&logo=kaggle&logoColor=white" alt="Kaggle" /></a>
  <a href="https://www.instagram.com/sushil1t/"><img src="https://img.shields.io/badge/Instagram-B03272?style=flat-square&logo=instagram&logoColor=white" alt="Instagram" /></a>
  <a href="https://x.com/sushilsah288149"><img src="https://img.shields.io/badge/X-202124?style=flat-square&logo=x&logoColor=white" alt="X" /></a>
  <a href="https://www.facebook.com/sushil1rs"><img src="https://img.shields.io/badge/Facebook-1877F2?style=flat-square&logo=facebook&logoColor=white" alt="Facebook" /></a>
  <a href="https://www.tiktok.com/@sushil1r"><img src="https://img.shields.io/badge/TikTok-202124?style=flat-square&logo=tiktok&logoColor=white" alt="TikTok" /></a>
</p>
