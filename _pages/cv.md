---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
------

* **MSc. in Computational linguistics** \| 2018-2020 (expected) \| LMU, Germany
  * Project to determine the semantic similarity between two documents from an input of 1.3k docs on a corpus of 58k words. Generation of semantic features of all docs in 32s, comparison of documents in 5s.
  * Implementation of an (in-)sincere question classifier with pre-trained embeddings on a BiLSTM model with Attention on a 1.3M question input with 94%-6% imbalance. F1-score of 0.66. ([~/kaggle](https://github.com/anebz/kaggle))
  * Semester-long group project on transport recommendation given an origin and destination coordinate points. Development of geodata preprocessing and ensemble models yielding an F1-score of 0.68. ([~/kdd-cup-2019](https://github.com/AlessandroVol23/kdd-cup-2019))
  * Exploration of semantic similarities between contextualized embeddings in English and Basque. ([~/eu-sim](https://github.com/anebz/eu-sim))

* **BSc. in Telecommunication Systems Engineering** \| 2013-2017 \| Tecnun - Universidad de Navarra, Spain
  * Project to determine the highest-scoring combination of letters in a Boggle board that yields a given hash. An error of one letter is allowed and the algorithm runs in under 0.1s. ([~/boggle](https://github.com/julencestero/boggle))
  * Bachelor thesis: implementation of a traceability processing algorithm with high recursivity in 8MB input csv files producing ~900MB files. Programmed in Scala to use RDDs and run in an AWS EMR.

Work experience
------

* **Student job: NLP** \| 2019/05 - Present \| Siemens, Germany
  * Implementation of a NER algorithm to extract company names from PDFs using XML scrapping and NLP libraries.
* **Student job: deep learning** \| 2018/12 - 2019/02 \| Terraloupe, Germany
  * Testing of semantic segmentation models with different preprocessing on gcloud.
* **Data scientist** \| 2018 Summer \| Skootik, Spain
  * Implementation of a multiclass image classifier from scratch focused on high class imbalance and a small dataset.
  * Image processing with cv2, CNN on Keras and F1-score of 0.7 on 5 classes across 4k images.
* **Research assistant** \| 2017/07 - 2018/07 \| Fraunhofer IIS, Germany
  * Development, optimization and testing of a psychoacoustic model for the MPEG-H 3D Audio encoder.
  * Publication of *"Improved psychoacoustic model for efficient perceptual audio codecs"* in AES New York 2018.

Projects
------

* 2019 \| **Cracking the coding interview**
  * Learning data structures and algorithms through the book and publication of notes and solutions ([~/ctci](https://github.com/anebz/ctci))
* 2019 \| **NLP papers**
  * Reading current NLP papers and publication of notes and references ([~/papers](https://github.com/anebz/papers))
* 2019 \| **Gendered pronoun resolution**
  * Implementation of a coreference resolution algorithm with pre-trained embeddings on a Multi-CNN/BERT model on a 4k input text from the Google GAP dataset.
* 2017 \| **Huffman compressor**
  * Developed the lossless Huffman compression algorithm to compress text files.

Professional development
------

* 2018 \| *Deep learning specialization* \| Coursera, deeplearning.ai
  * DL algorithm design, implementation, optimization. Python, TensorFlow, Keras, CNNs, NLP.
* 2017 \| *Machine learning online course* \| Coursera, Stanford University
  * Regression, gradient descent, regularization, neural networks, SVMs, recommender systems.
* 2017 \| *Smart cities online course* \| edX, ETH Zürich
  * Smart cities, information architecture, big data, citizen-design science, complexity science, liveability.

Skills
------

* Software
  * Matlab, C/C++, Java, bash, Scala, Spark
  * Basic web development: HTML, CSS, JavaScript, PHP, mySQL
* Data science
  * SQL, Python, numpy, pandas, scikit-learn, openCV, nltk
  * TensorFlow, Keras
  * Basic Docker, Google Cloud
* Version control
  * git, svn
* Writing
  * Office, LaTeX, Markdown
* Natural languages
  * *Fluent*: Basque, Spanish, English
  * *Advanced*: German
  * *Intermediate*: Italian

Publications
------

  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
<!---
Talks
------
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
------
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
------
* Currently signed in to 43 different slack teams

-->