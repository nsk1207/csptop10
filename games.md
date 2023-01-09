## Top 10 Games of the Year
> Here, you can find our top 10 games of 2022. What do you think? 

### #10: 









<!-- Include Chart.js library -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.3/Chart.min.js%22%3E</script>

<!-- Chart container -->
<div id="chart-container">
  <canvas id="myChart"></canvas>
</div>

// Function to create the chart
<script>
function createChart() {
  // Get the user input from the form
  var input = document.getElementById("user-input").value;

  // Parse the input to extract the data for the chart
  var data = parseInput(input);

  // Get the chart container element
  var ctx = document.getElementById("myChart");

  // Create a new Chart.js chart
  var chart = new Chart(ctx, {
    type: 'line',
    data: {
      labels: data.labels, // x-axis labels
      datasets: [{
        label: 'My Chart',
        data: data.data, // y-axis data
        backgroundColor: 'rgba(255, 99, 132, 0.2)',
        borderColor: 'rgba(255, 99, 132, 1)',
        borderWidth: 1
      }]
    },
    options: {
      scales: {
        yAxes: [{
          ticks: {
            beginAtZero: true
          }
        }]
      }
    }
  });
}
</script>

<!-- HTML form for user input -->
<form>
  <label for="user-input">Enter data:</label><br>
  <input type="text" id="user-input" value="10,20,30,40,50"><br>
  <input type="button" value="Submit" onclick="createChart()">
</form>