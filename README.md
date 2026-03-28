<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=4000&pause=1000&color=58A6FF&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=100&lines=Ishan+Madhani;Backend+Engineer+%C2%B7+ML+Systems+%C2%B7+Distributed+Infra" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://linkedin.com/in/ishan-madhani"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:ishan.madhani@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/ishan0410"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <img src="https://komarev.com/ghpvc/?username=ishan0410&style=for-the-badge&color=58A6FF&label=PROFILE+VIEWS" />
</p>

---

<img align="right" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ishan0410&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&langs_count=6" width="320" />

### About Me

MS Computer Science @ **USC** (2026). I build backend systems and ML pipelines that run in production — LLM extraction pipelines processing thousands of financial documents, churn prediction models serving **1.2M+ users** on AWS, and retrieval systems backed by vector search.

Currently focused on **backend infrastructure**, **API design**, and **applied ML systems**.

<br clear="right"/>

---

### Tech Stack

<p align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**ML / AI**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)

**Cloud & Infrastructure**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white)

</p>

---

### Production Experience

<table>
<tr>
<td width="50%">

#### <img src="https://img.shields.io/badge/Fiscali-000000?style=flat-square" /> AI/ML Intern

<br>

Designed a **multi-stage LLM pipeline** (GPT-4 + JSON schema extraction) that converts unstructured financial agreements into normalized, queryable datasets.

| Metric | Impact |
|--------|--------|
| Processing Speed | **3x faster** |
| Manual Effort | **↓ 80%** |
| Terms Clustered | **11,000+** |

`GPT-4` `Prompt Chaining` `TF-IDF` `K-Means` `JSON Schema`

</td>
<td width="50%">

#### <img src="https://img.shields.io/badge/RazorThink-000000?style=flat-square" /> Software Developer Intern

<br>

Built and deployed a **churn prediction system** on AWS infrastructure with optimized inference latency across the serving stack.

| Metric | Impact |
|--------|--------|
| Users Served | **1.2M+** |
| Model AUC | **0.91** |
| System Uptime | **98.6%** |

`SageMaker` `Lambda` `EC2` `Scikit-learn` `AWS`

</td>
</tr>
</table>

---

### Featured Projects

<a href="https://github.com/ishan0410/document-intelligence-pipeline">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=ishan0410&repo=document-intelligence-pipeline&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9" />
</a>
<a href="https://github.com/ishan0410/Transfer-Learning-for-Waste-Image-Classification">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=ishan0410&repo=waste-image-classifier&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9" />
</a>

<br><br>

<details>
<summary><b>📂 document-intelligence-pipeline</b> — End-to-end RAG system</summary>
<br>

```
PDF Upload → Text Extraction → Chunking → Embedding ─┬─ FAISS (dense)
                                                      └─ TF-IDF (sparse)
                                                             │
                                                      Hybrid Retrieval
                                                             │
                                                      LLM Generation → Structured Output
```

**What it does:** Ingests raw PDFs, builds a semantic retrieval index using dual embedding (dense + sparse), and generates structured assessments via LLM generation with output parsing.

**Why hybrid retrieval:** Dense embeddings alone miss keyword-exact matches. Sparse alone misses semantic similarity. Combining both gives significantly better retrieval precision.

**Stack:** `Python` `LangChain` `FAISS` `TF-IDF` `Gradio` `OpenAI API`

**Design:** Each pipeline stage (chunker, embedder, retriever, generator) is independently testable and swappable.

</details>

<details>
<summary><b>📂 waste-image-classifier</b> — CNN architecture benchmark</summary>
<br>

Systematic transfer learning benchmark across 5 CNN architectures for multi-class waste sorting under identical training protocols.

| Architecture | F1 Score | AUC | Status |
|-------------|----------|-----|--------|
| **ResNet101** | **0.768** | **0.971** | **✅ Best** |
| VGG16 | — | — | Tested |
| EfficientNet-B0 | — | — | Tested |
| DenseNet121 | — | — | Tested |
| MobileNetV2 | — | — | Tested |

**Key insight:** Deeper architectures (ResNet101) significantly outperformed lightweight models on this dataset due to fine-grained texture differences between waste categories.

**Stack:** `TensorFlow` `OpenCV` `Scikit-learn` `Matplotlib`

</details>

---

### GitHub Analytics

<p align="center">
  <img width="49%" src="https://github-readme-stats.vercel.app/api?username=ishan0410&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9&count_private=true" />
  <img width="49%" src="https://streak-stats.demolab.com/?user=ishan0410&theme=github-dark-blue&hide_border=true&background=0d1117&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff" />
</p>

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=58a6ff&height=80&section=footer" width="100%" />
</p>
