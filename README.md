# Interactive-Dashboard

The notebook contains code primarily focused on building an interactive dashboard for a CSV file named indian_food using the libraries such as panel, bokeh, and pandas.

1. First Cell: Installing/Checking Requirements
It checks for required libraries like panel, bokeh, param, and pandas. These are necessary for data visualization and dashboard creation.

2. Second Cell: Loading Data
The code loads a dataset from a CSV file called indian_food.csv using pandas. The first 10 rows of the dataset are displayed using food.head(10).

3. Third Cell: Environment Detection
A function named environment() determines whether the code is running in a Jupyter notebook or a server environment. If it detects the notebook environment, it returns 'notebook', otherwise, it returns 'server'.

4. Creating Interactive Elements
pn.Row(state_slider.controls(jslink=True), state_slider): This code creates a row layout with a range slider. The slider allows users to interact with the dashboard by selecting values within a certain range.

5. Using Widgets for User Input
Various inputs and sliders are created:
LiteralInput(description='Allows to create additional controls', ...): This is used to create literal inputs.
RangeSlider(end=3.14, ...): This range slider allows users to choose values between 0 and 3.14.
Other widgets like Select, Checkbox, and IntInput are added to allow users to select options, check boxes, or input integers.

6. Data Binding and Interactivity
The slider values (state_slider.value) are dynamically updated based on user interaction, and this is reflected in the dashboard output.

The final five cells of the notebook relate to generating and displaying interactive visualizations using the hvplot library in combination with Panel to create a dashboard. Here's a summary of the last five cells:

7. Sets up the interactive visualization by defining an hvplot object (ihvplot). This object plots data on the x-axis (course) and y-axis (a dynamic variable yaxis), grouped by the flavor_profile, with custom colors and line width.

8. Instantiates the plot (ihvplot), which outputs an interactive plot. This allows for dynamic updates based on changes in the dashboard's filters.

9. Launches a local server using panel for viewing the dashboard. This allows users to interact with the dashboard via a web interface. The server runs locally on a specified port.

10. Creates a FastListTemplate for the dashboard. This template includes a sidebar for user inputs (like cook_time, course, and yaxis), and the main panel displays multiple plots (ihvplot, scatter, line, hist, bar, box, violin, and heatmap).

11. Runs the template.show() function, which displays the interactive dashboard on the local server. The dashboard contains the interactive plots mentioned earlier, all styled with a consistent color theme.



#CODES




