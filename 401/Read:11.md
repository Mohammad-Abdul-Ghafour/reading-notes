# Data Analysis
## JupyterLab :
**`JupyterLab`** is a web-based interactive development environment for **`Jupyter`** *`notebooks`*, *`code`*, and *`data`*.

**`JupyterLab`** provides a unified architecture for viewing and editing data in a wide variety of formats. This model applies whether the data is in a file or is provided by a kernel as rich cell output in a notebook or code console.

### Text Editor, Code Consoles and Terminals : 
The **`text editor`** in JupyterLab enables you to edit text files in JupyterLab, includes syntax highlighting, configurable indentation.

![Text Editor](https://jupyterlab.readthedocs.io/en/stable/_images/file_editor_overview.png)

**`Code consoles`** enable you to run code interactively in a kernel. The cells of a code console show the order in which code was executed in the kernel, as opposed to the explicit ordering of cells in a notebook document. Code consoles also display rich output, just like notebook cells.

![Code consoles](https://i.stack.imgur.com/G48uW.png)

JupyterLab **`terminals`** provide full support for system shells (bash, tsch, etc.) on Mac/Linux and PowerShell on Windows. You can run anything in your system shell with a terminal, including programs such as vim or emacs. The terminals run on the system where the Jupyter server is running, with the privileges of your user. Thus, if JupyterLab is installed on your local machine, the JupyterLab terminals will run there.

![Terminals](https://jupyterlab.readthedocs.io/en/stable/_images/terminal_layout.png)

### Jupyter Notebook :
The **`Jupyter Notebook`** is an open source web application that you can use to create and share documents that contain live code, equations, visualizations, and text. Jupyter Notebook is maintained by the people at Project Jupyter.

**`Jupyter notebooks`** are documents that combine live runnable code with narrative text (Markdown), equations (LaTeX), images, interactive visualizations and other rich output:

![Jupyter Notebook](https://jupyterlab.readthedocs.io/en/stable/_images/notebook_ui.png)

## NumPy :

![NumPy](https://miro.medium.com/max/765/1*cyXCE-JcBelTyrK-58w6_Q.png)

**`NumPy`** is a general-purpose array-processing package. It provides a high-performance multidimensional array object, and tools for working with these arrays.

It is the fundamental package for scientific computing with Python. It contains various features including these important ones: 

* A powerful N-dimensional array object.
* Sophisticated (broadcasting) functions.
* Tools for integrating C/C++ and Fortran code.
* Useful linear algebra, Fourier transform, and random number capabilities.

Besides its obvious scientific uses, **`NumPy`** can also be used as an efficient multi-dimensional container of generic data. 

Arbitrary data-types can be defined using **`Numpy`** which allows **`NumPy`** to seamlessly and speedily integrate with a wide variety of databases.

**`Arrays in NumPy`** : NumPy’s main object is the homogeneous multidimensional array.
   * It is a table of elements, all of the same type, indexed by a tuple of positive integers.
   * In NumPy dimensions are called axes. The number of axes is rank.
   * NumPy’s array class is called ndarray. It is also known by the alias array.

Example : 

```
[[ 1, 2, 3],
 [ 4, 2, 5]]
Here,
rank = 2 (as it is 2-dimensional or it has 2 axes)
first dimension(axis) length = 2, second dimension has length = 3
overall shape can be expressed as: (2, 3)
```

Code :

```python
import numpy as np
 
# Creating array object
arr = np.array( [[ 1, 2, 3],
                 [ 4, 2, 5]] )
 
# Printing type of arr object
print("Array is of type: ", type(arr))
 
# Printing array dimensions (axes)
print("No. of dimensions: ", arr.ndim)
 
# Printing shape of array
print("Shape of array: ", arr.shape)
 
# Printing size (total number of elements) of array
print("Size of array: ", arr.size)
 
# Printing type of elements in array
print("Array stores elements of type: ", arr.dtype)
```

Output :

```
Array is of type:  
No. of dimensions:  2
Shape of array:  (2, 3)
Size of array:  6
Array stores elements of type:  int64
```