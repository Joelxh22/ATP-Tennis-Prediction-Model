# 🎾 ATP Tennis Match Outcome Predictor (2024)

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![PowerBI](https://img.shields.io/badge/Visuals-PowerBI-yellow)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Accuracy](https://img.shields.io/badge/Accuracy-74.33%25-brightgreen)

## 📌 Project Overview
This project applies Machine Learning to predict the winners of ATP Tennis matches for the 2024 season. By engineering custom features such as **Surface-Specific Win Percentages** and **Player Height Differences**, the Random Forest model achieved a **74.33% accuracy rate** on unseen test data.

The project includes a full end-to-end pipeline: Data Cleaning, Feature Engineering, Model Training, and an interactive Power BI Dashboard for auditing results.

---

## 📊 Key Results
| Metric | Result |
| :--- | :--- |
| **Model Used** | Random Forest Classifier |
| **Test Accuracy** | **74.33%** |
| **Key Predictor** | Rank Difference |
| **Secondary Predictor** | Surface Win % Differential |

---

## 🧠 Feature Engineering (The "Secret Sauce")
Instead of relying solely on player rankings, this project engineered deep domain-specific features to improve prediction logic:

1.  **Surface Specialization:** Calculated individual win percentages for Hard, Clay, and Grass courts to capture "specialist" advantages.
2.  **Physical Attributes:** Engineered a `Height Difference` feature, recognizing the advantage of serve dominance in modern tennis.
3.  **Comparative Stats:** Created differential features (e.g., `Rank Diff`, `Age Diff`) to represent the *gap* between Player 1 and Player 2, rather than just raw values.

---

## 📈 Power BI Dashboard
An interactive dashboard was built to visualize the model's confidence and audit specific matches.

### 1. Main Dashboard View
*Shows the overall accuracy and the breakdown of correct vs. incorrect predictions.*
![Dashboard Overview](images/PowerBI_Tennis_Model_Screenshot.PNG)

---

## 🛠️ Installation & Usage

### Prerequisites
* Python 3.x
* Jupyter Notebook
* Power BI Desktop (for visualization)

### Steps
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/ATP-Tennis-Prediction-Model.git](https://github.com/yourusername/ATP-Tennis-Prediction-Model.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the analysis:**
    Open `Tennis ATP 2024 Match Predictions.ipynb` in Jupyter and run all cells.
4.  **View the Dashboard:**
    Open `ATP Predictive Analysis 2024.pbix` in Power BI Desktop.

---

## 📂 Project Structure
* `Tennis ATP 2024 Match Predictions.ipynb`: The main Python code for data processing and modeling.
* `atp_matches_2024.csv`: Raw input data containing match statistics.
* `tennis_final_predictions_v4.csv`: The processed output file fed into Power BI.
* `ATP Predictive Analysis 2024.pbix`: The Power BI visualization file.

---

## 🤝 Contributing
Feedback and suggestions are welcome! Feel free to open an issue or submit a pull request if you have ideas on how to improve the model (e.g., adding player fatigue or head-to-head history).

## 📜 License
This project is open-source.
