<script>
    import Header from '../../layout/Header.svelte';
    import Footer from '../../layout/Footer.svelte';

    let questions = [
      {
        question: "Favorite Outdoor Setting:",
        choices: ["Forest or Woods", "Flower Garden", "Ocean or Lakeside", "Exotic Spice Market"],
        answer: "Ocean or Lakeside",
      },
      {
        question: "Preferred Flower:",
        choices: [
          "None - I prefer the scent of trees and earth",
          "Sampaguita or Ylang-Ylang",
          "Calamansi Blossom or Dama de Noche",
          "Orchid or Gumamela",
        ],
        answer: "None - I prefer the scent of trees and earth",
      },
      {
        question: "Ideal Vacation Destination:",
        choices: ["Mountain Cabin", "Countryside Bed and Breakfast", "Tropical Island", "Historic City in the Middle East or Asia"],
        answer: "Tropical Island",
      },
      {
        question: "Preferred Candle Scent:",
        choices: ["Sandalwood or Guijo Wood", "Sampaguita or Jasmine", "Mango or Coconut", "Cinnamon or Pandan"],
        answer: "Sandalwood or Guijo Wood",
      },
      {
        question: "Favorite Season:",
        choices: ["Fall", "Spring", "Summer", "Winter"],
        answer: "Fall",
      },
      {
        question: "Preferred Beverage:",
        choices: ["Barako Coffee or Lambanog", "Pandan or Lemongrass Tea", "Buko Juice or Calamansi Juice", "Salabat or Tsokolate"],
        answer: "Barako Coffee or Lambanog",
      },
      {
        question: "Favorite Dessert:",
        choices: [
          "Pili Nut Tart or Coconut Macaroons",
          "Ube Halaya or Bibingka",
          "Mango Float or Halo-Halo",
          "Espasol or Kalamay",
        ],
        answer: "Pili Nut Tart or Coconut Macaroons",
      },
    ];
  
    let currentQuestion = 0;
    let selectedChoice = null;
    let score = 0;
  
    function checkAnswer() {
      if (selectedChoice === questions[currentQuestion].answer) {
        score++;
      }
      nextQuestion();
    }
  
    function nextQuestion() {
      if (currentQuestion < questions.length - 1) {
        currentQuestion++;
        selectedChoice = null;
      } else {
        // Quiz is finished
        alert(`Your perfume is brewing... check your email!`);
      }
    }
  </script>
  
    <Header />  
  <div class="div">
    {#if currentQuestion < questions.length}
    <h1>{questions[currentQuestion].question}</h1>
    <ul>
      {#each questions[currentQuestion].choices as choice}
      <li>
        <label>
            <input type="radio" name="choices" bind:group={selectedChoice} value={choice} />
          {choice}
        </label>
      </li>
      {/each}
    </ul>
    <button on:click={checkAnswer}>Next</button>
    {:else}
    <p>No more questions.</p>
    {/if}
</div>
      
     <Footer />
  
  <style>
    .div {
      text-align: center;
      margin: 20px;
    }
  
    ul {
      list-style-type: none;
      padding: 0;
    }
  
    li {
      margin-bottom: 10px;
    }
  
    button {
      margin-top: 10px;
      padding: 8px 16px;
      cursor: pointer;
    }
  </style>
  