<script>
  import Ophold_afrejse from "../components/ophold_afrejse.svelte";
  import MyButton from "../components/button.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section class="maxwidthwrapper" id="no-pad">
    <h2 class="">AFREJSEDATOER</h2>
    <p>
      Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
      Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
      masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved Buck
      Island og turtlewatch på programmet.
    </p>

    <br />
    <hr />

    <section class="grid gap-8" id="no-inner-pad">
      <h4>2022</h4>
      <div class="grid gap-8">
        <Ophold_afrejse
          dato="06. Jul 2022"
          pris="29.000 DKK"
          varig="3 måneder"
        />
        <Ophold_afrejse
          dato="06. Sep 2022"
          pris="29.700 DKK"
          varig="3 måneder"
        />
        <Ophold_afrejse
          dato="06. Dec 2022"
          pris="31.400 DKK"
          varig="3 måneder"
        />
      </div>

      <h4>2023</h4>
      <div class="grid gap-8">
        <Ophold_afrejse
          dato="02. Mar 2023"
          pris="31.900 DKK"
          varig="3 måneder"
        />
        <Ophold_afrejse dato="04. Apr 2023" pris="32.700" varig="3 måneder" />
        <Ophold_afrejse dato="05. Maj 2023" pris="33.00" varig="3 måneder" />
      </div>
    </section>
  </section>

  <section class="flex justify-end px-4">
    <MyButton type="linkbutton"> GODT AT VIDE<svg class="m-auto" width="18" height="16" viewBox="0 0 18 16" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M17.7071 8.70711C18.0976 8.31658 18.0976 7.68342 17.7071 7.29289L11.3431 0.928932C10.9526 0.538408 10.3195 0.538408 9.92893 0.928932C9.53841 1.31946 9.53841 1.95262 9.92893 2.34315L15.5858 8L9.92893 13.6569C9.53841 14.0474 9.53841 14.6805 9.92893 15.0711C10.3195 15.4616 10.9526 15.4616 11.3431 15.0711L17.7071 8.70711ZM17 7L-4.76837e-07 7V9L17 9V7Z" fill="#929292"/>
      </svg></MyButton> 
  </section>
</main>

<style>
  main {
    background-image: url(src/_icons/gurfers.png);
    background-position: cover;
    background-size: 500%;
    background-repeat: repeat-y;
    background-position-y: 10%;
  }
  section {
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }

  #no-pad {
    padding-top: 0;
  }

  #no-inner-pad {
    padding-left: 0;
    padding-right: 0;
  }
</style>
