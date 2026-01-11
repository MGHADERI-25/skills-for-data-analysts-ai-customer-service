# Group Research Project Report
## **Public Attitudes Toward AI in Customer Service**
*This project examines public attitudes toward AI in customer service, using survey data to evaluate key factors such as trust, convenience, helpfulness, and ease of interaction. Statistical analyses reveal generally positive perceptions, with trust and convenience emerging as the strongest predictors of AI preference and usage intention. The findings provide clear insights into how users form opinions about AI systems and what influences their willingness to adopt them.*



## Team Members:
1. Karthik Ramu 2. Nargus Batool 3. Mohammadali Ghaderi

## Declaration

We affirm that our report is the product of our own independent research and has not been submitted, either entirely or partially, for any other evaluation. All the information and concepts that contributed to the project have been properly credited with the use of the Harvard referencing style. The generative AI tools were only consulted to assist with the idea generation and report structuring in line with the module’s Level 2 guidance on AI use; the final wording, analyses, and interpretations displayed here were composed and verified by the project team members. The dataset, analysis files, and supporting documents are in the possession of the group and can be provided to the examiners if requested.

## Executive Summary

OmniAssist Technologies is an organization that creates AI-enabled customer service tools that are implemented by banks, retailers, and the travel sector and telecoms companies. With the growing prominence of these technologies among the end-users, the company has a need for clear proof about people's attitudes toward AI interactions as compared to human interactions. This study aims to investigate the attitudes of university students toward AI and the human foals along the lines of trust, perceived helpfulness, convenience, frustration, and preferences for AI-led versus human-led customer service. The research team performed a quantitative survey with a structured questionnaire uploaded online for students aged 18–34. The responses of sixty-two participants were taken into account. The ratings given on multiple Likert-scale items were firstly grouped together and then translated into composite scores for six constructs: Trust, Helpfulness, Convenience, Ease of Interaction (low frustration), Preference for AI and Behavioral Intention. Descriptive statistics, correlations, one-way ANOVA tests and multiple regression models were performed using Python.

The findings point to a general tendency to view AI in customer service positively but with reservations. Trust and convenience are the most impactful factors behind the preference for AI; the correlations with preference are r = 0.735 and r = 0.695 respectively. A multiple regression model comprising of trust, helpfulness, and convenience explains about 81% of the variation in preference, with trust being the most important predictor. Self-reported technology comfort, however, does not have any significant effect on trust or preference, while frequency of AI use leads to greater trust and easier interactions but not to convenience. Based on these findings, it is our recommendation that OmniAssist should concentrate on the design features and deployment strategies that will build trust and reduce friction and also ensure positive initial experiences with the AI tools. Rather than completely separating users according to demographics or technology comfort level, the company should rely on usage-based journeys, open communication, and ongoing feedback loops to steer users’ confidence in the AI-enabled customer service.

## Introduction

AI quickly became a part of customer service and it has changed the business interaction with customers by providing faster, efficient and personalized support experiences. Sectors like banking, retail, travel and telecom are using AI-powered tools more, such as chatbots, virtual assistants and automated support systems for taking the customer inquiries and improving quality of service. OmniAssist Technologies, a global software company that offers AI-based customer service solutions, looks for a way to know how the public sees and interacts with these technologies. To put it differently, as AI developments continue, it will be ascertained to be critical for customer satisfaction, user trust, and long-term trust. Thus, understanding customer's service attitudes towards AI in their service environment will be the main factor in successful implementation (Wang et al., 2022).

On one hand AI systems offer several advantages, on the other hand public opinion is still not settled and remains divided. Some users of AI are praising it for its quick replies, consistent service, and always available support. Others, however, are complaining about the system’s lack of human touch, limited ability to understand and solve issues, and their potential to get lost in communication. In addition, customer trust in AI is determined by the level of transparency, security of personal data, and the company’s ability to interact effectively. These different opinions stress the need for research to find out how users rate AI in customer service against human agents. Understanding such attitudes can assist OmniAssist Technologies in setting proper product development cycle, marketing strategies, and customer training programs that meet the expectations of consumers.

The research question guiding this study is:

* What are the public attitudes toward AI in customer service, and how do trust, helpfulness, convenience, and frustration influence preferences for AI-led versus human-led interactions?  

## Methodology
This study adopted a quantitative, survey-based design to explore attitudes toward AI in customer service among university-aged respondents. A structured online questionnaire allowed us to capture standardized ratings on multiple constructs and to link these two basic demographic and behavioral variables.

### Data collection and population

Google Forms survey was used to gather data. The link was shared via university WhatsApp groups, cohort chats, and personal social media networks. The target population was students and young adults (approximately 18–34 years old) who frequently interact with digital services and are thus prone to meet AI-powered customer support in areas such as banking, e-commerce, and travel. Participation was compulsory and non-identifying. We did not obtain names, email addresses or other direct identifiers. The dataset eventually used for the analysis contained 62 valid responses after the exclusion of incomplete or inconsistent entries.

### Survey instrument and measures

The questionnaire included Likert-scale items grouped into six constructs informed by prior research on AI acceptance and technology adoption (Bristows, 2019; Granlund and Lundström, 2024):

- Helpfulness (five items) – perceived ability of AI tools to provide useful and accurate support.
- Convenience (four items) – time-saving, availability, and suitability for simple queries.
- Ease of Interaction (six items) – clarity, smoothness, and perceived effort when interacting with AI.
- Trust (five items) – perceived reliability, credibility, and alignment with customers’ best interests.
- Preference for AI (four items) – relative preference for AI versus human agents in routine tasks.
- Behavioral Intention (five items) – willingness to reuse, recommend, and continue relying on AI tools.

All attitudinal items were rated on a five-point Likert scale from 1 (“Strongly disagree”) to 5 (“Strongly agree”). Demographic questions covered age group, gender, education level, region, self-reported comfort with new technologies, and frequency of interacting with AI customer service tools.

### Data preparation and analytical tools

The final data set was first exported as survey_final.csv and then analyzed using Python on the Google Colab platform. For cleaning and transforming data, the panda’s library was utilized, whereas descriptive and inferential statistics were carried out with pingouin and scipy.stats, and lastly, the ANOVA and regression models were created with statsmodels. The process of visualization included the use of matplotlib, seaborn, and sometimes plotly for the exploratory plots in the notebook. A composite score for each construct was calculated by taking the average of the corresponding Likert items for each respondent. These composites became the primary variables for our analyses. The cleaned dataset and the steps of the analysis are presented in the file 1.ipynb.

### Analysis Plan and Hypotheses

Our research analysis followed the study's recommendations for small-sample survey research (n ≈ 60) and first provided descriptive statistics (means and standard deviations) for each construct. Subsequently, it correlated the variables Helpfulness, Convenience, Ease of Interaction, Trust, AI Preference, and Intention to Use using Pearson’s r. One-way ANOVA was then applied to conduct group comparisons based on the participants' self-reported tech comfort and the frequency of their AI customer service use. The regression modeling technique was utilized to assess the collective predictive power of Trust, Helpfulness, and Convenience for either AI Preference or Behavioral Intention. The major hypotheses that guided the analysis were that Trust would be positively related to AI Preference in customer service (H1); the influence of Trust on Preference would be through Convenience (H2); the differences between Trust and Preference would be significant for self-reported tech comfort (H3); the difference between Trust, Convenience, and Ease of Interaction would be significant for AI usage frequency (H4), and the multi-predictor model of Trust, Helpfulness, and Convenience would account for a large share of the variance in AI Preference or Behavioral Intention (H5). 

---

## Results
### Descriptive Analysis

The descriptive statistics provide an initial understanding of respondents’ overall attitudes toward AI customer service. Composite means indicate moderately positive but generally cautious evaluations on a five-point Likert scale (1 = strongly disagree, 5 = strongly agree). Convenience (M = 3.05, SD = 0.86), Preference for AI (M = 3.00, SD = 1.01), and Behavioral Intention (M = 2.96, SD = 1.02) were the highest-rated constructs, suggesting that respondents slightly agreed that AI offers functional advantages and that they might use such systems again. In contrast, Ease of Interaction (M = 2.85, SD = 0.80), Helpfulness (M = 2.74, SD = 0.90), and Trust (M = 2.71, SD = 0.88) remained close to the midpoint. These lower scores imply reservations regarding AI’s understanding, reliability, and interpretive capability. 

![Trust in AI by Tech Comfort](Charts/1.png)

![Which AI Constructs Score Highest and Lowest?](Charts/16.png)

![Profile of Attitudes Toward AI Customer Service](Charts/18.png)

### Correlations among key constructs

The output of the correlation analysis was that all key variables had very strong, positive relationships between them. The variables Helpfulness, Convenience, Ease of Interaction, and Trust had very high inter-correlations with values between approximately r ≈ 0.65 and r = 0.84. Not only this, but also the Preference for AI and Behavioral Intention showed very high correlation with the other constructs, r ≈ 0.69–0.87, which means that good experiential evaluations are very much associated with stronger preferences and a higher likelihood of use of AI interfaces again. Trust was recognized as a particularly important concept, as it had strong correlations not only with Preference for AI (r ≈ 0.72) but also with Behavioral Intention (r ≈ 0.80). The findings that both Trust and perceived Convenience are very important factors in the process of AI acceptance at the correlational level, thus providing support for H1 and H2 in this respect. The situation is similar to what is found in the established technology acceptance research, especially TAM and related models, where trust and perceived usefulness are always the primary factors influencing user attitudes and behavioral responses.

![Correlation Matrix of AI Attitude Constructs](Charts/9.png)

![Correlation Matrix: Trust, Convenience, Behavioral Intention](Charts/19.png)

![Trust vs Behavioral Intention](Charts/14.png)

![Convenience vs Behavioral Intention](Charts/15.png)

### Group differences by tech comfort (H3)

One-way ANOVA was the statistical method of choice to figure out the level of the radically different attitudes that might at the top be associated with the self-reported respondents' levels of technology comfort. The major findings did not indicate statistically different outcomes for Trust, F(3,56) ≈ 0.58, p ≈ 0.63, nor for Preference for AI, F(3,56) ≈ 1.59, p > 0.05. However, the group of "very comfortable" described themselves slightly more positively, but the differences were small enough not to be counted as statistically significant. Thus, the hypothesis was rejected. In light of this, it is seen that the finding holds that technology is not a barrier in the case of negative attitudes towards AI customer service, while the opposite holds for positive attitudes. In addition, the central point of this finding is the already-stated nature of the case that acceptance of AI systems relies much more on the prior experience with specific AI tools, perceived fairness, and perceived quality of interaction rather than on the general technology skill level.

![Trust in AI by Tech Comfort](Charts/5.png)

![Preference for AI by Tech Comfort](Charts/6.png)

![Distribution of Trust Scores by Tech Comfort](Charts/3.png)

![Distribution of Preference Scores by Tech Comfort](Charts/4.png)

### Group differences by AI usage frequency (H4)

Differences in attitudes were also examined based on respondents’ frequency of AI customer service use. The ANOVA results showed significant effects for Trust, F(2,57) ≈ 6.44, p ≈ 0.003, and Ease of Interaction, F(2,57) ≈ 3.52, p ≈ 0.04. Respondents who used AI customer service tools more frequently reported higher trust levels and smoother interaction experiences. The effect for Convenience approached significance, F(2,57) ≈ 2.90, p ≈ 0.06, but did not meet the 5% threshold. These results provide partial support for H4, indicating that familiarity and repeated exposure improve user confidence and interaction quality, although perceived convenience may be recognized regardless of usage frequency. This trend is consistent with previous research demonstrating that repeated exposure reduces uncertainty and builds trust over time.

![Trust in AI by AI Interaction Frequency](Charts/7.png)

![Ease / Low Frustration by AI Interaction Frequency](Charts/8.png)

### Regression models (H1, H2, H5)

Regression analyses were carried out to investigate the predictive relationships between Trust, Helpfulness, Convenience, Preference for AI, and Behavioral Intention. In the bivariate models, Trust alone was responsible for the largest portion of the variance in Behavioral Intention (R² ≈ 0.63). On the other hand, Convenience was given a smaller but still considerable share of variance (R² ≈ 0.48). The three single predictor’s model of Trust, Helpfulness, and Convenience performed very well with R² ≈ 0.71 and all predictors being significant (p < 0.05). Trust was by far the strongest predictor, making its fundamental importance for future interaction with AI systems clearly visible. The same predictive model for Preference for AI made it possible to obtain the R² value of about 0.65, with Trust being the most important factor again. These findings confirm hypotheses H1, H2, and H5, demonstrating that Trust and the perception of Convenience significantly influence the preference for AI, while the joint model offers an excellent explanation of the behavioral intentions. 

![Regression Coefficients Predicting Behavioral Intention](Charts/10.png)

![Interaction: Trust × Convenience](Charts/13.png)

![Low Trust vs High Trust: Convenience & Behavioral Intention](Charts/12.png)

---

## Discussion
The results indicate that although the respondents acknowledge the advantages of AI customer service in terms of convenience and efficiency, they still have doubts concerning its trustworthiness and the possibility of a human-like interaction. Trust emerged to be the primary factor influencing both Preference for AI and Behavioral Intention, thus coinciding with existing studies which emphasize the importance of reliability, transparency, and ethical data use for AI to be accepted. Technology comfort was not a significant factor in shaping attitudes, but rather, frequent AI users indicated higher trust and smoother conversations, which implies that personal experience—not digital skill perceived by others—creates confidence. The above-mentioned findings suggest that organizations ought to invest in the creation of user-friendly, patient onboarding that guides the potential users in getting used to the AI systems. Nevertheless, the limited size of the sample, which mainly consisted of students, restricts the generalization of the results, therefore indicating the necessity of wider future research. 

## Recommendations
The study's conclusions offer multiple recommendations to assist OmniAssist Technologies in the sphere of artificial intelligence (AI) customer support tools, which are capable of boosting user trust, adoption, and satisfaction. To begin with, trust should be given top priority at every stage of system design and deployment since it was the strongest predictor of AI preference and user intention. As a result, OmniAssist should convince users of its commitment to transparency by giving detailed information about the AI system’s operation, the data collection, and the measures taken for privacy protection. Besides, users can be kept confident through the incorporation of explainable AI responses, visible security cues, and consistent interaction patterns.

Next, the focus has to be on the removal of deterrents and enhancement of interactivity that the customer experiences—first-time users in particular. As the frequent users reported having higher trust and smoother interactions, OmniAssist should come up with early experiences that are easily understandable and do not cause frustration at all. Negative initial impressions can be averted through techniques such as ushering new users through the setup process, offering personalized tips, and straightforwardly handling mistakes, as well as prompt issue escalation when AI reaches its limits.

Third, since the comfort with technology did not considerably affect the trust or preference, the company should not segment its customer base on the basis of demographics. A more effective technique is user-based personalization which modifies the support level, interface sophistication, and guidance in accordance to the users’ actual interaction habits instead of the assumed skill levels. 

## Reflection on Team Process

Our group applied the Agile and Kanban methodologies learned during the SKIB353 course to carry out the project in an efficient manner. A team Kanban board was used to organize the tasks, which were survey design, data cleaning, coding in Python, and writing, while at the same time preventing overload and increasing visibility. The short meetings enabled us to quickly change our plans and fix any problems that arose. Although initially, not all the team members were confident using Python, its use helped with the reproducibility and analytical depth, and GitHub was the tool that made the async collaboration the smoothest one. The adoption of an iterative agile mindset was what allowed us to continuously improve our work and, finally, produce a report for OmniAssist that was clear and data-driven.

---

## References and Appendices

### References

* Bristows LLP (2019) *Artificial Intelligence: Public Perception, Attitude and Trust*. London: Bristows LLP.
* Bryman, A. (2016) *Social Research Methods*. 5th edn. Oxford: Oxford University Press.
* Field, A. (2018) *Discovering Statistics Using IBM SPSS Statistics*. 5th edn. London: Sage.
* Granlund, J. and Lundström, D. (2024) *Unveiling the Impact of AI-Powered Chatbots on Customer Acceptance in Sweden*. Bachelor thesis. Mälardalen University.
* Nature HSSC (2024) ‘Exploring the mechanism of sustained consumer trust in AI chatbots after service failures: a perspective based on attribution and CASA theories’, *Humanities and Social Sciences Communications*, 11, pp. 1–15.
* Pallant, J. (2020) *SPSS Survival Manual*. 7th edn. Maidenhead: McGraw-Hill Education.
* Schulz, P.J. et al. (2023) ‘Modeling the influence of attitudes, trust, and beliefs on endoscopists’ acceptance of artificial intelligence applications in medical practice’, *Frontiers in Public Health*, 11, 1301563.
* SKIB353 Module Materials (2025) *Skills for Data Analysts: Empirical Research Guidance*.
* University Moodle Resources, Weeks 1–3.
* Wang, X., Lin, X. and Shao, B. (2022) ‘How does artificial intelligence create business agility? Evidence from chatbots’, *International Journal of Information Management*, 66, 102535.

---
### Appendices Appendix

#### A. Survey questionnaire (full list of Likert items and demographic questions). 

##### Survey on Public Attitudes Toward AI in Customer Service 

###### Introduction Text 

Thank you for taking part in this short anonymous survey about customer service experiences.  
Your responses will help us understand how people perceive the use of artificial intelligence (AI) tools such as chatbots and virtual assistants in customer service.  
The survey takes about 5 minutes to complete.  

---

##### Section 1: Screening and Background 

*(To ensure participants have basic familiarity with the topic.)*  

1. Have you ever interacted with an AI-based customer service tool (for example, a chatbot or virtual assistant)?  
   - o Yes  
   - o No  
   - o I’m not sure  

2. How often do you interact with AI customer service tools?  
   - o Frequently  
   - o Occasionally  
   - o Rarely  
   - o Never  

3. In which of the following service areas have you experienced AI-based customer service? (Select all that apply)  
   - o Retail or online shopping  
   - o Banking or financial services  
   - o Telecommunications or internet services  
   - o Travel or hospitality  
   - o Healthcare  
   - o Other sectors  
   - o I have not used any  

---

##### Section 2: Perceived Helpfulness of AI 

*(5-point Likert scale: 1 = Strongly Disagree → 5 = Strongly Agree)*  

4. AI customer service tools help me find the information I need efficiently.  
5. AI systems are able to provide accurate answers to my questions.  
6. AI tools make it easier to solve simple service-related issues.  
7. I am usually satisfied with the results provided by AI customer service systems.  
8. AI customer service tools improve my overall experience with the company.  

---

##### Section 3: Perceived Convenience 

*(5-point Likert scale)*  

9. Using AI customer service tools saves me time.  
10. AI systems are available whenever I need assistance.  
11. I find it easy to access AI-based support on company websites or apps.  
12. The process of interacting with an AI chatbot or assistant is straightforward.  
13. AI-based customer service helps me resolve issues without waiting in line for human support.  

---

##### Section 4: Perceived Trust 

*(5-point Likert scale)*  

14. I believe AI customer service tools provide reliable information.  
15. I trust AI chatbots to handle my customer queries properly.  
16. I feel confident that AI systems respond to my requests accurately.  
17. I consider AI-based customer service tools credible.  
18. I believe AI assistants are designed to serve customers’ best interests.  

---

##### Section 5: Perceived Frustration (Low-friction Focus) 

*(5-point Likert scale — all positive phrasing to avoid emotional/negative tone)*  

19. I find it easy to communicate my needs when using AI customer service tools.  
20. AI systems usually understand my questions correctly.  
21. Interacting with AI systems feels smooth and efficient.  
22. AI tools guide me clearly through the support process.  
23. AI-based customer service meets my expectations most of the time.  

---

##### Section 6: Preference for Human vs. AI Interaction 

*(5-point Likert scale)*  

24. AI customer service is suitable for handling simple inquiries.  
25. I prefer using AI tools when I need quick answers.  
26. I am comfortable relying on AI systems for common service tasks.  
27. I believe human agents should focus on complex issues, while AI handles routine ones.  
28. I would be willing to use AI customer service again in the future.  
29. I would recommend AI-based customer support to others.  
30. I believe companies benefit from using AI alongside human customer service teams.  

---

##### Section 7: Demographic Information 

*(Optional and non-intrusive — no personal data)*  

31. What is your age group?  
   - • Under 18  
   - • 18–24  
   - • 25–34  
   - • 35–44  
   - • 45–54  
   - • 55–64  
   - • 65 or older  

32. What is your gender?  
   - • Male  
   - • Female  
   - • Non-binary / other  
   - • Prefer not to say  

33. What is your highest level of education completed?  
   - • High school or equivalent  
   - • Some college or diploma  
   - • Bachelor’s degree  
   - • Master’s degree  
   - • Doctorate or higher  
   - • Prefer not to say  

34. Which region or country do you currently live in?  
   - • Africa  
   - • Asia  
   - • Europe  
   - • North America  
   - • South America  
   - • Oceania  

35. How comfortable are you using new technologies in daily life?  
   - • Very comfortable  
   - • Somewhat comfortable  
   - • Neutral  
   - • Slightly uncomfortable  
   - • Very uncomfortable  

---

##### Response Scale Reminder 

All attitude statements (Questions 4–30) use a 5-point Likert scale:  

1 = Strongly Disagree  
2 = Disagree  
3 = Neutral  
4 = Agree  
5 = Strongly Agree  

---

##### Construct Mapping 

| Construct                  | Question Numbers |
|----------------------------|------------------|
| Helpfulness                | 4–8              |
| Convenience                | 9–13             |
| Trust                      | 14–18            |
| Frustration (low-friction) | 19–23            |
| Preference                 | 24–30            |
| Demographics               | 31–35            |

--- 
#### B.	Appendix B. Python analysis notebook (a3_analysis.ipynb), including full code and additional exploratory figures. 
[Click here to view the Python Notebook](A3_analysis.pynb)
---
#### C. Additional charts not embedded in the main report (exported as .png and linked from the Results section).

![Behavioral Intention by Gender](Charts/17.png)