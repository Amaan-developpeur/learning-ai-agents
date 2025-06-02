# Learning AI Agents

This repository documents my journey in learning and building AI Agents from scratch. The goal is to not just train machine learning models, but to structure them into autonomous agents that can perceive their environment, make decisions, and act in a goal-oriented way — all inspired by the foundational principles from the book *Artificial Intelligence: A Modern Approach (AIMA)*.

---

## What is an AI Agent?
An AI Agent is a system that:
- **Perceives** its environment via sensors (e.g., an image classifier for fundus scans)
- **Decides** what action to take (e.g., refer the patient, monitor, or do nothing)
- **Acts** using effectors or actuators (in our case, logging the decision, referring cases)
- Optionally receives **feedback** from the environment to improve over time

This repo takes the idea beyond just CNNs — into actual systems thinking: building complete agent loops.

---

## Project Objective
To build a decision-making AI agent that:
- Wraps a trained CNN model (for glaucoma or fundus disease detection)
- Implements a `perceive-decide-act` loop
- Simulates basic environment responses (reward, penalty, feedback)
- Evolves from a rule-based agent to more goal- or utility-based designs

---

## Learning Milestones
| Phase | Topic | Status |
|-------|-------|--------|
| 1 | Understand AI agents from AIMA Ch. 2, 3, 4, 18 | ✅ In Progress |
| 2 | Build initial agent loop with CNN as sensor | ⏳ |
| 3 | Add decision logic + simple environment | ⏳ |
| 4 | Evaluate agent behavior vs. raw model | ⏳ |
| 5 | Extend agent intelligence (rewards, rules, memory) | ⏳ |

---

## Repository Structure
```
learning-ai-agents/
│
├── README.md              # This document
├── requirements.txt       # Python dependencies
│__ notes.docx
├── models/
│   └── glaucoma_cnn.pt    # Pretrained or custom model
│
├── agent/
│   ├── agent_loop.py      # Agent's main control logic
│   ├── environment.py     # Simulated feedback or rule-based reward system
│   └── utils.py           # Helper functions for thresholds, logging
│
├── notebooks/
│   └── agent_demo.ipynb   # Notebook demo of agent on fundus images
│
└── data/
    └── demo_images/       # Sample images for agent testing
```

---

## Dependencies
- Python ≥ 3.8
- tensorflow
- keras
- NumPy, OpenCV, Matplotlib
- tqdm, pandas (for logs and analysis)

Install via:
```bash
pip install -r requirements.txt
```

---

## Future Work
- [ ] Add reward feedback from environment
- [ ] Use confidence calibration for utility-based decisions
- [ ] Explore learning-based policies (Q-learning, planning)
- [ ] Shift toward goal-directed and learning agents

---

## References
- Russell & Norvig, "Artificial Intelligence: A Modern Approach"
- AIMA Python Code: [https://github.com/aimacode/aima-python](https://github.com/aimacode/aima-python)
- Retinal Fundus Data: Kaggle datasets

---



---

