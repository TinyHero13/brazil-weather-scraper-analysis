# Nova Iguaçu Weather Analysis
[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)

# Table of Contents
- [Introduction](#introduction)
- [How to Use](#how-to-use)
- [Setup](#setup)
- [Power BI Report](#power-bi-report)

# Introduction
[Back to top](#table-of-contents)

A script built to analyze the maximum and minimum weekly temperatures in Nova Iguaçu, RJ.

Built using Google Colab, it calculates the minimum, maximum, and average temperatures for the week. Data is scraped from [tempo.com](https://www.tempo.com/nova-iguacu.htm).

# How to Use
[Back to top](#table-of-contents)

To scrape weather data for a different location, search for the desired city on [tempo.com](https://www.tempo.com/) and update the URL in the request:

```python
r = requests.get('newLink')
```

# Setup
[Back to top](#table-of-contents)

The following libraries are required to run the project:

- `requests` — to fetch the URL content
- `bs4` — for parsing HTML with BeautifulSoup
- `pandas` — to transform the data into a DataFrame
- `google.colab` — to download the output CSV file

Import them at the top of your notebook:

```python
import requests
import re
import pandas as pd
from bs4 import BeautifulSoup
from google.colab import files
```

# Power BI Report
[Back to top](#table-of-contents)

For a better visualization of the data, the DataFrame was exported as a CSV and imported into Power BI:

![Report](https://github.com/TinyHero13/climaNovaIguacu/blob/main/assets/relatorio.png)
