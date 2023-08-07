<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
</script>

<main>
  <div class="gameboard">
    <div class="card">
      <h3 class="card__comandname">Команда №1</h3>
      <Counter />
    </div>
    <div class="card">
      <h3 class="card__comandname">Команда №2</h3>
      <Counter />
    </div>
    <div class="card">
      <h3 class="card__comandname">Команда №3</h3>
      <Counter />
    </div>
  </div>

  <p class="read-the-docs">
    
  </p>
</main>

<style>
  .read-the-docs {
    color: #888;
  }
  .gameboard {
    display: flex;
  }
  .card {
    width: 300px;
    font-size: 40px;
    background-color: #ECECEC;
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

  .card__comandname { 
    margin-bottom: 20px;
  }
</style>
