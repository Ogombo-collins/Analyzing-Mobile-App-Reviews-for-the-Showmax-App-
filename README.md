# Analyzing-Mobile-App-Reviews-for-the-Showmax-App-
A Natural Language Processing (NLP) Project focused on: Analyzing customer sentiment to understand how users interact with the Showmax app, thus improving their experience and the quality of the Showmax App. 

![Snapshot of Showmax’s Original Shows from Showmax Homepage](https://github.com/Ogombo-collins/Analyzing-Mobile-App-Reviews-for-the-Showmax-App-/blob/main/Showmax%20Home%20Page.png)

## Showmax App
[Showmax](https://www.showmax.com/ke?) is a subscription video-on-demand service. The streaming platform hosts a variety of content in its library, including original TV shows and films, serving underserved market segments such as Africa. It operates in 70+ markets across Africa and Eastern Europe. 
Launched in South Africa in 2015, Showmax has been streaming local content that has garnered strong support from the African customer base.

# Project Outline: Analyzing Showmax’s Mobile App Reviews


Analyzing customer sentiment to understand how users interact with the Showmax app, thus improving their experience and the quality of the product-streaming platform and the content library is important for Showmax. Mobile app reviews provide app users' explicit reactions, frustrations, and opinions. 

The analysis will follow the following phases:
1. Data Scraping Plan
2. Exploratory Data Analysis
3. Dataset profile
4. Data Pre-processing: Data cleansing actions
5. Exploratory questions: Answering key questions linked to the dataset
6. Sentiment Analysis: Conduct sentiment analysis using algorithms like TextBob, VADER and Huggie's NLP pre-trained models to determine the sentiment (positive, negative, neutral) of each review
7. Keyword Analysis: Identify common themes and issues affecting Showmax app users
8. User segment analysis: Segment users based on review patterns
9. Summarized Insights
10. Recommendations

**Key facts about the Showmax Mobile App**:
- Mobile app downloads are 1M+
- Overall app rating is 4.1
- Total number of reviews submitted by users is 80,262
- App genre is Entertainment
- Content rating is Teenager
- Date of the last update: 17th October 2024
- Developer/App owner is Showmax Africa Holdings Limited

**Data Collection**

The data collection plan entails acquiring Showmax app mobile reviews from Google Playstore and analysing them. The data collection method uses the Google Play Scrapper library to collect mobile review data. Only relevant mobile app reviews were retrieved from Google Playstore.

**Showmax Dataset Profile**

The dataset contains 12,009 data points(rows) and 11 columns. 
Columns present in the dataset include:
- reviewId: Unique identifier for each review
- userName: Name of the user who posted the review
- userImage: URL of the user’s profile image
- content: Text content of the review
- score: Star rating given by the user (1-5)
- thumbsUpCount: Number of thumbs-up (likes) the review received
- reviewCreatedVersion: Version of the app when the review was created
- at: Date and time when the review was posted
- replyContent: Content of the developer’s reply to the review
- repliedAt: Date and time when the developer replied to the review
- appVersion: Version of the app when the review was posted

**Data Analytics Notebook**

This  [Jupyter notebook](https://github.com/Ogombo-collins/Analyzing-Mobile-App-Reviews-for-the-Showmax-App-/blob/main/Showmax_Reviews_NLP_Project_2024.ipynb), hosted on my GitHub page, contains detailed analysis (Python code scripts). Please feel free to look it over.

# Showmax App Reviews Summarized Insights

The overarching insights obtained from the NLP project entails:


1. 1-Score reviews dwarfed others by leading with 7,771 1-Score reviews submitted by Showmax users

2. Showmax **App version 4.12.21** had the highest number of reviews submited by Showmax App users, about **3,633** reviews. In contrast, **App verison 5.9.32** had the lowest number of reviews submitted by Showmax users, about 7 reviews.


3. Based on review scores metric, the best-performing version of the Showmax app was App version 5.9.33. **App version 5.9.33** received the highest average review score of 3.5. The number of reviews submitted by users for App version 5.9.33 was 182. **App version 1.10.74** received the lowest average review score of 1.2.

4. The low average score App version 1.0.0 contrasts the number of reviews it received, 1474 reviews.

5. In general, the **average sentiment score is 0.98.** This means the majority of reviews expressed by Showmax App users are positive.

6. In terms of segmenting number of reviews per sentiment score, **about 11,120 reviews**, the leading number of reviews, had a sentiment score ranging between **0.975 and 1.02**. In contrast, only 39 reviews had a relatively low positive score ranging between 0.62 and 0.67

7. In terms of topic modeling and frequency of words analysis:

  **Topic 0**

  * Top words include: ['like', 'old', 'series', 'showmax', 'just', 'watch', 'shows', 'watching', 'new', 'app']

  * In terms of volume of words relating to the top 3 sub-themes:

    a) ***app*** : 1,296 mentions

    b) ***new*** : 1,036 mentions

    c) ***watching***: 793 mentions

  The three sub-themes represent what showmax users care about the most when interacting with the app based on app reviews: the app's experience, new interface and the streaming experience.

  **Interpretation**:

* **Themes**: This topic focuses on showmax's **app user interface and user experience**, based on the frequency of words such as 'watch', 'showmax', 'old','new', 'shows' and 'series'. Some users most likely prefer the old version of the showmax app and some like the new updated version based on access to quality content.

* **Insights**: Users who commented using keywords grouped in this topic are likely to continue using the app or churn based on the user interface and user experience of the showmax app. Customer-centric UI/UX and showmax's content library quality are important for showmax users.

  **Topic 3**

  * Top words include: ['play', 'subscription', 'doesn', 'phone', 'keeps', 'new', 'showmax', 'watch', 'tv', 'app']

  * In terms of volume of words relating to the top 3 sub-themes:

    a) ***app*** : 1,480 mentions

    b) ***tv*** : 1,277 mentions

    c) ***watch***: 977 mentions

The three sub-themes represent what showmax users care about the most when interacting with the app based on app reviews: app (functionality), tv (integration with television and tv streaming experience) and streaming experience.

**Interpretation**:

* **Themes**: This topic focuses on showmax's **app performance and integration capabilities**  in terms of users paying for subscriptions, integrating showmaxapp with televion set for a family or group watching experience and quality of mobile app  based on frequency of words such as 'subscription', 'tv', 'play' 'new', and 'watch'.

* **Insights**: Users who commented using keywords grouped in this topic are likely expressing disatisfaction with their current showmax app, app updates that make using the app difficult, and poor copatibity with television sets.


**Other General Themes and Insights**

* slow: About 239 users had a challenge with the app's response time
* great: About 398 users had great experience using the showmax app
* download: About 104 mentioned download in relation to showmax app, sugesting having trouble downloading the app


8. In terms of **segmenting user types by Sentiment**:

* There are about **2,399** Happy Showmax users
* There are about **8,589** Sad Showmax users
* There are about  **1,021** Neutral Showmax Users - Neither happy or sad, expressing both positive and negative sentiment.

9. In terms of **segmenting user types by Review Scores**:

Happy Showmax Users segmentation:

* 4-Star Happy Showmax app users: 338 users
* 5-Star HappyShowmax app users: 2,061 users

Sad Showmax Users Segmentation:

* 1-Star Sad Showmax app users: 7,452 users
* 2-Star Sad Showmax app users: 731 users
* 3-Star Sad Showmax app users: 406 users

10. In terms of **segmenting Shoxmax app users by dominant features/topic**:
* Showmax users segmented by  **Streaming Experience & Content Variety** topic: 7,528 users
* Showmax users segmented by **Device Compatibility Issues** topic: 1,316 users
* Showmax users segmented by **App Peformance & Quality Issues** topic: 1,174 users
* Showmax users segmented by **App Version & Usability** topic: 1,034 users
* Showmax users segmented by **User Experience** topic: 957 users


# Data-Driven Recommendations for Showmax

The key recommendations Showmax can adopt based on the data-influenced insights include:


1. **Focus on Performance and Stability with Every App Update**

* **Data Insight:** Showmax version 4.12.21 had the highest number of reviews (3,633), while version 5.9.32 had only 7. Version 5.9.33 received the highest average score of 3.5, with 182 reviews. In contrast, version 4.12.21 had an average score of 1.9. The volume of negative reviews around performance and functionality issues in the early version indicates that stability and performance improvements are key.

* **Recommendation:** Focus on replicating the elements that made version 5.9.33 more successful, potentially applying these to future versions to increase positive feedback. Conduct more rigorous testing before rolling out updates, especially to avoid disrupting features users find essential.

* **Actionable Suggestion:** Analyze the development changes made in version 5.9.33 versus other versions, prioritize similar updates, and incorporate enhancements into future releases. For upcoming updates, release beta versions for a small group of users to test performance and stability before rolling out the update to all users.


2. **Improving User Interface (UI) and User Experience (UX)**

* **Data Insight:** Topic 0 highlighted the importance of the app’s experience, new interface, and streaming experience, with 1,036 mentions of “new” and 793 mentions of “watching.” Users expressed mixed feelings, with some preferring the old version of the app.

* **Recommendation:** Create a more customer-centric UI/UX by balancing the needs of users who prefer the old interface with those who appreciate the new interface to appeal to a broader user base.

* **Actionable Suggestion:** Roll out a survey or a feedback prompt within the app to gather specific feedback on desired UI/UX elements. Implement a “classic mode” alongside the updated interface, allowing users to switch between views based on preference.

3. **Invest in Improving Content Access and Streaming Experience**

* **Data Insight:** A large group of users (7,528) focuses on the streaming experience and content variety, indicating that this is a core value for Showmax subscribers. Content themes had high engagement (e.g., “app” had 1,296 mentions and “watch” had 1,700+ mentions). The quality of Showmax's content library is important for Showmax customers.

* **Recommendation:** Prioritize content variety and accessibility updates, ensuring high-quality streaming for both new and existing content.

* **Actionable Suggestion:** Regularly update and promote new shows based on popularity and audience engagement, consider adding filters for easy content discovery, and optimize personalized recommendations based on watching history.

4. **Optimize Device Compatibility and App Performance Issues**

* **Data Insight:** 1,316 users mentioned device compatibility, and 1,174 mentioned app performance issues as prominent concerns.

* **Recommendation:** Address app integration issues, particularly for TV and other devices, to provide a more consistent streaming experience.

* **Actionable Suggestion:** Perform compatibility testing on a wide range of devices, including popular smart TVs, and release specific updates for improved performance on these platforms. Consider adding a **“Help & Support”** guide specifically for TV connectivity and streaming setup within the app to help users troubleshoot.

5. **Provide Transparency and Clear Communication Around App Updates**

* **Data Insight:** Reviews indicated that many users were dissatisfied with app updates, particularly when they impacted user experience or functionality. Version 4.12.21 received a high number of reviews, but the feedback indicated dissatisfaction with the updates.

* **Recommendation:** Be transparent with users about what to expect from updates, explaining changes and improvements in detail to avoid confusion or frustration.

* **Actionable Suggestion:** Before releasing major updates, provide users with detailed release notes or a short video highlighting the changes and improvements, addressing common pain points (e.g., improved login, and enhanced performance).

6. **Leverage Happy Users for Brand Advocacy**

* **Data Insight:** There are around 2,399 Happy Showmax users, of which 2,061 gave 5-star ratings. These users are likely to advocate for Showmax if engaged appropriately.

* **Recommendation:** Engage satisfied users by encouraging them to share positive experiences on social media and tag Showmax, which may offset negative reviews.

* **Actionable Suggestion:** Create a referral program or incentives for users to leave reviews and share their Showmax experience on social media, amplifying positive sentiments. Rewards can be discounts on monthly subscriptions or free subscription periods.








