# AI Lab Project Repository

## Overview

This repository contains a collection of artificial intelligence and machine learning projects developed for the AI Lab. Each project demonstrates different AI techniques and approaches to solving complex computational problems.

---

## Projects

### 1. Puzzle Solver

#### Description
An intelligent puzzle-solving system designed to solve the 8-puzzle problem using advanced search algorithms. This project implements the A* (A-Star) pathfinding algorithm to find optimal solutions efficiently.

#### Objectives
- Implement heuristic-based search algorithms for puzzle solving
- Demonstrate the efficiency of A* algorithm over traditional search methods
- Provide an optimal path from initial state to goal state

#### Key Features
- **A* Algorithm Implementation**: Combines cost and heuristic evaluation for optimal pathfinding
- **Heuristic Functions**: Employs Manhattan distance and other heuristics for intelligent state exploration
- **Optimized State Space Search**: Efficiently navigates through possible puzzle configurations

#### Technology Stack
- Python 3.x
- Jupyter Notebook for interactive exploration and visualization
- Data structures: Priority queues, graphs

#### Files
- `8_puzzle_astar.ipynb`: Main implementation notebook with algorithm explanation and demonstrations

---

### 2. Customer Churn Prediction

#### Description
A machine learning project focused on predicting customer churn in the telecommunications industry. This project utilizes classification algorithms to identify customers at risk of discontinuing service.

#### Objectives
- Develop predictive models to identify customers likely to churn
- Analyze key features influencing customer retention
- Provide actionable insights for customer retention strategies

#### Key Features
- **Data Analysis**: Comprehensive exploratory data analysis of customer behavior patterns
- **Predictive Modeling**: Implementation of machine learning classifiers
- **Feature Engineering**: Identification and optimization of relevant features
- **Performance Metrics**: Evaluation using standard classification metrics (accuracy, precision, recall, F1-score)

#### Technology Stack
- Python 3.x
- Jupyter Notebook for data analysis and model development
- Machine Learning Libraries: scikit-learn, pandas, numpy
- Data Visualization: matplotlib, seaborn

#### Dataset
- **Source**: Telecom customer churn dataset
- **File**: `data/telecom_churn.csv`
- **Content**: Customer demographics, service usage, and churn status

#### Files
- `customer-churn-pred.ipynb`: Comprehensive analysis and model implementation notebook
- `data/telecom_churn.csv`: Raw dataset
- `requirements.txt`: Python dependencies

---

## Installation & Setup

### Prerequisites
- Python 3.7 or higher
- Jupyter Notebook

### Getting Started

1. Clone the repository
2. Navigate to the project directory
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open the respective `.ipynb` files to explore and run the projects

---

## Project Structure

```
AI-Lab-Project/
├── README.md
├── Puzzle-Solver/
│   ├── 8_puzzle_astar.ipynb
│   └── README.md
├── Customer-Churn-Prediction/
│   ├── customer-churn-pred.ipynb
│   ├── requirements.txt
│   ├── README.md
│   └── data/
│       └── telecom_churn.csv
```

---

## License & Acknowledgments

These projects are part of the AI Lab curriculum and serve as educational demonstrations of AI and machine learning concepts.
