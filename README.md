<h1>Sushil Kumar Sah <img src="https://flagcdn.com/w40/np.png" width="22" alt="Nepal" /></h1>

**Computer science student at Xavier International College · Aspiring AI engineer**

[Browse my work](https://github.com/Sushil25742?tab=repositories) &nbsp; / &nbsp; [Kaggle](https://www.kaggle.com/sushil1j) &nbsp; / &nbsp; [LinkedIn](https://www.linkedin.com/in/sushil-sah-740a6b416/)

<img
  src="https://thumb.wikimedia.org/wikipedia/commons/thumb/8/8f/PanoAnnapurana.JPG/1280px-PanoAnnapurana.JPG"
  width="100%"
  alt="A panoramic view across the Himalayas from Poon Hill in Nepal, with Dhaulagiri to the left and Annapurna to the right."
/>
<sub>Poon Hill, Nepal &nbsp;·&nbsp; Dhaulagiri and Annapurna &nbsp;·&nbsp; <a href="https://commons.wikimedia.org/wiki/File:PanoAnnapurana.JPG">James Heilman</a> / <a href="https://creativecommons.org/licenses/by-sa/3.0/">CC BY-SA 3.0</a></sub>

<br />

## Namaste 👋

I’m **Sushil**, a computer science student in Nepal. I write Python, JavaScript, and Java, and I’m learning how to build AI applications that hold up when someone tries them with their own words, data, or questions.

One question behind my interest in AI is simple: **what happens when a tool built around English meets a student who asks the same question in Nepali?** Here’s a small example you can try right on this page.

<p>
  <a href="#experiment"><img src="https://img.shields.io/badge/Try_the_experiment-115E59?style=for-the-badge" alt="Try the experiment" /></a>
  <a href="#toolkit"><img src="https://img.shields.io/badge/Explore_my_toolkit-3730A3?style=for-the-badge" alt="Explore my toolkit" /></a>
  <a href="#research"><img src="https://img.shields.io/badge/Read_my_research_notes-9A3412?style=for-the-badge" alt="Read my research notes" /></a>
</p>

---

<a name="experiment"></a>

## 🔎 One question, two languages

Imagine a student portal with these three documents:

| ID | Document |
| :---: | :--- |
| **A** | The **scholarship deadline** is Friday. |
| **B** | The library opens at nine. |
| **C** | The robotics club meets on Monday. |

Now search for **“scholarship deadline”**. Document A is an easy match. What happens if you search for **“छात्रवृत्तिको म्याद”** instead?

<details>
<summary><strong>Reveal what a keyword search sees</strong></summary>

<br />

| Search | Matching words in document A | Result |
| :--- | :---: | :--- |
| `scholarship deadline` | 2 | Document A |
| `छात्रवृत्तिको म्याद` | 0 | No match |

Both queries ask about the scholarship deadline. A search based on exact word overlap can answer one and miss the other entirely.

**What I’d test next:** Compare a small bilingual glossary with multilingual embeddings. For a narrow student portal, the glossary might work surprisingly well. I’d test spelling variations, mixed Nepali–English questions, and questions the documents cannot answer before choosing an approach.

</details>

<details>
<summary><strong>Run the baseline in Python · standard library only</strong></summary>

```python
from string import punctuation

documents = {
    "A": "The scholarship deadline is Friday.",
    "B": "The library opens at nine.",
    "C": "The robotics club meets on Monday.",
}


def words(text):
    return {word.strip(punctuation).casefold() for word in text.split()}


def search(query):
    query_words = words(query)
    scores = {
        doc_id: len(query_words & words(document))
        for doc_id, document in documents.items()
    }
    best_score = max(scores.values(), default=0)
    return [doc_id for doc_id, score in scores.items() if score == best_score > 0]


print(search("scholarship deadline"))  # ['A']
print(search("छात्रवृत्तिको म्याद"))       # []
```

Try searching for `Monday`, `scholarships`, or `पुस्तकालय`. Which misses could you fix by normalizing words, and which would need knowledge of another language?

</details>

<a name="toolkit"></a>

## 🧰 Tools I work with

### Code & data

<img src="https://skillicons.dev/icons?i=python,java,js,c,mysql&theme=dark" alt="Python, Java, JavaScript, C, and MySQL" />

Python is my starting point for data experiments. I also work with JavaScript, Java, C, and SQL, and I’m studying the data structures and algorithms underneath them.

### Models & interfaces

<img src="https://skillicons.dev/icons?i=pytorch,tensorflow,html,css,nodejs,firebase,figma&theme=dark" alt="PyTorch, TensorFlow, HTML, CSS, Node.js, Firebase, and Figma" />

I’m exploring both sides of an AI application: the model that produces a result and the interface where a person reads it. I’m especially interested in how to show a source, explain a low-confidence answer, or help someone recover from an unexpected input.

<details>
<summary><strong>☁️ Cloud, deployment, and development tools</strong></summary>

<br />

<img src="https://skillicons.dev/icons?i=aws,azure,gcp,netlify,git,github,vscode&theme=dark" alt="AWS, Azure, Google Cloud, Netlify, Git, GitHub, and VS Code" />

I’m learning how to package a model, deploy it behind a web interface, and reproduce a result after the code or data changes. My next milestone is a small deployment where I can trace a prediction back to the model version that produced it.

</details>

<a name="research"></a>

## 📓 Research notebook

### What does an entry-level job listing actually ask a student to do?

Two listings can both mention **Python**. One might ask a student to clean a spreadsheet. Another might expect them to build an API. Counting the keyword treats both jobs as the same opportunity, even though preparing for them takes different work.

For a small study of digital skills and youth employment in Nepal, I’d start by recording the **task behind each skill**.

| Example phrase | Skill | Task | What I’d preserve |
| :--- | :--- | :--- | :--- |
| “Prepare weekly reports using SQL” | SQL | Reporting | The sentence describing the work |
| “Python experience preferred” | Python | Unspecified | The word *preferred* |
| “Deploy a web application” | Web development | Deployment | The task, even when no tool is named |

These are illustrative examples. For the study itself, I’d keep the source, posting date, and location alongside each entry so a reader could inspect the evidence.

<details>
<summary><strong>Open the first three questions I’d ask students</strong></summary>

1. Think of the last internship you considered. Which requirement was hardest to interpret?
2. Which project from college would you show to demonstrate that skill?
3. What would you change about that project if you knew someone would spend only two minutes reviewing it?

The answer I’d most like to hear is a specific story: a listing someone almost skipped, a project that helped them apply, or a requirement they understood only after speaking with the employer.

</details>

## 🌱 What I’m learning now

| Focus | A milestone I can test |
| :--- | :--- |
| 🟣 **Deep learning** | Trace one example through a training loop and explain why the model’s parameters change. |
| 🔵 **Generative AI** | Build a handout assistant that shows the passage behind an answer and recognizes when the handout is silent. |
| 🟢 **MLOps** | Run the same input through a notebook and a deployed service and investigate any difference. |
| 🟠 **Research methods** | Turn a broad question about digital skills into a small study another student could repeat. |

## 📊 GitHub activity

<a href="https://github.com/Sushil25742?tab=repositories">
  <img
    width="100%"
    src="https://github-readme-activity-graph.vercel.app/graph?username=Sushil25742&bg_color=102825&color=EAF5E8&line=76D6AD&point=FFC989&area=true&area_color=28665D&hide_border=true&custom_title=Recent%20contributions"
    alt="Recent GitHub contributions by Sushil Kumar Sah"
  />
</a>

**Explore my GitHub** &nbsp; [Repositories ↗](https://github.com/Sushil25742?tab=repositories) &nbsp;·&nbsp; [Projects I’ve starred ↗](https://github.com/Sushil25742?tab=stars)

## 📚 Resources worth opening

- **For a first training loop:** [PyTorch — Learn the Basics](https://docs.pytorch.org/tutorials/beginner/basics/intro.html)
- **For an evaluation score that looks too good:** [scikit-learn — Common Pitfalls](https://scikit-learn.org/stable/common_pitfalls.html)
- **For tokenizers and language models:** [Hugging Face — LLM Course](https://huggingface.co/learn/llm-course/chapter1/1)
- **For short, hands-on data exercises:** [Kaggle Learn](https://www.kaggle.com/learn)

---

## 💬 Connect

I’d love to hear from people working on **Nepali-language tools, student projects, or applied machine learning**. If you know a public Nepali dataset that a student could use for a first search experiment, send it my way.

[**LinkedIn**](https://www.linkedin.com/in/sushil-sah-740a6b416/) &nbsp;·&nbsp; [**Kaggle**](https://www.kaggle.com/sushil1j) &nbsp;·&nbsp; [Instagram](https://www.instagram.com/sushil1t/) &nbsp;·&nbsp; [X](https://x.com/sushilsah288149) &nbsp;·&nbsp; [Facebook](https://www.facebook.com/sushil1rs) &nbsp;·&nbsp; [TikTok](https://www.tiktok.com/@sushil1r)
