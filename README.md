# 💫 About Project:
THIS PROJECT IS MADE FOR PEOPLES WHO ARE WILLING TO MAKE PROGRESS IN THEIR <br>PERSONALITY-DYNAMICS<br>


# 🏗️ Architecture:

```mermaid
flowchart TD
    User["User"] -->|uses| Presentation["Presentation Layer - Tkinter Interface (quiz.py)"]
    Presentation -->|dispatches| Orchestration["App Orchestration - AttentionApp Controller (quiz.py)"]

    subgraph ContentStores["Content Stores"]
        TipsData[("Tips Data (tips.json)")]
        QuizQuestions[("Quiz Questions (quiz_questions.json)")]
        PDAQuestions[("PDA Questions (PDA.json)")]
    end

    subgraph AssessmentStages["Assessment Stages"]
        TipsBrowser["Tips Browser (quiz.py)"]
        GeneralQuiz["General Quiz (quiz.py)"]
        PDAEvaluation["PDA Evaluation (quiz.py)"]
        EvalResults["Evaluation Results (quiz.py)"]

        GeneralQuiz -->|produces| EvalResults
        PDAEvaluation -->|produces| EvalResults
    end

    Orchestration -->|reads| TipsData
    Orchestration -->|reads| QuizQuestions
    Orchestration -->|reads| PDAQuestions

    Orchestration -->|opens| TipsBrowser
    Orchestration -->|starts| GeneralQuiz
    Orchestration -->|starts| PDAEvaluation
```


# 💻 Tech Stack:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

---
[![](https://visitcount.itsvg.in/api?id=rakesh8345&icon=0&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
