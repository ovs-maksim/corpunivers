<script>
  import svelteLogo from "./assets/svelte.svg";
  import viteLogo from "/vite.svg";
  import Counter from "./lib/Counter.svelte";
  import Question from "./lib/Question.svelte";
</script>

<main>
  <div class="gameboard">

    <div class="gameboard__question question">
      <div class="question__card card">
        <h3 class="card__comandname">Вопрос</h3>
        <Question />
      </div>
    </div>
    <div class="gameboard__score score">
      <div class="score__card card">
        <h3 class="card__comandname">Команда №1</h3>
        <Counter />
      </div>
      <div class="score__card card">
        <h3 class="card__comandname">Команда №2</h3>
        <Counter />
      </div>
      <div class="score__card card">
        <h3 class="card__comandname">Команда №3</h3>
        <Counter />
      </div>
    </div>
  </div>
</main>

<style>
  .gameboard {
    display: flex;
  }
  .gameboard__score {
    display: flex;
  }

  .card {
    font-size: 40px;
    background-color: #ececec;
    margin: 0px 20px;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: start;
    /* padding:; */
    padding-top: 20px;
    padding-left: 0;
    padding-right: 0;
    padding-bottom: 10px;
  }

  .score__card {
    width: 300px;
  }

  .question {
    flex-grow: 1;
  }

  .card__comandname {
    margin-bottom: 20px;
  }
</style>
