<script>
  let clicks = 0;
  function increaseClicks() {
    clicks++;
  }
</script>

<main>
  <h2>클릭 : {clicks}</h2>
  <button on:click={increaseClicks}>클릭!!</button>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  button {
    border: 0;
    background: tomato;
    color: white;
    border-radius: 50px;
    padding: 5px 20px;
    cursor: pointer;
  }
  button:active {
    opacity: 0.5;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
