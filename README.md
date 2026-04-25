# Billboard Hot 100 Animation Tutorial (2025)

This repository contains a tutorial on building animated data visualizations with Python using `matplotlib.animation`. The tutorial uses Billboard Hot 100 data from 2025, which is the most recent complete year available in the dataset used for this project as of April 25, 2026. Overal, the goal of the tutorial is to display how animation can be used to communicate change over time in a way that is visually engaging and analytically clear. 

Overall, the focus is on building animated data visualizations in Python using **Matplotlib**, **FFmpeg**, and **ImageMagick** with real Billboard Hot 100 data from 2025.

This repository was created as an honors option project for **CMSE 402: Data Visualization Principles and Techniques** at **Michigan State University**.

## Project Overview

This tutorial focuses on two types of animated visualizations:

1. **Bar Chart Race**
   - Shows songs building chart longevity over the course of 2025
   - Demonstrates how to animate ranked categories over time

2. **Song Rank Trajectory**
   - Follows three songs across multiple chart weeks
   - Demonstrates how to animate movement through the Billboard rankings

The notebook walks through the full animation process, including:

- loading Billboard Hot 100 data directly from a public URL
- filtering the dataset to 2025
- exploring song longevity with EDA before animating anything
- focusing in/testing out a single frame before creating a full animation
- building animations with `FuncAnimation`
- previewing animations inside Jupyter
- exporting animations using **FFmpeg** or **ImageMagick** and their differences

## Repository Contents

- `402_animation_notebook.ipynb`  
  Main tutorial notebook containing the full walkthrough, code, explanations, and animations.
- `README.md`  
  Overview of the project, dataset, tools, and course context.


## Dataset

This project uses the following publicly available dataset:

- [Billboard Hot 100 Current Data](https://raw.githubusercontent.com/utdata/rwd-billboard-data/main/data-out/hot-100-current.csv)

The tutorial filters this dataset to only include entries from **2025**.

## Dataset

This project uses the following publicly available dataset:

- [Billboard Hot 100 Current Data](https://raw.githubusercontent.com/utdata/rwd-billboard-data/main/data-out/hot-100-current.csv)

The dataset is loaded directly from the public URL inside the notebook, so no manual download is required.

The tutorial filters the dataset to only include entries from **2025**.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- `matplotlib.animation`
- FFmpeg
- ImageMagick
- Jupyter Notebook

## Prerequisites

To run the notebook, make sure you have Python and the required libraries installed.

Install the Python dependencies with:

```bash
pip install pandas matplotlib numpy
```

Example packages used in the notebook:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from matplotlib.animation import FuncAnimation
from IPython.display import HTML, display
```

To save animations as files, **FFmpeg** or **ImageMagick** may need to be installed on your computer.


## How to Run

1. Clone or download this repository.
2. Open `402_animation_notebook.ipynb` in Jupyter Notebook or JupyterLab.
3. Run the cells from top to bottom.
4. To export the animations, uncomment the `.save()` lines in the notebook.
5. Make sure FFmpeg or ImageMagick is installed if saving animations as MP4 or GIF files.

## Why This Tutorial

Many visualization tutorials focus on static plots, while animation tutorials are often either too brief or too advanced for beginners. Along with this, most animation tutorials online use synthetic data instead of any real world application data that is more simple for the average viewer to understand. This project was designed to fill that gap by giving a clear example of how animated visualizations can be built in Python using a real, relevant, and recent public dataset. Along with this, this tutorial also emphasizes that animation should have a purpose. Instead of just being used as a visual effect, the examples show how motion can assist in communicating more factors depending on your specific data. It aims to help understand why one should make the choice to employ animation in their visualizations!


## Running the Notebook

To run the notebook, make sure you have Python and the required libraries installed.

Example packages used in the notebook:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from matplotlib.animation import FuncAnimation
from IPython.display import HTML, display
```

The notebook can be run in Jupyter Notebook, JupyterLab, or another environment that supports Python notebooks.

To export the animations, FFmpeg or ImageMagick may need to be installed.

## References
- Cairo, A. (2016). *The truthful art: Data, charts, and maps for communication*. New Riders. ISBN 978-0321934079.
- Segel, E., & Heer, J. (2010). Narrative visualization: Telling stories with data. *IEEE Transactions on Visualization and Computer Graphics, 16*(6), 1139–1148. https://doi.org/10.1109/TVCG.2010.179
- Tufte, E. R. (2001). *The visual display of quantitative information* (2nd ed.). Graphics Press. ISBN 978-0961392147.
