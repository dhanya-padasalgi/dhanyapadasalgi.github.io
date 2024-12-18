---
title: "Types of Learning"
date: 2024-12-04
draft: false
summary: Types of Learning- Supervised, Unsupervised, Semi-Supervised and Reinforcement Learning

---

# Introduction

Now that I know about Computer Understanding, I now have become familiar with Learning and its types.  
This post will discuss an overview about the Learning Types. All the algorithms that are used to achieve learning of different types is discussed in the [Algorithm Post](/posts/another-post/).

---

## What are the Learning Types?

There are 4 types of learning that happen in a machine. They are:  
1. **Supervised Learning**  
2. **Unsupervised Learning**  
3. **Semi-Supervised Learning**  
4. **Reinforcement Learning**  

Each of them is chosen based on the type of data (structured or unstructured) and the task (classification, clustering, etc.). They have unique requirements and implementations.  

I will try to describe each of these learning techniques using a real-life comparison to organizing my closet.

---

## Supervised Learning

### What is Supervised Learning?
By definition, Supervised Learning is:  
**"Learning with labeled data where the model learns to map inputs to outputs based on given examples."**

It uses **structured data** (also called labeled data) to learn the pattern or relationship between the features and outputs.  
It is one of the most used and preferred learning types as it makes it easy for machines to learn, and the output is predictable.

### Analogy
When I am trying to organize my closet, my mom has already labeled all my clothes as “Shirts,” “Skirts,” “Pants,” etc. So I just place all of them in different sections. Now, when I buy a new item, I will find a label that best suits this new item and add it into that section.

### When is Supervised Learning used?

Supervised Learning requires **structured data** to train.  
These are the tasks that require Supervised Learning:  
- **Classification**: Assigning labels to data.  
  _Example_: Spam and no-spam classification for email.  
- **Regression**: Predicting continuous values.  
  _Example_: Predicting house prices based on features like size and location.  
- **Time Series Forecasting**: Predicting future values based on historical data.  
  _Example_: Stock price forecasting.  

---

## Unsupervised Learning

### What is Unsupervised Learning?
By definition, Unsupervised Learning is:  
**"Learning from unlabeled data to discover hidden patterns or structures."**

It uses **unstructured data** (also known as unlabeled data) and tries to group this data based on observed patterns or logic.

### Analogy
When arranging clothes in my closet, I have no idea what each item of clothing is. I will try and pile the clothes into different groups based on parameters like length, color, fabric, etc. Now, when I get a new piece of clothing, I will try to add it to the group that it is most similar to.

### When is Unsupervised Learning used?

Unsupervised Learning runs on **unstructured data**.  
These are the tasks that require Unsupervised Learning:  
- **Clustering**: Grouping similar data points together.  
  _Example_: Customer segmentation in marketing.  
- **Dimensionality Reduction**: Reducing the number of features while preserving essential information.  
  _Example_: Principal Component Analysis (PCA) for visualizing high-dimensional data.  
- **Anomaly Detection**: Identifying outliers or unusual patterns.  
  _Example_: Detecting fraudulent transactions.  

---

## Semi-Supervised Learning

### What is Semi-Supervised Learning?
By definition, Semi-Supervised Learning is:  
**"A hybrid approach that uses a small amount of labeled data along with a larger amount of unlabeled data."**

It uses a combination of **structured and unstructured data** to infer patterns.

### Analogy
My closet would have a few labeled items—e.g., “Shirt,” “Pant”—but most of it is unlabeled. I use the labeled items as a guide and figure out the categories for the rest based on similarity to the labeled examples. Now, when I buy a new item, I will try to associate it with the category closest to it and try to label it as well.

### When is Semi-Supervised Learning used?

These are the tasks that require Semi-Supervised Learning:  
- **Classification with Limited Labels**: Improving classification accuracy by leveraging unlabeled data.  
  _Example_: Recognizing handwritten digits with a few labeled samples.  
- **Data Label Propagation**: Assigning labels to unlabeled data using patterns derived from labeled data.  
  _Example_: Labeling parts of a medical image for diagnosis.  

---

## Reinforcement Learning

### What is Reinforcement Learning?
By definition, Reinforcement Learning is:  
**"Learning through trial and error by interacting with an environment to maximize cumulative rewards."**

In this type, learning happens through interaction and feedback to maximize rewards. The data is labeled based on the response received.

### Analogy
When organizing the closet, my mom is standing behind me. Every time I arrange an item right, she appreciates me, and every time it is not, she either does not react or scolds me. This makes a clear pattern of when I’m being rewarded and penalized. Now, when I buy a new item, I will choose my action based on my inference from the pattern.

### When is Reinforcement Learning used?

These are the tasks that require Reinforcement Learning:  
- **Game Playing**: Teaching AI to play games like chess or Go.  
  _Example_: AlphaGo defeating human champions.  
- **Robotics**: Teaching robots to perform tasks like walking or grasping objects.  
  _Example_: A robot learning to navigate through a warehouse.  
- **Control Systems**: Optimizing processes or systems over time.  
  _Example_: Self-driving cars learning to adjust speed and steering based on surroundings.  
- **Personalization**: Recommending content or adjusting strategies dynamically.  
  _Example_: Online recommendation systems adapting to user preferences.  

---

## How do the Learning Types differ from each other?

| **Feature**           | **Supervised Learning**         | **Unsupervised Learning**         | **Semi-Supervised Learning**         | **Reinforcement Learning**         |
|------------------------|----------------------------------|------------------------------------|---------------------------------------|-------------------------------------|
| **Input Data**         | Labeled data (input-output pairs). | Unlabeled data.                   | Mix of labeled and unlabeled data.   | Interaction with an environment.   |
| **Goal**               | Predict outputs.               | Discover hidden patterns.          | Improve accuracy.                   | Maximize rewards.                  |
| **Tasks**              | Classification, regression, time series forecasting. | Clustering, anomaly detection, dimensionality reduction. | Classification with limited labels, data labeling propagation. | Game playing, robotics, self-driving cars, personalized recommendations. |
| **Nature of Feedback** | Direct and explicit (labeled outputs). | No feedback; patterns are inferred. | Feedback for labeled data; inferred guidance for unlabeled data. | Feedback via rewards or penalties. |
