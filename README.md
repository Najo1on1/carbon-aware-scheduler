# Carbon-Aware Cloud Scheduler ♻️

## Overview  
Training AI models requires significant energy. Depending on the time of day, that energy may come from renewable sources or fossil fuels.  
This project implements an autonomous agent that monitors the UK National Grid (2018–2023) and dynamically defers non‑urgent AI workloads to “greener” time windows.

**Key Result:**  
In simulations, this agent achieves a **~15–18% reduction in carbon emissions** for standard AI workloads.

---

## 🚀 How to Navigate This Repo

### **1. The Solution (`/src`)**  
Go here for the clean, working implementation.

- **Notebook:** `Carbon-Aware_Cloud_Scheduler_2.ipynb`  
- **Features:** Contains the `WatcherAgent` (Sensor) and `SchedulerAgent` (Logic).  
- **Demo:** Includes an interactive function, `run_custom_scenario()`, allowing you to test the agent against any date range in the dataset.

---

### **2. The Journey (`/research`)**  
Go here to see how the system was built.

- **Notebook:** `Carbon-Aware_Cloud_Scheduler_1.ipynb`  
- **Contents:** Full Data Engineering (ETL), handling of missing values/duplicates, and the fidelity tests used to verify agent logic.

---

## 📦 Usage

1. Install requirements:

```bash
pip install -r requirements.txt
```

2. Navigate to:

```bash
cd src
```

3. Run the final cell to execute a full simulation:

```python
run_custom_scenario("2022-01-10", "2022-01-17")
```

---

## 🧠 Acknowledgments  
Built for the **Google & Kaggle AI Agents Intensive**.

---

## 📁 Repository Structure  

```
carbon-aware-scheduler/
│
├── README.md
├── LICENSE
├── requirements.txt
│
├── research/
│   ├── Carbon-Aware_Cloud_Scheduler_1.ipynb
│   └── artifacts/
│       ├── data_profile_raw.html
│       └── final_capstone_plot.png
│
└── src/
    ├── Carbon-Aware_Cloud_Scheduler_2.ipynb
    └── data/
        └── .gitkeep
```
