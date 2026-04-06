<div align="center">

<!-- Animated Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=Ahmad%20Saleh&fontSize=70&fontColor=fff&animation=twinkling&fontAlignY=38&desc=Data%20Scientist%20%7C%20ML%20Engineer%20%7C%20Backend%20Developer&descAlignY=58&descAlign=50" width="100%"/>

<!-- Typing Animation -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&height=55&lines=Data+Scientist+%F0%9F%93%8A;Machine+Learning+Engineer+%F0%9F%A4%96;Deep+Learning+Practitioner+%F0%9F%A7%A0;FastAPI+Backend+Developer+%E2%9A%A1;Turning+Data+into+Decisions+%F0%9F%9A%80" alt="Typing SVG" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ahmad%20Saleh-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ahmad-saleh0309/)
[![Email](https://img.shields.io/badge/Email-ahmadsaleh0309%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ahmadsaleh0309@gmail.com)
[![Profile Views](https://komarev.com/ghpvc/?username=AhmadHakeem03&style=for-the-badge&color=58A6FF&label=PROFILE+VIEWS)](https://github.com/AhmadHakeem03)

</div>

---

## 👨‍💻 About Me

```python
class DataScientist:
    def __init__(self):
        self.name        = "Ahmad Saleh"
        self.role        = "Data Scientist & ML Engineer"
        self.location    = "Jordan 🇯🇴"
        self.languages   = ["Python", "C++", "JavaScript"]
        self.focus       = ["Machine Learning", "Deep Learning", "Data Science"]
        self.backend     = ["FastAPI", "REST APIs", "LLM Integration"]
        self.tools       = ["Scikit-Learn", "TensorFlow", "PyTorch",
                            "Matplotlib", "Seaborn", "Pandas", "NumPy"]

    def current_goal(self):
        return "Building intelligent systems that solve real-world problems 🚀"

me = DataScientist()
print(me.current_goal())
```

---

## 🏆 Top Tech Skills

<div align="center">

### 💻 Programming Languages
<p>
  <img src="https://skillicons.dev/icons?i=python,cpp,js&theme=dark" />
</p>

### 🤖 Machine Learning & Deep Learning
<p>
  <img src="https://skillicons.dev/icons?i=tensorflow,pytorch&theme=dark" />
</p>
<p>
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/XGBoost-003366?style=for-the-badge&logo=data:image/png;base64,&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
</p>

### 📊 Data Science & Visualization
<p>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white"/>
</p>

### 🌐 Backend & Web
<p>
  <img src="https://skillicons.dev/icons?i=fastapi,html,css,js&theme=dark" />
</p>

### 🛠️ Tools & Environment
<p>
  <img src="https://skillicons.dev/icons?i=git,linux,vscode&theme=dark" />
</p>

</div>

---

## 📂 Featured Projects

<div align="center">

| 🚀 Project | 📝 Description | 🛠️ Tech Stack |
|:-----------|:---------------|:--------------|
| 🔬 **Medical Report Analyzer** | AI system that extracts & explains lab reports using OCR + LLMs | Python, FastAPI, OCR, LLMs |
| 📊 **Data Quality Checker** | Detects anomalies and ensures dataset consistency automatically | Python, Pandas, Scikit-Learn |
| 🤖 **AI APIs with FastAPI** | Intelligent backend services powered by large language models | FastAPI, Python, LLMs |

</div>

---

## 📊 Visualization Samples

> *Examples of data visualization work using Matplotlib & Seaborn*

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np

# ── Skill proficiency radar-style bar chart ──────────────────────────────────
skills = {
    "Machine Learning": 90,
    "Deep Learning":    85,
    "Data Analysis":    92,
    "FastAPI / Backend":80,
    "Data Visualization":88,
    "NLP / LLMs":       83,
}

sns.set_theme(style="darkgrid", palette="mako")
fig, axes = plt.subplots(1, 2, figsize=(14, 5))

# Horizontal bar chart
bars = axes[0].barh(list(skills.keys()), list(skills.values()),
                    color=sns.color_palette("mako", len(skills)))
axes[0].set_xlim(0, 100)
axes[0].set_title("Skill Proficiency (%)", fontsize=14, fontweight="bold")
axes[0].bar_label(bars, fmt="%.0f%%", padding=4)

# Correlation heatmap (sample data)
data = pd.DataFrame(np.random.rand(6, 6),
                    columns=list(skills.keys()),
                    index=list(skills.keys()))
sns.heatmap(data, ax=axes[1], cmap="mako", annot=True,
            fmt=".2f", linewidths=0.5, square=True)
axes[1].set_title("Feature Correlation Heatmap", fontsize=14, fontweight="bold")

plt.tight_layout()
plt.savefig("visualization_sample.png", dpi=150, bbox_inches="tight")
plt.show()
```

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3&section=header" width="100%"/>

---

## 🔥 Top Languages

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AhmadHakeem03&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
</div>

---

## ⚡ Fun Fact

<div align="center">

> *"Without data, you're just another person with an opinion."* — W. Edwards Deming

💡 I turn raw, messy data into clear, actionable insights that drive smarter decisions — one model at a time. 🚀

</div>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer" width="100%"/>
</div>
