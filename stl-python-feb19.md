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
  * Package & version conflicts! Here are ones I've experienced:
    * OpenCV2 vs ..3
    * PyTorch / TensorFlow / Keras / anything CUDA
    * Mail (Py2 vs Py3)
    * Fast.ai 0.7 vs 1.0
    * Everything! 
* What's the answer?
  * Install & use a tool to segregate packages into standalone environments
    * Get the packages set for a particular dev case and don't muck with it!
* Ok. So what are common Python environment managers? 
  * I have used 3, there are sure more:
    * Pipenv, Virtualenv, Anaconda
* Which one is the best?
  * Conda, for me. Also, spaces not tabs.
  * YMMV, just use one
* Why do I like Conda? 
  * (Mostly) combines functionality of Pip & Virtualenv
  * Heavily used in data science community
  * Not limited to Python

## 2 Integrated Development Environments (IDEs)
* Why can't I just script in Nano or Wordpad?
  * You can. Good luck with that. I used N++ on a Windows box for a decade
* Why do you use an IDE?
  * Usual reasons. Match ()s, indent, tab completion, troubleshooting, etc
* What IDEs?
  * I use VS Code (now), Atom seems fine, there are lots!
  
## 3 Jupyter Notebooks!
* What?
  * https://jupyter.org/
  * Open-source browser-based app to work with 40+ languages
  * Keep eyes open for .ipynb
  * Huge in data science
