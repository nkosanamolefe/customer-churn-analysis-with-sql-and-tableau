# Customer Churn Analysis with SQL and Tableau

# Background and Overview
365 is an e-Learning company offering pre-recorded lessons, exercises, quizzes, exams, and real-world projects on a subscription-based model, providing access to various courses and certification tracks.

The company is facing a critical challenge of understanding and mitigating subscriber churn. The company aims to identify the key factors driving customer churn, analyze the impact of churn on revenue, and implement strategies to improve customer retention.

<details>
  <summary>Understanding Churn (Click to Expand)</summary>
  Churn is a term used to describe the rate at which customers stop doing business with a company. Understanding churn is crucial because it directly impacts a company's growth and profitability.

Here's why it's important:
- Losing customers is expensive: It costs more to acquire new customers than to retain existing ones. 
- Churn impacts revenue: Losing customers means losing revenue, which can negatively impact a company's bottom line.
- Churn reveals problems: High churn rates can indicate issues with products, services, pricing, or customer service, all of which need to be addressed.

By understanding churn, companies can take steps to reduce it and improve customer loyalty, ultimately leading to greater success
</details>

**Insights and recommendations are provided in the following key areas:**

- **Customer churn:** Evaluation of net revenue generated by 365 and comparison to previous periods.
- **Customer retention:** Assessment of customer retention rate and its differences across subscription plans and customer segments.

# Data Structure Overview
365's database structure as seen below consists of 3 tables: students, purchases and subscriptions with a total records of .

![image](https://github.com/nkosanamolefe/customer-churn-analysis-with-sql-and-tableau/blob/main/data/data-structure.png)

# Executive Summary
365, has demonstrated strong performance in customer retention while facing some challenges in refund management. The company generated net revenue of $666,720 between December 2021 and October 2022, representing a modest growth of 0.93% compared to the previous period.
A significant achievement has been the reduction in customer churn rates from 9% to 4% between December 2021 and October 2022, substantially outperforming industry benchmarks of 5-20%. This improvement indicates strong product-market fit and effective retention strategies. However, the company maintains a 10% refund rate, while aligned with industry standards, presents an opportunity for optimization.

Marketing campaigns have proven particularly effective for annual subscriptions, with new customer acquisition reaching peaks during promotional periods, notably exceeding 1,049 new subscribers during the Black Friday promotion. The monthly subscription model shows strong retention, with approximately 70% of customers maintaining recurring subscriptions.

Geographically, the United States leads in lifetime revenue generation at $640,102, benefiting from high disposable income and advanced technological adoption. Nigeria has emerged as a promising market in Africa, generating $37,441 in revenue.

To maintain this positive trajectory, 365 should focus on reducing refund rates through improved product quality and customer expectation management, while continuing successful retention strategies. The company should also consider targeted expansion in high-performing markets through localized content and strategic partnerships, particularly in Spanish-speaking regions where language barriers create competitive advantages.

These findings suggest that while 365 has established a strong foundation in customer retention and market presence, strategic investments in product quality, market expansion, and customer experience will be crucial for sustained growth and profitability.

# Insights Deep Dive
## **Revenue and Churn**
### Net Revenue and Refunds

Net revenue generated for the period of December 2021 - October 2022 is $666,720, which is a slight increase of about 0.93% compare to the previous period. There were notable peaks, with the most significant peak occurring in January 2021 ($86,355).

The industry benchmark for refunds is around 10%, and 365’s average refund rate is also around 10% with refund rate for October 2022 at 11%. 
Reasons for high refund rates: 
- Product quality: Learning curve steeper than customer expectations
- Rising inflation in 2022: Increased price sensitivity among customers
- Increased sales: Volume-driven promotions attracting price-sensitive customers
- Clients switching their plan: Discovery of better-suited subscription tiers

### Churn rate

The company's impressive churn rate reduction across all customer segments - from concerning levels of 9% in December 2021 to much healthier rates of 4% respectively by October 2022 - significantly outperforms industry benchmarks (5-20% for online subscriptions and 10-15% for e-Learning), indicating strong product-market fit and effective customer retention strategies.

![image](https://github.com/nkosanamolefe/customer-churn-analysis-with-sql-and-tableau/blob/main/data/images/Net%20Revenue%20and%20Churn%20Rates.png)

## **New vs Recurring Customers**

In November, all subscription categories lifetime, annual, and monthly experienced a notable surge in new customer acquisitions, surpassing 1,049, attributed to the Black Friday promotion.

**Annual Subscription**: Most marketing campaigns promote the annual plan, resulting in an average of 65% new customers subscribing during odd months compared to recurring customers. New subscriptions during non-campaign months stem from organic traffic and evergreen campaigns.

**Monthly Subscription**: Recurring monthly subscriptions comprise about 70%.

In conclusion, marketing campaigns are effective in bringing in new customers.

![image](https://github.com/nkosanamolefe/customer-churn-analysis-with-sql-and-tableau/blob/main/data/images/New%20vs%20Recurring%20Customers.png)

## **Revenue by Country**
The US market has demonstrated strong performance with revenue of $640,102 and an average order value of $99, leveraging key market advantages. The nation's expansive consumer base of 330 million people, combined with high disposable income levels, creates significant market opportunity. The US position as a global technology leader, particularly in hubs like Silicon Valley, fosters rapid adoption of new products. Additionally, the unified English-speaking market enables efficient operations and marketing initiatives, streamlining customer engagement efforts.

Nigeria is the only African country in the top ten, with a revenue of $37,441 and an average order value of $96, Nigeria represents an emerging market with significant growth potential. The country's emphasis on digital skills development through government and private sector initiatives has created a foundation for technology adoption and market expansion. Nigeria's IT sector is experiencing rapid growth, particularly in Lagos and Abuja, which serve as technology hubs for West Africa.

Spain shows strong market engagement with revenue of $31,610 and an impressive average order value of $103. The country's high-income economy and substantial market size of 47 million consumers provide significant growth potential. While the Spanish-language market requires localized approach and dedicated resources, this investment barrier creates a competitive advantage for established operations. The market's advanced infrastructure and concentrated urban populations in Madrid, Barcelona, and Valencia support efficient market penetration and scalability opportunities.

![image](https://github.com/nkosanamolefe/customer-churn-analysis-with-sql-and-tableau/blob/main/data/images/Revenue%20by%20Country.png)

# Recommendations
### Address Refund Rates
**Investigate the Root Causes**: While the analysis provides potential reasons for high refunds, 365 should conduct a deeper dive to pinpoint specific issues. This could include:
- **Customer Surveys**: Gather direct feedback from customers who requested refunds about their specific pain points.
- **Course Content Review**: Ensure the course material is clear, up-to-date, and meets stated expectations, and that the learning curve is properly managed.
- **Sales and Marketing Alignment**: Verify that marketing materials accurately represent the learning experience to avoid misleading potential students.
- **Improve Product Quality:** Regularly update content to ensure it remains fresh and relevant by adapting to field changes and addressing user-reported issues.
- **Manage Pricing and Promotions:** Evaluate the effectiveness of volume-driven promotions. Perhaps these should be more focused on students with a higher likelihood of long-term engagement, rather than solely on price-sensitive customers.
- **Simplify Plan Switching:** Make the process of switching to a different subscription tier smoother, minimizing dissatisfaction and refunds by making this a good option for the student.

### Churn
**Maintain Low Churn Rates:**
**Sustain Customer Retention Efforts:** 365 has done a great job at reducing churn. They should continue implementing successful strategies and closely monitor churn rates for any early warning signs.

### New vs. Recurring Customers
Optimize Campaigns for Annual Subscriptions Formulate comprehensive organic growth strategies aimed at attracting students who will become loyal, repeat customers.
Boost Monthly Subscription Engagementby offering personalized recommendations for new content or courses to recurring customers based on their previous engagement to keep them engaged.
Balance Acquisition and Retention:
*   **Strategic Marketing:** Don't solely focus on bringing in new customers. Ensure marketing efforts also retain and engage existing customers.
*   **Customer Lifecycle Management:** Implement a customer lifecycle management strategy that focuses on long-term engagement and reduces churn.

### Revenue by Country

**1. Capitalize on US Market Strengths:**

*   **Partnerships:** Partner with US-based institutions or businesses to expand reach.
*   **Optimize for US:** Develop marketing approaches suited for US consumers.
*   **Maintain High Standards:** Keep up with evolving industry standards in tech to stay relevant in a fast-paced environment.

**2. Leverage Nigerian Market Growth:**

*   **Digital Skills Programs:** Invest in digital skills development programs in collaboration with government and local partners in Nigeria.
*   **Tailor Curriculum:** Develop courses relevant to Nigerian IT and skills gaps.
*   **Strategic Partnerships:** Seek out local partnerships to improve operations.

**3. Expand in the Spanish Market:**

*   **Localized Content:** Create Spanish language courses and resources, and tailor the content to the specific learning needs of Spanish students.
*   **Dedicated Support:** Invest in dedicated customer support, in the Spanish language.
*   **Targeted Marketing:** Develop marketing strategies targeted at Spanish-speaking areas, emphasizing the quality and value of 365’s course offerings.
*   **Competitive Edge:** Capitalize on the language barrier to establish a competitive advantage.

**4. Global Market Expansion:**

*   **Market Research:** Invest in in-depth market research before expanding into new areas.
*   **Gradual Approach:** Take a gradual approach, initially focusing on markets with the highest potential.

By implementing these recommendations, 365 can further reduce churn, enhance customer loyalty, and drive sustainable revenue growth across various markets. Remember to continuously track results to measure impact and identify further opportunities for optimization.
