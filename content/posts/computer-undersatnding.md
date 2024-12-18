---
title: "Computer Understanding??"
date: Dec 09, 2024
draft: false
summary: Learning computer's approch to making sense of the world. Basics of Rule Based and Learning Based Systems with primary idea about Algorithms and Models. 

---
# Introduction

Before trying to check if computers are capable of perceiving the world at a human level, I wanted to learn about the current and developing mechanism (or methodology) that is helping these machines to become human-like.

Here is the first of the many posts about the deconstruction of these methods.

## What is “Computer Understanding"?

When we say understanding in general, we mean the capability of someone to interpret, reason, and derive meaning from context. Applying the same to computer understanding would mean - a machine’s ability to analyze, comprehend, and infer from data (context for us, data for them).

## Why do Computers need to Understand?

Simple answer - for AI.  
The definition of AI is mimicking human behavior. It's a field that aims to create machines that can replicate humans in both thought and movement.

Artificial Intelligence makes life easier for the simple reason that it does the things that we do (at least the part of it we don't want to do). And to complete those tasks, it needs to make sense of the world we live in.

In basic words, a machine is like the new kid in your class. To be a part of your class, they have to observe and adapt to the existing routines your class has. They have to “understand and learn” before they become a working part of it.

## How do Computers Understand?

What makes a man perfect? Plain response - *practice makes man perfect*. So then what makes a machine perfectly human? The answer is simple: *through practice*. This practice is what everyone calls *Training*.

Now how exactly does this training happen? By two ways:
1. Rule-Based Systems
2. Learning-Based Systems

---

### Rule-Based System

#### How does Rule-Based Training work?

A specific set of rules is predefined by someone for the machine to learn from. The machine considers the posed request (or query) against this list of rules and performs the action as mentioned in the matching case.

#### What are these Rules?

The rules are mostly in the form of *"if-then statements"*, i.e., *"If so-and-so-situation then perform such-and-such-action"*.

These rules are defined in such a way that every possible scenario within the domain has been considered and has a very *Explicit Rule* associated with it. This means the person writing these rules is a domain expert who knows what they are doing.

---

### Learning-Based System

#### How does Learning-Based Systems work?

Learning-based systems work by leveraging Machine Learning techniques.  

A Machine Learning Model that has learned from data makes predictions of what could be the possible answer to the posed request (or query). There is no explicit rule mentioning actions; rather, there is a relation between variables.

#### Types of Learning

There are different types of learning based on how the data is provided and what is the task that needs to be completed. These types are:
- Supervised Learning
- Unsupervised Learning
- Semi-Supervised Learning
- Reinforcement Learning  

These have been discussed in detail [here](/posts/learning-types).

---

### What is Machine Learning?

Machine Learning is a mechanism through which machines learn patterns and make inferences (for data). There are no explicit rules; rather, there are pointers and formulas that help machines identify the pattern.  

A Machine Learning Model is created using the learned patterns that use its knowledge to predict the answer.

#### What is a Machine Learning Model?

**A model identifies trends and makes a relation between defining variables and predicting variables using modifiable parameters.**

In simple words, it is like an equation maker that interprets how different input factors influence the outcome factors.

A simple example being the line equation *y = mx + c*. Considering the line equation on the above definition:
- **Defining variable** is *x*
- **Predicting variable** is *y*
- **Modifiable parameters** are *m* and *c*

#### How to make a Model?

Technically, a model is made by passing *Data* through *Algorithm*. The internal working of a model is a black box, but a basic idea of what happens is presented here.

The model identifies patterns from the data using algorithms. It then forms a formula (or at least an expression) for the relation between the elements. This helps it make predictions when given unseen (but bounded—we will see about zero-shot learning later) queries.

#### What is an Algorithm?

An algorithm is the method to learn from data. It is a general outline (relation) based on the type of pattern that needs to be identified. The parameters of the relation are defined and revised based on the algorithm logic.

More about this is discussed here. [Link to Another Post](/posts/another-post/)

---

## Comparing the Two Systems

Extending the new kid example from above, we can understand the two systems better:

- The class monitor makes a list of do’s and don'ts and gives it to the new kid. Every time they have to interact with someone, they go back to the list and see what action they have to perform. This is a **Rule-Based System**.
- The kid mingles around, observes the other kids in the class, and makes inferences from their behavior. Now, when they have to interact with someone, they use their own knowledge and take appropriate action. This is a **Learning-Based System**.

There could be situations where Rule based would be better than Learning based. When there needs to be a perfect action such as greeting the teacher with their name, then the first option ensures that the names are not mixed up, because the actions are fixed.

There also are situations where Learning based is better than Rule based. When there is a need to face a new situation that neither they nor their classmates have encountered, such as a guest arriving at their class. Now an appropriate greeting has to be done based on how they have greeted the others until now.  


#### Situational Comparisons

- **Rule-Based Advantages**:
  - Deterministic actions for every situation.
  - Very easy to follow and trace back.
- **Rule-Based Disadvantages**:
  - Cannot handle situations outside the predefined scenario-action set.
  - Requires human expertise and intervention for modification of logic or data.

- **Learning-Based Advantages**:
  - Automation, no need for human expertise and intervention for modification of logic or data.
  - Scalable to huge amounts of data.
- **Learning-Based Disadvantages**:
  - Requires a good amount of data and computational power to work well.
  - Patterns are not easily human-interpretable and traceable.

By weighing the advantages and disadvantages, we can understand that learning-based systems are better suited for today's needs.

---

## Conclusion

The entire blog can be summarized in these two sentences:  
1. Machine understanding is a goal for achieving Artificial Intelligence-equipped computers.  
2. Machine understanding happens through Machine Learning.


