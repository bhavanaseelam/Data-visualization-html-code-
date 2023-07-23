# Data-visualization-html-code-
<!DOCTYPE html>
<html>
<head>
    <title>Dynamic Data Visualization</title>
    <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
</head>
<body>
    <div id="chart"></div>
    <script>
        // Load the JSON data for the chart and create the plot
        var graphJSON = {{ graphJSON | safe }};
        Plotly.newPlot('chart', graphJSON.data, graphJSON.layout);
    </script>
</body>
</html>
