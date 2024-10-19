# EV Sales Visualization Project

This project creates an animated racing bar chart to visualize the year-wise sales of electric vehicles (EVs) by different makers over the last decade.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Data Preparation](#data-preparation)
6. [Creating the Visualization](#creating-the-visualization)
7. [Viewing the Result](#viewing-the-result)
8. [Troubleshooting](#troubleshooting)
9. [Contributing](#contributing)
10. [License](#license)

## Project Overview

This project uses Python to process EV sales data and create an animated visualization showing how different car makers compete in EV sales over time. The main output is an MP4 video file displaying a racing bar chart of EV sales.

## Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

## Installation

1. Clone this repository or download the project files.

2. Install the required Python packages:

   ```
   pip install pandas matplotlib bar_chart_race
   ```

   Note: If you encounter issues with `bar_chart_race`, you may need to upgrade it:

   ```
   pip install --upgrade bar_chart_race
   ```

## Usage

1. Prepare your EV sales data in a CSV file.
2. Run the data preparation script to create the required DataFrame.
3. Run the visualization script to generate the racing bar chart video.
4. View the resulting MP4 file.

## Data Preparation

1. Ensure your CSV file contains columns for 'Make', 'Model Year', and any other relevant data.
2. Run the data preparation script:

   ```python
   python prepare_data.py
   ```

   This will create a DataFrame suitable for the visualization.

## Creating the Visualization

Run the visualization script:

```python
python create_visualization.py
```

This will generate an MP4 file named `ev_sales_by_maker.mp4` in your project directory.

## Viewing the Result

You can view the MP4 file using any of the following methods:

1. Open it with your system's default video player.
2. Use Python to open it programmatically (see the provided code in `view_video.py`).
3. Display it in a Jupyter Notebook using IPython's `Video` function.
4. Use OpenCV to play the video within a Python script.

## Troubleshooting

- If you encounter "unexpected kwargs argument" errors, check your version of `bar_chart_race`:

  ```python
  import bar_chart_race as bcr
  print(bcr.__version__)
  ```

  If it's an older version (e.g., 0.1.0), consider upgrading or adjusting the code to use fewer parameters.

- Ensure your data is properly formatted and contains no unexpected null values.

## Contributing

Contributions to improve the project are welcome. Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature.
3. Add your changes.
4. Submit a pull request.

## License

This project is open-source and available under the MIT License.
