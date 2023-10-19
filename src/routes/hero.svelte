<section class="hero-container">
  <div class="hero__content">
    <div class="hero__text">
      <h1 class="hero__title">Hello!</h1>
      <h2 class="hero__subtitle">My name is Karnikaa Velumani</h2>
    </div>
  </div>
</section>

<style>
  :global(body) {
    background-color: black;
    background-image: url('/assets/planet.svg');
    background-repeat: no-repeat;
    background-position: -10% -5%;
    background-size: 250%;
  }

  section {
    display: grid;
  }

  .hero-container {
    display: grid;
    justify-self: center;
    align-items: center;
    height: 100vh;
    width: 100%;
  }

  .hero__content {
    display: grid;
    grid-template-columns: 1fr;
    justify-self: center;
    align-items: center;
  }

  .hero__text {
    display: grid;
    justify-self: center;
    align-items: center;
    color: #fff;
  }

  .hero__title {
    font-size: 8rem;
    font-weight: 700;
    margin: 0 1em 0 1em;
  }

  .hero__subtitle {
    font-size: 2rem;
    font-weight: 400;
    margin: 0 1em 0 1em;
  }

  @media (min-width: 768px) {
    :global(body) {
      background-position: 100% 0%;
      background-size: 70%;
    }

     section {
      display: grid;
    }

    .hero__content {
      display: grid;
      grid-template-columns: 1fr 1fr;
      justify-self: center;
      align-items: center;
    }

    .hero__text {
      display: grid;
      justify-self: start;
      margin: 0 5em 0 10rem;
      z-index: 10;
    }

    .hero__title {
      font-size: 15rem;
      text-align: start;
      margin: 0;
      margin-bottom: -0.3em;
    }

    .hero__subtitle {
      font-size: 4rem;
      text-align: start;
      margin: 0;
    }

  }
</style>