# Employee Sentiment Analysis – README

## Project Overview
This project analyzes internal employee email data to understand sentiment trends, identify at-risk employees, and build predictive models using NLP and statistical techniques. The data has been labeled using transformer-based sentiment models, followed by detailed EDA, employee-level analysis, and machine learning modeling.

---

## Summary of Key Results

### Top 3 Positive Employees (Based on Monthly Sentiment Scores)
| Rank | Employee         | Behavior Summary                             |
|------|------------------|-----------------------------------------------|
| 1    | **Johnny Palmer** | Consistently high positivity in all months    |
| 2    | **Tori Kuykendall** | Regular positive sentiment                   |
| 3    | **Kara Moriarty**  | Strong positive spikes in certain months     |

### Top 3 Negative Employees
| Rank | Employee         | Behavior Summary                             |
|------|------------------|-----------------------------------------------|
| 1    | **Kayne Coulter** | Multiple months of net negative sentiment     |
| 2    | **Bobette Riner** | Sent the most negative emails overall         |
| 3    | **John Arnold**   | Frequently appeared in bottom sentiment ranks |

### Flagged Flight-Risk Employees
Identified based on 4+ negative messages in a 30-day window:

- **bobette.riner**
- **don.baughman**
- **john.arnold**
- **rhonda.denton**
- **sally.beck**

These employees showed repeated negative communication patterns that may indicate burnout, disengagement, or potential attrition risk.

---

## Key Insights & Takeaways

- **Neutral Tone Dominates**: ~69% of emails are neutral, suggesting factual or transactional communication styles dominate the workplace.
- **Positive Leaders Identified**: Johnny Palmer, Tori Kuykendall, and Kara Moriarty consistently use positive language and may be good internal culture influencers.
- **Negative Sentiment Patterns**: Kayne Coulter and Bobette Riner showed consistent negativity, which could indicate personal dissatisfaction or workplace issues.
- **Seasonal Shifts**: December 2010 saw emotional spikes – both positive and negative – potentially linked to end-of-year pressures or announcements.
- **Predictive Modeling Success**:
  - **RMSE**: 1.25
  - **MAE**: 0.87
  - **R² Score**: 0.61
  - The model confirms that emotional intensity per message is a strong predictor of monthly sentiment trends.

---

## Recommendations

1. **Engage Positive Influencers**:
   - Promote individuals like Johnny Palmer in internal communications, mentorship, or leadership roles to amplify positivity.

2. **Monitor At-Risk Employees**:
   - Conduct confidential check-ins with flagged employees to understand issues and offer support.

3. **Monthly Sentiment Reports**:
   - Regularly track sentiment scores using the modeling approach to proactively detect emerging dissatisfaction trends.

4. **Communication Workshops**:
   - Offer training to help employees craft constructive, emotionally intelligent emails—especially for teams showing negativity clusters.

5. **Enhance Culture Analytics**:
   - Expand this methodology to chat logs, meetings, or feedback systems to get a fuller picture of employee sentiment.

---

## Files in This Repository

- `test_with_roberta_sentiment.csv` – Preprocessed dataset with sentiment labels.
- `notebook.ipynb` – Full analysis pipeline: sentiment labeling, EDA, modeling.
- `README.md` – Summary of project insights, findings, and recommendations.
- `at_risk_employees.csv` – List of flagged individuals.
- `employee_sentiment_heatmap.png` – Visual showing sentiment shifts across employees.
- `top_bottom_sentiment_employees.png` – Monthly sentiment ranking charts.

---

## Tools & Libraries

- Hugging Face Transformers (RoBERTa model)
- Scikit-learn (Linear Regression, Metrics)
- Matplotlib, Seaborn (EDA, Visualizations)
- Pandas, NumPy (Data Handling)

---

## Contact
For questions or contributions, please contact **[Huzaifa Chauhan]** at [mdhuzaifachauhan.com].

