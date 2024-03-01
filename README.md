# Computational-Linguistics-over-Reddit-Data
Part I: Data Acquisition and Loading
Objective: The initial phase of the project was dedicated to acquiring and structuring data from selected subreddits, focusing on areas of personal interest to ensure engagement and relevance throughout the analysis. The goal was to design and implement a database capable of efficiently storing, updating, and querying Reddit posts and their associated metadata for in-depth analysis and information retrieval (IR).

Database Design and Implementation:

A PostgreSQL schema was conceptualized to accommodate the diverse range of data associated with Reddit posts. Key attributes such as title, link, author, subreddit, tag/flair, timestamp, and the post's body text were identified as essential for capturing the full context and facilitating effective IR.
To ensure data integrity and uniqueness, constraints were imposed to prevent the duplication of posts.
Triggers were created to automate the updating of IR-related fields, ensuring that the database remains current with minimal manual intervention.
Indexing strategies, specifically using GIN (Generalized Inverted Index) or GiST (Generalized Search Tree), were applied to the IR fields to enhance search capabilities and performance.
A sentiment field was introduced to store sentiment analysis results, providing a foundational metric for subsequent analytical and linguistic exploration.
Data Collection and Processing:

Python scripts were developed to interface with the Reddit API, collecting the latest posts from chosen subreddits. The scripts were designed to fetch a minimum of 500 posts from each subreddit, focusing on text-dominant content to align with the project's IR and sentiment analysis objectives.
Extracted data underwent preprocessing to separate metadata from post content, alongside the implementation of computational linguistics techniques to derive sentiment scores from the post text.
Expansion and Scalability:

Following the initial data acquisition from a single subreddit, the project scaled to include additional subreddits. This not only enriched the dataset but also broadened the scope for comparative analysis across different communities and topics.
Part II: Analytics
Data Exploration and Analysis:

Utilizing the PostgreSQL database and Python for analysis, test queries were executed to explore text vectors, leveraging the indexes created for efficient IR.
Sentiment analysis was performed on the collected posts, providing insights into the general mood and tone across different subreddits.
Visualization and Findings:

The project featured a range of visualizations, including trend analysis within individual subreddits and comparative views across different communities. These visualizations highlighted linguistic patterns, sentiment fluctuations, and topic variations, offering a nuanced understanding of discourse dynamics on Reddit.
Comparative plots revealed interesting insights into how different subreddits engage with various topics, along with sentiment trends that may correlate with specific events, topics, or community behaviors.
Conclusion and Insights:

The comprehensive approach to data acquisition, coupled with detailed analytics and sentiment analysis, unveiled the complex interplay of topics, engagement, and emotional tones across Reddit. The project not only demonstrated the technical feasibility of real-time data acquisition and analysis but also provided a framework for understanding online communities through the lens of computational linguistics and sentiment analysis.
Key insights included the identification of sentiment trends tied to specific topics or events, variations in engagement and discussion themes across subreddits, and the potential for using sentiment analysis as a predictor for community behavior or interest shifts.
