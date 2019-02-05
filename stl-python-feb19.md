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
  * Crawl, Walk, Run (How to code Pythonically)
  * Work With Others

* Things I Need to Learn (Python Adjacent)
  * Terraform
  * Docker
  * Packer


## How I got Here

### Education
* Carleton College - History BA (2004)
* University of Illinois Urbana-Champaign -- Applied Mathematics (2018)

### Work History
* SIGINT Analyst / Arabic Linguist @ NSA 
  * !اهلاً
* Data Privacy @ Corning
* Cloud Security @ Monsanto
* Compliance & Security Automation @ DataStax

### Python History
![My Python in a Nutshell]
(https://i.pinimg.com/originals/53/be/34/53be34c987b10821f7c10b9d88436b92.jpg)

* Data Normalization (Geospatial)
* Machine Learning / Deep Learning
* Lambda

## 1 Environments
* Why do I care about this? 
  * Package & version conflicts! Here are ones I've experienced:
    * OpenCV2 vs ..3
    * PyTorch / TensorFlow / Keras / anything CUDA
    * Mail (Py2 vs Py3)
    * Fast.ai 0.7 vs 1.0
    * Everything! 
    * Examples: https://stackoverflow.com/questions/39315156/how-to-install-xgboost-in-python-on-macos or https://stackoverflow.com/questions/44439443/can-i-pip-install-opencv2-for-python
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
  * Over 700 packages

## 2 Integrated Development Environments (IDEs)
* Why can't I just script in Nano or Wordpad?
  * You can. I used N++ on a Windows box for a decade. There are better ways.
* Why do you use an IDE?
  * Usual reasons: Match ()s & []s, indent properly, autocomplete, error tracing, etc
* What IDEs?
  * I use VS Code (now), Atom seems fine, I didn't like Pycharm
    * There are lots! 
  
## 3 Jupyter Notebooks!
* What:
  * Julia + Python + R
  * https://jupyter.org/
  * Open-source browser-based app to work with 40+ languages
  * Mixture of code, text, graphics
  * Huge in data science
* Where: 
  * Anywhere, the same:
    * Your browser, EC2 instance, IDEs, Kaggle, Docker
* Functions:
  * Multiple environments (Py2, Py3, PyTorch, TF)
  * Rich visuals (matplotlib, LaTex, plotly)
  * Bash & magic cmomands
* Examples:
  * https://nbviewer.jupyter.org/github/carljv/Will_it_Python/blob/master/ARM/ch5/arsenic_wells_switching.ipynb
  * https://nbviewer.jupyter.org/url/finiterank.com/cuadernos/suavesylocas.ipynb
    * Both from https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks

## 4 Errors
* What are they good for?
* Example: https://stackoverflow.com/questions/7818811/import-error-no-module-named-numpy
  * asked 7 years, 3 months ago
  * viewed 426,222 times
 * Read the stack trace, look at line numbers, search for the error, read the existing questions
 * Another example: 

```
/opt/conda/lib/python3.6/site-packages/torch/nn/functional.py in linear(input, weight, bias)
   1352         ret = torch.addmm(torch.jit._unwrap_optional(bias), input, weight.t())
   1353     else:
-> 1354         output = input.matmul(weight.t())
   1355         if bias is not None:
   1356             output += torch.jit._unwrap_optional(bias)

RuntimeError: Expected object of scalar type Double but got scalar type Float for argument #2 'mat2'
```
   * https://discuss.pytorch.org/search?q=Expected%20object%20of%20scalar%20type%20Double%20but%20got%20scalar%20type
 * Bad! https://stackoverflow.com/questions/54522426/i-was-training-the-lstm-network-using-pytorch-and-encountered-this-error
 * Opportunity for collaboration as well as skill development
 
 ## 5 Versioning & Repositories
 * What? 
   * A place to store, share, deploy code (while tracking changes)
 * Why?
   * So many reasons!
 * Which one?
   * Options: GitHub, GitLab, BitBucket, AWS CodeCommit, SourceForge, Gitea, Phabricator, etc.
     * Whichever your team / role model / sector uses? 
 * Best Practices!
   * https://guides.github.com/introduction/flow/
   * Ask another dev what they do

 ## 6 The Easy Dumb Way vs the Elegant Way
 * aka _The Pythonic Way_ and _The Way I Got It To Work_
   * Ex: Loops vs Lambda
     * https://www.geeksforgeeks.org/loops-in-python/
     * https://www.programiz.com/python-programming/anonymous-function
   * More seriously
     * https://www.python.org/dev/peps/pep-0008/

## 7 Collaboration
 * Domain-Specific Forums
 * StackOverflow
 * OSS Contributions
 * GH Issues
 * Other
 
## Next Items to Learn
 * Infrastructure-as-Code
   * Terraform
 * Containers
   * Docker
   * Kubernetes
 * Other
   * Spark
   * Data Viz
     * R's GGPlot to ?Plotly?
   * Regex
 
 
