+++
draft = false
comments = false
slug = ""
tags = ["NLU", "Java", "Neo4j", "Graph", "Watson", "Chatbot", "IR", "IE"]
categories = ["Machine Learning", "School"]

showpagemeta = true
showcomments = true
date = 2018-05-21T21:13:38-06:00

title = "Personalized Knowledge Graphs"
description = "A progressive graph builder to power a chatbot"
externalUrl = "https://github.com/ammarasmro/personalized-knowledge-graphs"
image = "/img/portfolio/personalized-knowledge-graphs/schema.png"
+++

A personal assistant that helps with projects

This project started as an idea last summer, I started researching and experimenting around. I have decided to work on it during the last term of my Master of Engineering program as my capstone project.

The biggest inspiration for me was Jarvis from Iron Man, I always wanted to have a Jarvis that can help me with building projects, keep track of the steps, and help me find information.

{{< figure src="/img/portfolio/personalized-knowledge-graphs/schema.png" width="60%" >}}

## Main parts
* **Discovery Client:** This client communicates with the discovery service provided by IBM Watson. It gets a JSON response which contains text, keywords, concepts, etc. Those are sent into the DiscoveryDocument class for parsing.
* **OpenIE Client:** Stanford CoreNLP provides Open Information Extraction. Basically this takes sentences and turns them into subject -- verb --> object triplets.
* **Coref Client:** Stanford CoreNLP also provides Coreference Resolution. This is useful to detect multiple mentions of the same subject. In our case, I'm also using it as a story telling part, since it can separate the same sentence on multiple points and give the depending verb that links the two sentences. This will be useful to create more triplets and also to check the previous triplets.
* **Database:** Neo4j is going to be used to store the information for the projects. This is a very tricky part of the project and will take time to finish.
* **Actions on Google:** (Out of current scope) This will be the last step of the project. By following the procedure on the Actions Console I will submit my chatbot to the Google Assistant team for review and hopefully it will be available for public use.

<!-- [1]: /img/portfolio/personalized-knowledge-graphs/schema.png -->
