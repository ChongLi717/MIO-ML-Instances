# MPT-Instances

**Two Groups of Instances for Accelerating Real-Time Train Timetable Rescheduling via Machine Learning**

This repository provides instance datasets designed for training and evaluating machine learning models for **real-time train timetable rescheduling**. The dataset supports research on data-driven parameter tuning and optimization methods for disruption management in railway operations.

---

## Repository Structure

```
MPT-Instances/
│
├── Param_Default.csv        # Default solver parameter settings
├── Param_Range.csv          # Feasible ranges of solver parameters
├── TrainingInstances.csv    # Training dataset
├── TestInstances.csv        # Test/validation dataset
└── README.md                # Repository documentation
```

---

## Dataset Description

The repository organizes instances into two primary datasets for supervised learning and performance evaluation.

### 1. TrainingInstances.csv

This dataset is used for model training. Each row corresponds to a disruption scenario instance and contains:

* Instance feature vectors describing timetable and disruption characteristics
* Associated solver parameter configurations
* Performance-related labels or targets

The exact column definitions can be found in the CSV header. These data support regression, classification, or hybrid learning approaches.

---

### 2. TestInstances.csv

This dataset is reserved for evaluation and benchmarking. It follows the same format as the training dataset and is used to assess generalization performance on unseen disruption scenarios.

---

### 3. Parameter Configuration Files

* **Param_Default.csv** — Contains default solver parameter values, useful for baseline comparisons and initialization.
* **Param_Range.csv** — Specifies feasible parameter ranges, which can be used for:

  * Parameter search and hyperparameter tuning
  * Feature normalization
  * Defining configuration constraints

---
