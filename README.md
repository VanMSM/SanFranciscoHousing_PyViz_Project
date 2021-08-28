# San Francisco Housing Analysis


![6-4-challenge-image](https://user-images.githubusercontent.com/80144026/131201552-2e199e9e-e1c7-43b5-b5f4-554aecc2a2c2.png)

In this project, I assume the role of an  analyst at a proptech company that wants to offer an instant, one-click service for people to buy properties and then rent them. The company wants to have a trial of this offering in the San Francisco real-estate market. If the service proves popular, they can then expand to other markets.

I am using data visualization, including aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

___



## Technologies

This project is written in Python within the Jupyter Lab environment with the following packages:

* Pyviz
* MapBox API


## Installation Guide
Before running the application first install and verify the following dependencies:
 
* Install the PyViz Ecosystem. From your terminal, activate dev environment:
 ```python
conda install -c plotly plotly=4.13.
conda install -c pyviz hvplot
conda install -c conda-forge nodejs=12
 ```
 note: Make sure to use Plotly version 4.13.0 and hvPlot version 0.7.0 or later, and NodeJS version 12 or later.

* Install the JupyterLab Dependencies
 ```python
conda install -c conda-forge jupyterlab=2
jupyter labextension install jupyterlab-plotly@4.13.0 --no-build
jupyter labextension install @jupyter-widgets/jupyterlab-manager plotlywidget@4.13.0 --no-build
jupyter labextension install @pyviz/jupyterlab_pyviz --no-build
jupyter lab build (note: this may take a few minutes to install)
 ```
 ## Set Up MAPBOX API
 
 * Navigate: https://account.mapbox.com/access-tokens/
 *  Enter a username, your email, and a password. Check the “I agree to the Mapbox Terms of Service and Privacy Policy” box at the bottom of the page, and then click the “Get started” button, as the following image shows:

<img width="557" alt="Screen Shot 2021-08-27 at 6 55 18 PM" src="https://user-images.githubusercontent.com/80144026/131202626-5b774638-289d-485a-912f-8f176dd9edc7.png">
* Note that the Account page displays the default public token, which is your Mapbox API access token. Copy this token to a document on your local computer for safekeeping. The following image shows the Account page:

<img width="573" alt="Screen Shot 2021-08-27 at 6 55 43 PM" src="https://user-images.githubusercontent.com/80144026/131202640-0b938195-e26e-4c9c-b6c6-e1d4fd301c34.png">

You’ll use the Mapbox API access token together with an environment file (.env) to import it into the notebooks where you’ll create your visualizations.

* Next, Import the Modules

 ```python
import os
import pandas as pd
import plotly.express as px
import hvplot.pandas
from pathlib import Path
from dotenv import load_dotenv
```

* Clone to your repo and run in Jupyter Lab.


## DEMO IMAGES

<img width="887" alt="Screen Shot 2021-08-27 at 2 50 34 PM" src="https://user-images.githubusercontent.com/80144026/131201590-0bb3ce7c-111b-4b79-b855-c2dbb912cc57.png">

<img width="891" alt="Screen Shot 2021-08-27 at 4 59 50 PM" src="https://user-images.githubusercontent.com/80144026/131201570-b9ecf313-28e2-4516-91e7-7511f4c949b8.png">

<img width="893" alt="Screen Shot 2021-08-27 at 5 00 27 PM" src="https://user-images.githubusercontent.com/80144026/131201572-9bb0344e-ca1b-4597-b872-8aa06184a63f.png">

<img width="900" alt="Screen Shot 2021-08-27 at 5 08 55 PM" src="https://user-images.githubusercontent.com/80144026/131201575-8d7a6718-94c1-4c51-8b27-7a0dddfda002.png">

<img width="1317" alt="Screen Shot 2021-08-27 at 6 31 56 PM" src="https://user-images.githubusercontent.com/80144026/131202918-12756fc3-5b16-4964-8698-e3d0a5d6fbde.png">



https://user-images.githubusercontent.com/80144026/131202731-339af4f6-ee4c-43de-bba5-fef6bcdf2161.mov

## Contributors

* [Van Maquilan](https://www.linkedin.com/in/van-miller-sarcov-maquilan-20b472202/)

## License

MIT License

 Copyright (c) 2021 VanMSM

 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:

 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.

 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.



