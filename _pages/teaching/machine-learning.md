---
layout: page
title: Machine Learning
permalink: /teaching/machine-learning/
description: Course materials for Machine Learning
course_id: ml
nav: false

lectures:
  - title: "Introduction to Machine Learning"
    description: "Types of learning, supervised vs unsupervised learning, model evaluation"
    slides: "/assets/teaching/ml/lecture1_slides.pdf"
    video: "https://example.com/ml_lecture1"
    notes: "/assets/teaching/ml/lecture1_notes.pdf"
  
  - title: "Linear Regression and Gradient Descent"
    description: "Linear models, cost functions, gradient descent optimization"
    slides: "/assets/teaching/ml/lecture2_slides.pdf"
    video: "https://example.com/ml_lecture2"
  
  - title: "Classification: Logistic Regression and SVM"
    description: "Binary and multiclass classification, support vector machines"
    slides: "/assets/teaching/ml/lecture3_slides.pdf"
    notes: "/assets/teaching/ml/lecture3_notes.pdf"

assignments:
  - title: "Assignment 1: Linear Regression"
    description: "Implement linear regression from scratch and analyze performance"
    pdf: "/assets/teaching/ml/assignment1.pdf"
    solution: "/assets/teaching/ml/assignment1_solution.pdf"
    due_date: "October 15, 2024"
  
  - title: "Assignment 2: Classification"
    description: "Compare logistic regression and SVM on real datasets"
    pdf: "/assets/teaching/ml/assignment2.pdf"
    due_date: "November 1, 2024"
  
  - title: "Final Project"
    description: "End-to-end machine learning project with your choice of dataset"
    pdf: "/assets/teaching/ml/project_guidelines.pdf"
    due_date: "December 15, 2024"

resources:
  - title: "Pattern Recognition and Machine Learning"
    description: "Christopher Bishop - Comprehensive ML textbook"
    url: "https://example.com/bishop_book"
  
  - title: "scikit-learn Documentation"
    description: "Python machine learning library with examples and tutorials"
    url: "https://scikit-learn.org/stable/"
  
  - title: "Coursera ML Course"
    description: "Andrew Ng's Machine Learning course for additional reference"
    url: "https://www.coursera.org/learn/machine-learning"
---

{% include course-materials.liquid %}
