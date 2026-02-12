# Customer Support Chatbot Analysis

This repository contains the analysis of customer support chatbot conversations, including clustering by intent, sentiment & urgency analysis, handoff detection, and conceptual design of a next-generation agentic AI system.

---

## **Dataset**

- File: `CustomerSupportSample.json`
- Contains 678 customer support conversations 
- Columns: `index`, `conversation`, `category`

---

## **Analysis Pipeline**

1. **Data Loading & Cleaning**
   - Remove special characters and speaker labels
   - Remove Arabic stopwords
   - Normalize conversation text

2. **Feature Extraction**
   - TF-IDF vectorization with unigrams and bigrams

3. **Clustering**
   - K-Means clustering to identify conversation intents
   - Top terms per cluster for labeling

4. **Handoff Detection**
   - Detect bot → human agent escalations using keywords

5. **Sentiment & Urgency**
   - Sentiment classification: Positive / Neutral / Negative
   - Urgency detection: Low / Medium / High

6. **Handling Quality**
   - Determine whether issues were resolved or unresolved

7. **Visualization**
   - Cluster distribution, sentiment distribution, handoff detection

8. **Agentic AI Design (Conceptual)**
   - High-level flow integrating intent detection, sentiment, urgency, automated response, and human escalation

---

## **Results Summary**

- **Clusters**: 12 clusters labeled by intent, bot templates, and support actions
- **Handoff**: 487 conversations required human agent intervention (~72%)
- **Sentiment**: 357 Positive, 242 Neutral, 79 Negative
- **Urgency**: 471 Medium, 153 High, 54 Low
- **Handling Quality**: 336 Unresolved, 179 Resolved, 163 Unknown

**Insights:**
- Majority of queries still need human intervention
- Automated bot responses can handle FAQs and standard requests
- Urgent or unresolved issues are escalated to maintain customer satisfaction
- Proposed agentic AI system improves efficiency and continuous learning

---


