## Top 10 Games of the Year
> Here, you can find our top 10 games of 2022. What do you think? 

### 10) Horizon: Forbidden West

### 9) Gran Turismo 7

### 8) Gothan Knights

### 7) Nintendo Switch Sports

### 6) Splatoon 3

### 5) Return to Monkey Island

### 4) LEGO Star Wars: The Skywalker Saga

### 3) Sonic Frontiers
Sonic Frontiers shows that SEGA still has the ability to make great games. An awesome open-world game with awesome gameplay to boot. Honestly shattered the expectations that people set for this series.
### 2) God of War
The sequel to the GOTY winning PS4 title God of War, Ragnarok smashes the high expectations set by the first game. The story picks up even more steam and the gameplay also gets a massive improvement as well.
### 1) Elden Ring
This massive open world RPG game is another classic by From Software. The expansive open world experience is followed by incredibly well designed bosses and encounters! Pair that with a very in-depth RPG system and you got yourself the game of the year!








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