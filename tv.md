## Top 10 Tv Shows of the Year
> Here, you can find our top 10 tv shows of 2022. What do you think? 

### 10) House Of The Dragons

### 9) 1899

### 8) The Serpent Queen
 
### 7) Tusla King

### 6) Night Sky

### 5) The Devil's Hour

### 4) Stranger Things Season 4

### 3) Vampire Academey

### 2) Wednesday

### 1) Eurphoria 


<html>
  <head>
    <title>Show Personality Quiz</title>
    <style>
      /* Style the quiz container */
      .quiz-container {
        max-width: 600px;
        margin: 0 auto;
        text-align: center;
      }
      /* Style the quiz question */
      .quiz-question {
        font-size: 18px;
        margin: 20px 0;
      }
      /* Style the quiz choices */
      .quiz-choice {
        display: inline-block;
        margin: 10px;
        padding: 10px 20px;
        border: 1px solid black;
        cursor: pointer;
      }
      /* Style the quiz result */
      .quiz-result {
        margin: 20px 0;
        font-size: 20px;
      }
    </style>
  </head>
  <body>
    <div class="quiz-container">
      <h1>Which Show Are You?</h1>
      <!-- Quiz questions and choices will be added here -->
      <div class="quiz-result"></div>
    </div>
    <script>
      // Define the quiz questions and choices
      const quizData = [
        {
          question: "Which of these shows do you prefer?",
          choices: [
            "House Of The Dragons (Fantasy)",
            "1899 (Mystery)",
            "The Serpent Queen (Action)",
            "Tusla King (Drama)",
            "Night Sky (Action)",
            "The Devil's Hour (Drama)",
            "Stranger Things Season 4 (Action)",
            "Vampire Academy (Action)",
            "Wednesday (Mystery)",
            "Euphoria (Drama)"
          ]
        }
      ];
      // Set the initial quiz state
      let currentQuestionIndex = 0;
      let selectedChoices = [];
      // Get the quiz container element
      const quizContainer = document.querySelector(".quiz-container");
      // Create a function to render the quiz
      function renderQuiz() {
        // Clear the quiz container
        quizContainer.innerHTML = "";
        // Get the current quiz data
        const currentQuestion = quizData[currentQuestionIndex];
        // Add the quiz question
        const questionElement = document.createElement("div");
        questionElement.classList.add("quiz-question");
        questionElement.textContent = currentQuestion.question;
        quizContainer.appendChild(questionElement);
        // Add the quiz choices
        for (const choice of currentQuestion.choices) {
          const choiceElement = document.createElement("div");
          choiceElement.classList.add("quiz-choice");
          choiceElement.textContent = choice;
          choiceElement.addEventListener("click", selectChoice);
          quizContainer.appendChild(choiceElement);
        }
      }
      // Create a function to select a quiz choice
      function selectChoice() {
        // Add the selected choice to the selected choices array
        selectedChoices.push(this.textContent);
        // Go to the next question
        currentQuestionIndex++;
        // If there are no more questions, show the result
       </script>