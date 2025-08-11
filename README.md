
# Project: AI-Powered Customer Query Assistant

## Objective
Parts Avatar wants to enhance our customer support and on-site search experience using Generative AI. We want to better understand customer feedback from reviews and help customers find the right products even when they don't know the exact part name.

Your goal is to build a prototype of an AI assistant with two core capabilities: sentiment analysis and semantic product search.

## The Challenge
This project requires you to think conceptually about how to solve nuanced language problems. How do you handle a review that is both positive and negative? How do you match a vague user query to a specific product? Your choice of models, prompts, and overall strategy is more important than the complexity of the code.

## Datasets
* `data/customer_reviews.csv`: A sample of customer reviews for various products.
* `data/product_catalog.csv`: A list of products we sell.

## Your Tasks

### Part 1: Automated Sentiment Analysis
1.  **Design a Sentiment Schema:**
    * Go beyond a simple `positive/negative/neutral` classification. Design a more nuanced schema. For example, you could identify both an overall sentiment and topic-specific sentiments (e.g., `{"overall_sentiment": "mixed", "topics": {"product_quality": "positive", "shipping_experience": "negative"}}`).
2.  **Implement the Analysis:**
    * Write a Python script that takes a review and outputs its sentiment according to your schema. You can use a pre-trained model from Hugging Face, an LLM API (like OpenAI's), or any other modern NLP technique. Justify your choice.
3.  **Process the Sample Data:**
    * Run your script on the `customer_reviews.csv` and output the results.

### Part 2: Semantic Product Search
1.  **Develop a Matching Strategy:**
    * Design a system to find the best-matching products from our `product_catalog.csv` given a natural language query from a customer (e.g., "I need brake pads for a 2019 Toyota Camry that are quiet and long-lasting").
    * **Hint:** A good approach would involve creating embeddings for the product descriptions and the user query, then using vector similarity to find the closest matches.
2.  **Implement the Search Function:**
    * Write a Python function that takes a user query as input and returns the top 3 most relevant SKUs from the catalog.

### Documentation
* Update this `README.md` to be a comprehensive report of your project.
* **Crucially, explain your design choices:**
    * Describe your sentiment analysis schema and why you chose it.
    * Justify your choice of model/API for sentiment analysis.
    * Explain your semantic search strategy, including your choice of embedding model.
* Provide clear instructions on how to set up and run your code for both tasks.
* Discuss the limitations of your prototype and how you would improve it in a production environment.

## Evaluation Criteria
* **Conceptual Design & Problem-Solving:** The thoughtfulness of your sentiment schema and semantic search strategy.
* **Proficiency with Gen AI Tools:** Your choice and implementation of modern NLP models/frameworks.
* **Clarity of Explanation:** How well you justify your design decisions and explain the system's capabilities and limitations in the README.
* **Code Quality:** The clarity and organization of your implementation.
