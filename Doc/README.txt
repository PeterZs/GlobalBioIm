###### DESCRIPTION
The documentation is generated using Sphinx
     http://www.sphinx-doc.org/en/stable/
together with the matlabdomain extension
     https://pypi.python.org/pypi/sphinxcontrib-matlabdomain
Documentation is generated from Matlab's comments

###### SETUP
some commands that worked on macOSX

sudo -H pip install --ignore-installed Sphinx
sudo -H pip install --ignore-installed -U sphinxcontrib-matlabdomain
sudo -H pip install --ignore-installed sphinx_rtd_theme
sudo -H pip install --ignore-installed sphinxcontrib-email 

###### COMPILATION

    1. To make the documentation, type
    
       make html

    1a. To see the results, open Doc/build/index.html in a web browser.

    2. To clean up for release:
    
    add style="text-align:justify" in the body "basile":
    <body class="wy-body-for-nav" role="document" style="text-align:justify">
    I did not find a nicer way to do that... 
    
    add <img src="logo.png"  width="300" /> at the following position
    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
    <div class="wy-side-scroll">
       <img src="logo.png"  width="300" />  <<<------- HERE
    <div class="wy-side-nav-search">
    

###### HOW TO USE

	- within your comments you can refer to any:
	     - class by      :class:`classname`
	     - attribute by  :attr:`attributename`
	     - method by     :meth:`mathodname`
	
	- You can insert latex within $$ $$ or \\(  \\) (inline) and this will be correctly interpreted.
	  Note that backslashes have to be doubled '\\' (i.e. \int_x --> \\int_x)
	  
	- Let an empty line (i.e. without any %) before the copyright paragraph:
	% See also :class:`LinOp`.

    %     Copyright (C) 2017 ...
    
    
    
	
	
	

