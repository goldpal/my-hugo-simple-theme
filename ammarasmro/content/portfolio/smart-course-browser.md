+++
draft = false
comments = false
slug = ""
tags = ["Recommender", "Flask", "Python", "Watson", "TradeOff Analytics", "Apache-Solr", "Word2Vec", "Word embeddings"]
categories = ["Machine Learning"]

showpagemeta = true
showcomments = true
date = 2018-05-21T21:01:27-06:00

title = "Smart Course Browser"
description = "A search engine powered by two recommendation systems to help students find courses"
externalUrl = ""
image = "img/portfolio/smart-course-browser/TA3.png"
+++
Abstract—Choosing a course at the university is a challenge to students that is overlooked by the system. The student to advisor ratio is big and the student needs to spend months researching a course without finding sufficient data. With so few resources, the student is left with the few lines of description from the course website and the word of mouth, which have such a big risk. Education shouldn’t be relying on risky actions. In this project, I address this issue and suggest a platform that can help in fixing it. I propose a recommender system that uses the new techniques that are used in different fields and applies them to education. The final product is a complete platform with a search engine, recommender algorithms, and a decision-making tool. The value in the methods presented here is that, unlike other educational recommendation systems, it tries to help the student decide with a step-by-step approach rather than doing all the prediction automatically.

#### Data Collection
The data used for this project was obtained from the Software Product Management Specialization Massive Open Online Course (MOOC) that is hosted on Coursera. Data include personal data, such as grade books, ratings, performance, and assessment. This tabular data comes in Comma Delimited Value (CSV) files. The data also included notes and transcripts from the lectures. User names were anonymized by Coursera to protect the privacy of the students. So each user has a specific encrypted user ID. Those user ID’s are not consistent across the sections, for example, students’ performance cannot be linked to their feedback. Five courses are required, plus a capstone project, to finish the specialization. Table I shows the names of the courses that were used for this project.

| Courses |
| --- |
| Introduction to Software Product Management |
| Software Processes and Agile Practices |
| Client Needs and Software Requirements |
| Agile Planning for Software Products |
| Reviews & Metrics for Software Improvements|

#### Main parts
* **Apache Solr**
* **Word2vec**
* **Recommender Systems**
  * Item-Similarity
  * Matrix Factorization
* **IBM Watson**
  * TradeOff Analytics API

#### Dependencies
* ***SQLAlchemy***
* ***Pandas***
* ***Scikit-Learn***
* ***Gensim***
* ***NLTK***
* ***SparseSVD***

#### The system
{{< figure src="/img/portfolio/smart-course-browser/system.jpg" width="60%" >}}

#### Results

##### Sample results of the Word2Vec model

agile  |  manager
--- | ---
methodologies  | owner
principles | leader
Agile | delivering
methods | decision
Lean | seagull
practices | vision
methodology | evolves
Scrum | evolving
lean | managers
linear | responsibility

*Word embeddings*
{{< figure src="/img/portfolio/smart-course-browser/nesave.png" width="60%" >}}
{{< figure src="/img/portfolio/smart-course-browser/nepartsave.png" width="60%" >}}


##### TradeOff Analytics
{{< figure src="/img/portfolio/smart-course-browser/TA1.png" width="60%" >}}
{{< figure src="/img/portfolio/smart-course-browser/TA2.png" width="60%" >}}

#### Our UI
{{< figure src="/img/portfolio/smart-course-browser/ui.png" width="60%" >}}
