# **Twitter Sentiment Analysis Using NLP**

## **Introduction**  
This project analyzes **73,996 tweets** from the `twitter_training.csv` dataset to understand public sentiment using Natural Language Processing (NLP). The dataset includes columns like `Tweet Content`, `Sentiment` (labeled as Positive/Negative/Neutral/Irrelevant), and `Entity` (e.g., brands, topics). The goal is to compare **traditional sentiment labels** with **NLP-based sentiment scores** (using TextBlob) and uncover patterns in public opinion.

---

## **Objective**  
1. **Compare traditional sentiment labels** (pre-classified) with **NLP-derived sentiment** (TextBlob).  
2. **Quantify sentiment intensity** using polarity scores (-1 to +1).  
3. **Identify extreme sentiments** (most positive/negative tweets) for actionable insights.  

---

## **Steps Conducted**  

### **1. Data Preprocessing**  
- **Handled Missing Values**: Dropped rows with null entries.  
- **Traditional Sentiment Distribution**: Visualized labeled sentiments (Positive, Negative, Neutral, Irrelevant).  

### **2. NLP Sentiment Analysis**  
- **TextBlob Implementation**:  
  - **Categorized Tweets**: `Positive` (polarity > 0), `Negative` (polarity < 0), `Neutral` (polarity = 0).  
  - **Polarity Scores**: Calculated continuous scores (-1 to +1) for granular sentiment analysis.  

### **3. Comparative Analysis**  
- **Traditional vs. NLP Labels**: Stacked bar chart showing alignment/misalignment between manual labels and NLP predictions.  
- **Key Findings**:  
  - **Discrepancies**: Some tweets labeled "Neutral" in traditional analysis were classified as "Positive" or "Negative" by NLP.  
  - **Strong Agreement**: Most "Positive" labeled tweets aligned with NLP's "Positive" class.  

### **4. Sentiment Intensity Analysis**  
- **Distribution Plot**: Majority of tweets had **mild positivity** (mean polarity: 0.077).  
- **Extreme Sentiments**:  
  - **Most Positive**: "Platinum is the best loot @Borderlands" (polarity = 1).  
  - **Most Negative**: "What terrible bitch!" (polarity = -1).  

---

## **Key Insights**  
1. **Sentiment Distribution**:  
   - **Traditional Labels**: Dominated by "Neutral" and "Positive" sentiments.  
   - **NLP Scores**: Revealed hidden negativity in tweets labeled "Neutral."  

2. **NLP Advantages**:  
   - Detected **nuanced sentiments** (e.g., sarcasm, mild positivity) missed by manual labels.  
   - Provided **quantifiable metrics** (polarity scores) for trend analysis.  

3. **Business Applications**:  
   - **Brand Monitoring**: Identify negative tweets for crisis management (e.g., "@EpicGames" complaints).  
   - **Campaign Optimization**: Leverage highly positive tweets (e.g., "@Borderlands" praise) for marketing.  

---

## **Conclusion**  
The project demonstrated **NLP's superiority** in capturing nuanced sentiments compared to traditional labels. While TextBlob provided granular polarity scores, future work could:  
- Use **advanced models** (BERT, VADER) for context-aware analysis.  
- Address **sarcasm/irony detection** to improve accuracy.  

**Tools Used**: Python, Pandas, TextBlob, Matplotlib, Seaborn  
**Author**: Jay Thakur
