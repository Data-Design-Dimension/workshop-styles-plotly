# Customizing Visual Styles in Plotly

Code for a workshop originally developed for an Unconference session during the [Outlier Conference](https://outlierconf.com/) hosted by Data Visualization Society.

To jump right in:
Fork this repository, or download the Jupyter Notebook file Styling_Plotly_Themes_Templates.ipynb.

Ever have that feeling that a lot of data viz you see screams the tool it was made in? Using the [Plotly Open Source](https://github.com/plotly/plotly.py) Python graphing library, we will take a look under the hood of:

- the style themes available, 
- understand the visual elements like figure and chart backgrounds, and 
- build our own default theme script inspired by 1980's computers. 

This informal workshop is for a seasoned Pythonista wanting to add to your design toolbox or a newbie curious about custom interfaces beyond the usual BI tools (listen or follow along).

## Quick Start Prep 
###(most of this occurs before the workshop to follow along live...)
We're not going to spend too much time here, but if you're just starting out in Python, and want to get your hands _dirty_, here's a few building blocks useful to get the most from the workshop:

1. __Python__ ...All you _really_ need is a Python code interpreter installed as a foundation.
   1. Start from the source, [Python Software Foundation's helpful steps](https://wiki.python.org/moin/BeginnersGuide/Download) and downloads (yep, the be all end all source).
      1. Many computers come with a version pre-installed, a bit old, but if you don't want to touch or download anything, it may get you acquainted, at least. (to check in command line or terminal, run **python --version**)
   2. Or Python comes with an [Anaconda installation](https://docs.anaconda.com/anaconda/install/index.html) (bigger topic than this workshop, but if you're in it for the long haul using Python consider e.g. the Individual Edition or a miniconda).
<br><br>
2. A virtual environment (_optional_, but do this next if you're doing it.)
   1. Skip this step if the sound of it or # steps has you scared away already! Don't go, stay!
   2. It's _recommended_, but not necessary, to make and work in an isolated virtual environment for any Python project like this one, to help manage work requiring different versions of things. 
      1. Options to manage this: 
         1. I find [virtualenv](https://virtualenv.pypa.io/en/latest/user_guide.html#python-discovery) a sure bet, 
            1. (e.g. On Mac Terminal (Zsh), from my project root folder, I ran **virtualenv plotlystyle_env** to make it; to activate it, I'll run **source plotlystyle_env/bin/activate**) _*pip install virtualenv*__if necessary first._
            2. I'll refer you to the docs for Windows.
         2. the simplified [venv](https://docs.python.org/3/library/venv.html#module-venv) built into Python version 3.3+, 
         3. [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) which I feel is cleanest with its centralized file structure, but fussy at times like an angry schoolchild, and 
         4. those are the big ones.
<br><br>
3. [__Jupyter Notebook__](https://docs.jupyter.org/en/latest/install/notebook-classic.html) (strongly recommended, we'll spend the workshop in the .ipynb Notebook file)
   1. Notebooks run directly in your web browser, so you need: Chrome, Safari, or Firefox (up to date Opera and Edge *maybe* works)
   2. If you installed an Anaconda distribution in step 1, congratulations, Jupyter Notebook is included! Read up on [running the Notebook](https://docs.jupyter.org/en/latest/running.html#running) where we'll pick up!
   3. You can alternately install Jupyter Notebook with the [pip](https://pip.pypa.io/) package manager.

   4. If you're working in a virtual environment (step 2 above), also install the [IPython kernel](https://ipython.readthedocs.io/en/stable/install/kernel_install.html).
      1. Otherwise, this Jupyter Notebooks does have this automatically for your system Python interpreter. 
      2. This basically supports more quick, interactive, code which makes Notebooks great for learning in chunks, and exploring without running a whole script.

4. Kiss your brain!

<span style="color:Teal">_*Who's tired of hyperlinks and docs already?! You promised fun!*_</span>
<br><br>

#### General Disclaimer
This work is open source, like [Plotly Open Source Graphing Libraries](https://plotly.com/graphing-libraries/), so try it, use it and spread the love by teaching someone else!<br>
To keep up with what others are working on, join the [Plotly Community Forum](https://community.plotly.com/).
Made with 💌 for the Python and data viz ecosystems under the limited liability company Data, Design & Daughters LLC doing business as Data Design Dimension by Kathryn Hurchla.

<!-- my custom buy me and a mentee a tea button -->
<a href="https://www.buymeacoffee.com/earthtokathy"><img src="https://img.buymeacoffee.com/button-api/?text=Fuel coding styles with tea&emoji=🍵&slug=earthtokathy&button_colour=ecd0df&font_colour=062D3F&font_family=Poppins&outline_colour=000000&coffee_colour=FFDD00"></a>