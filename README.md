# jupyter-starter
Starter repo with the bare minimum to start a new jupyter notebook

Assumptions
-----------

The following things are assumed to be true in this documentation.

* You are running OSX.
* You are using Python 2.7. (Probably the version that came OSX.)
* You have [virtualenv](https://pypi.python.org/pypi/virtualenv) and [virtualenvwrapper](https://pypi.python.org/pypi/virtualenvwrapper) installed and working.
* You have NPR's AWS credentials stored as environment variables locally.

For more details on the technology stack used with the app-template, see our [development environment blog post](http://blog.apps.npr.org/2013/06/06/how-to-setup-a-developers-environment.html).


Bootstrap the project
---------------------

```
cd jupyter-starter
mkvirtualenv TKTK
pip install -r requirements.txt
```

**Problems installing requirements?** You may need to run the pip command as ``ARCHFLAGS=-Wno-error=unused-command-line-argument-hard-error-in-future pip install -r requirements.txt`` to work around an issue with OSX.

Run the notebook
---------------

`
jupyter notebook
`

Import the libraries in the first cell
---------------

```
# -*- coding: utf-8 -*-
%matplotlib inline
import pandas as pd
import numpy as np
import seaborn as sns
import math
import matplotlib as mplstyle
import matplotlib.pyplot as plt
import locale from locale
import atof from dateutil
import parser from datetime
import datetime
import arrow
```
