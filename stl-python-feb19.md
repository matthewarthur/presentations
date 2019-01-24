# Python Lessons I Learned (the Hard Way)

## Name: Matt Arthur
### Current Role: Compliance & Security Engineering, DataStax Cloud 
### 5 Feb 2019 -- STL Python Meetup

# Agenda

* My Background (Python & Professional)
* Things I Learned Slowly & Out-of-Order (Presented In Order)
  * Environment Management (Pipenv, Anaconda & Virtualenv)
  * IDE Use (PyCharm, VS Code, N++)
  * Jupyter Notebooks! 
  * How to Read Errors
	* And how to ask questions about these errors
  * Git! GitHub! GitLab! BitBucket! etc.
  * The Easy Dumb Way vs the Elegant Way: Same Outcome
  * Iterate! Crawl, Walk, Run

* Things I Need to Learn
  * Jenkins
  * Docker
  * Packer


## How I got Here

### Education
* Carleton College - History BA (2004)
* UIUC -- Applied Mathematics (2018)

### Work History
* SIGINT Analyst / Arabic Linguist @ NSA 
* Data Privacy @ Corning
* Cloud Security Architect @ Monsanto
* Compliance & Security Automation @ DataStax

### Python History
* Data Normalization (Geospatial)
* Machine Learning & Deep Learning
* Lambda Lambda Lambda

## 1 Environments
* Why do I care about this? 
  * Package & version conflicts! Here are common ones:
    ** OpenCV2 vs ..3
    ** PyTorch / TensorFlow / Keras / anything CUDA
    ** Mail (Py2 vs Py3)
    ** Fast.ai 0.7 vs 1.0
    ** Everything! 
* What's the answer?
  * Install & use a tool to segregate packages into standalone environments
* Ok. So what are common Python environment managers? 
  * I have used 3, there are probably lots:
    ** Pipenv, Virtualenv, Anaconda
* Which one is the best?
  * Conda. Also, spaces.
* Why? 

## 2 Integrated Development Environments (IDEs)
* Why can't I just script in Nano or Wordpad?
  * You can. Good luck with that.
