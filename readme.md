###Confidence Interval Simulation App

This is a **Confidence Interval Simulation** app built using **Streamlit**. The app allows users to simulate confidence intervals based on various methods (Z-procedure or T-procedure) and visualize how often the intervals capture the true population mean.

## Features:

- **Simulate Confidence Intervals**: The app generates random samples from a population and computes confidence intervals based on user-specified parameters.
- **Multiple Methods**: Users can choose between:
  - "Z with sigma" (using the population standard deviation)
  - "Z with s" (using the sample standard deviation)
  - "T with s" (using the T-distribution and sample standard deviation)
- **Interactive Sliders**: Customize the following parameters in the sidebar:
  - Sample Size: Number of observations in each simulation.
  - Population Mean: The true mean of the population.
  - Population Standard Deviation: The true standard deviation of the population.
  - Number of Simulations: Total number of simulations to run.
  - Confidence Level: Desired confidence level (e.g., 95%).
- **Graphical Output**: The app displays a plot showing the confidence intervals from each simulation, along with the actual population mean for comparison.
  - Intervals that capture the true population mean are displayed in **blue**.
  - Intervals that miss the population mean are shown in **orange**.
- **Summary**: The app shows the percentage of simulations where the confidence interval successfully captured the population mean.

## How to Use:

1. Adjust the input parameters using the **sliders** in the sidebar.
2. Select the **method** for calculating confidence intervals:
   - **Z with sigma**: Confidence intervals are computed using the population standard deviation.
   - **Z with s**: Confidence intervals are computed using the sample standard deviation.
   - **T with s**: Confidence intervals are computed using the sample standard deviation and the T-distribution.
3. The app will automatically run the simulations, plot the results, and display the percentage of intervals that capture the population mean.

## Running the App Locally:

### Prerequisites:

Ensure that you have **Python** installed along with the following dependencies:

- **Streamlit**
- **NumPy**
- **SciPy**
- **Matplotlib**

You can install the required packages using `pip`:

```bash
pip install streamlit numpy scipy matplotlib
Running the App:
Clone this repository:
bash
Copy code
git clone https://github.com/your-username/confidence-interval-simulation.git
cd confidence-interval-simulation
Run the Streamlit app:
bash
Copy code
streamlit run app.py
The app will open in your web browser at http://localhost:8501.
File Overview:
app.py: The main Python script that contains the Streamlit app and the logic for the confidence interval simulations.
README.md: This documentation file.
Technologies Used:
Streamlit: For creating the web app interface.
NumPy: For generating random samples and performing numerical computations.
SciPy: For calculating critical values from normal and T-distributions.
Matplotlib: For plotting the confidence intervals and visualizing the results.