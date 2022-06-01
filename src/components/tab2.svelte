<script>
  import MyButton from "../components/button.svelte";
</script>

<main class="col-start-2">
  <!-- SECTION 1 -->
  <section class="maxwidthwrapper" id="no-pad">
    <section class="" id="no-pad">
    <h2>DET FÅR DU MED PÅ REJSEN</h2>
    <p class="">
      Når vi ikke arbejder, nyder vi stranden, drikker lækre drinks på
      Rumrunners eller snorkler efter havskildpadder. Derudover har vi haft en
      masse fede ting som fx Jeepsafari i den dybe regnskov, snorkling ved Buck
      Island og turtlewatch på programmet.
    </p>
    <br />

    <hr/>
  </section>

    <section class="grid gap-20 lg:col-start-1 inkl">
      <div>
          <div>
            <p class="preh2">DET FÅR DU MED</p>
            <h3>INKLUDERET</h3>
            
          </div>
       
        <div class="grid inner_spacing mt-12">
          <div>
            <p>OVERORDNET</p>
            <ul>
              <li>
                Fly tur/retur: DK > New York > Caribien > Mexico > Hawaii > DK
              </li>
              <li>Indkvartering i New York, Caribien, Mexico og Hawaii</li>
              <li>Undervisning i ‘Projektstyring & Teambuilding’</li>
              <li>Undervisning i ‘Frivilligt Arbejde & Kulturforståelse’</li>
              <li>Undervisning i ‘Selvudvikling & Kommunikation’</li>
              <li>Transfers fra lufthavne tur/retur</li>
              <li>
                15% rabat på vaccinationer hos ‘Danske Lægers Vaccinations
                Service’
              </li>
            </ul>
          </div>

          <div>
            <p>ADVENTURE, AKTIVITETER & OPLEVELSER</p>
            <ul>
              <li>
                Fly tur/retur: DK > New York > Caribien > Mexico > Hawaii > DK
              </li>
              <li>Indkvartering i New York, Caribien, Mexico og Hawaii</li>
              <li>Undervisning i ‘Projektstyring & Teambuilding’</li>
              <li>Undervisning i ‘Frivilligt Arbejde & Kulturforståelse’</li>
              <li>Undervisning i ‘Selvudvikling & Kommunikation’</li>
              <li>Transfers fra lufthavne tur/retur</li>
              <li>
                15% rabat på vaccinationer hos ‘Danske Lægers Vaccinations
                Service’
              </li>
            </ul>
          </div>

          <div>
            <p>PRAKTISK</p>
            <ul>
              <li>
                Infobreve o opholdet inden afrejse (med bl.a. pakkeliste,
                rejsetips, praktisk, etc.)
              </li>
              <li>
                Afrejsemøde ca. 5 uger inden afrejse (du møder dine rejsevenner
                og rejseleder)
              </li>
              <li>Dansk rejseleder på hele opholdet</li>
              <li>Undervisning af engagerede, dygtige og danske undervisere</li>
              <li>Højskolebevis (kan bruges til kvote 2)</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="lg:col-start-1">
        <p class="preh2">IKKE EN DEL AF PAKKEN</p>
            <h3>IKKE INKLUDERET</h3>
            


        <div class="grid inner_spacing mt-10">
          <div>
            <p>OVERORDNET</p>
            <ul>
              <li>Lommepenge</li>
              <li>Indkvartering i New York, Caribien, Mexico og Hawaii</li>
              <li>Mad & Drikke</li>
              <li>Rejseforsikring (+ evt. afbestillingsforsikring)</li>
              <li>Visum</li>
              <li>Vaccinationer</li>
              <li>Friuger</li>
            </ul>
          </div>

          <div>
            <p>SAMLET ESTIMAT</p>
            <ul>
              <li>
                Tidligere elever har samlet brugt ca. 30.000 DKK til 40.000 DKK
                undervejs på opholdet.
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </section>
  <section class="flex justify-end px-4">
    <MyButton type="linkbutton"> PROGRAM <svg class="m-auto" width="18" height="16" viewBox="0 0 18 16" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M17.7071 8.70711C18.0976 8.31658 18.0976 7.68342 17.7071 7.29289L11.3431 0.928932C10.9526 0.538408 10.3195 0.538408 9.92893 0.928932C9.53841 1.31946 9.53841 1.95262 9.92893 2.34315L15.5858 8L9.92893 13.6569C9.53841 14.0474 9.53841 14.6805 9.92893 15.0711C10.3195 15.4616 10.9526 15.4616 11.3431 15.0711L17.7071 8.70711ZM17 7L-4.76837e-07 7V9L17 9V7Z" fill="#929292"/>
      </svg> </MyButton> 
  </section>
</main>

<style>
  main {
    background-image: url(src/_icons/gurfers.png);
    background-position: cover;
    background-size: 280%;
    background-repeat: no-repeat;
    background-position-y: 60%;
  }
  section {
    padding-top: var(--padding-sections);
    padding-bottom: var(--padding-sections);
  }

  .inkl p {
    color: var(--txtcolor-700);
  }

  li {
    list-style: inside;
    line-height: var(--line-xl);
    font-family: "lato", sans-serif;
    color: var(--txtcolor-600);
  }
  #no-pad {
    padding-top: 0;
  }

  .inner_spacing {
    gap: var(--spacing-20);
  }

  img {
    width: 70px;
  }

  .inkluderet {
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 20px;
  }
</style>
