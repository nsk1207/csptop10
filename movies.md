## Top 10 Albums of the Year
> Here, you can find our top 10 movies of 2022. What do you think? 

### 1. Top Gun: Maverick
Paramount Pictures | May 27
Domestic Total: $718.7M
Domestic Opening Weekend: $126.7M (three-day); $160.5M (four-day)


### 2. Avatar: The Way of Water*
20th Century Studios / Disney | December 16
Domestic Total (2022): $446.9M
Domestic Opening Weekend: $134.1M


### 3. Black Panther: Wakanda Forever*
Walt Disney Studios Motion Pictures | November 11
Domestic Total: $439.9M
Domestic Opening Weekend: $181.3M


### 4. Doctor Strange in the Multiverse of Madness
Walt Disney Studios Motion Pictures | May 6
Domestic Total: $411.3M
Domestic Opening Weekend: $187.4M


### 5. Jurassic World: Dominion
Universal Pictures | June 10
Domestic Total: $376.8M
Domestic Opening Weekend: $145M


### 6. Minions: The Rise of Gru
Universal Pictures | July 1
Domestic Total: $369.6M
Domestic Opening Weekend: $107M


### 7. The Batman
Warner Bros. | March 4
Domestic Total: $369.3M
Domestic Opening Weekend: $134M


### 8. Thor: Love and Thunder
Walt Disney Studios Motion Pictures | July 8
Domestic Total: $343.2M
Domestic Opening Weekend: $144.1M


### 9. Sonic the Hedgehog 2
Paramount Pictures | April 8
Domestic Total: $190.8M
Domestic Opening Weekend: $72.1M


### 10. Black Adam
Warner Bros. | October 21
Domestic Total: $168M
Domestic Opening Weekend: $67M


<html>
  <head>
    <title>Movie Matching Game</title>
    <style>
      /* Style the game board */
      #game-board {
        display: flex;
        flex-wrap: wrap;
        width: 500px;
        margin: 0 auto;
      }
      /* Style the cards */
      .card {
        width: 125px;
        height: 125px;
        border: 1px solid black;
        text-align: center;
        line-height: 125px;
        font-size: 18px;
        background-color: white;
        color: black;
        cursor: pointer;
      }
      /* Style the cards when they are turned over */
      .card.flipped {
        background-color: black;
        color: white;
      }
      /* Style the cards when they are matched */
      .card.matched {
        background-color: green;
        color: white;
        pointer-events: none;
      }
    </style>
  </head>
  <body>
    <h1>Movie Matching Game</h1>
    <div id="game-board">
      <!-- Cards will be added here -->
    </div>
    <script>
      // Create an array of movie titles
      const movieTitles = [
        "Top Gun: Maverick",
        "Avatar: The Way of Water",
        "Black Panther: Wakanda Forever",
        "Doctor Strange in the Multiverse of Madness",
        "Jurassic World: Dominion",
        "Minions: The Rise of Gru",
        "The Batman",
        "Thor: Love and Thunder",
        "Sonic the Hedgehog 2",
        "Black Adam"
      ];

<script>
      // Shuffle the array of movie titles
      function shuffleArray(array) {
        for (let i = array.length - 1; i > 0; i--) {
          const j = Math.floor(Math.random() * (i + 1));
          [array[i], array[j]] = [array[j], array[i]];
        }
        return array;
      }
      const shuffledTitles = shuffleArray(movieTitles);

      // Create an array of movie pairs
      const moviePairs = [];
      for (let i = 0; i < shuffledTitles.length; i += 2) {
        moviePairs.push([shuffledTitles[i], shuffledTitles[i + 1]]);
      }

      // Create HTML elements for the game board
      const gameBoard = document.getElementById("game-board");
      for (const pair of moviePairs) {
        const card1 = document.createElement("div");
        card1.classList.add("card");
        card1.addEventListener("click", flipCard);
        card1.textContent = pair[0];
        gameBoard.appendChild(card1);

        const card2 = document.createElement("div");
        card2.classList.add("card");
        card2.addEventListener("click", flipCard);
        card2.textContent = pair[1];
        gameBoard.appendChild(card2);
</script>