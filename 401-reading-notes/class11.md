# What is Jupyter Lab
JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner. For a demonstration of JupyterLab and its features, you can view this video:
[video](https://youtu.be/A5YyoCKxEOU)

You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing, for example:

Code Consoles provide transient scratchpads for running code interactively, with full support for rich output. A code console can be linked to a notebook kernel as a computation log from the notebook, for example.

Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.

Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. For example, it is easy to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.

# Numpy Tutorial

NumPy is a commonly used Python data analysis package. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood.


Creating A NumPy Array
- We can create a NumPy array using the numpy.array function. 

![](https://miro.medium.com/max/604/1*VtiuhTuylfr8kU-D6QAMBg.png)

Using NumPy To Read In Files
- It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function. 

`wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)`

Indexing NumPy Arrays

wines[2,3]

Slicing NumPy Arrays
- wines[0:3,3]

Assigning Values To NumPy Arrays
- wines[1,5] = 10

Notes taken from (https://www.dataquest.io/blog/numpy-tutorial-python/)
