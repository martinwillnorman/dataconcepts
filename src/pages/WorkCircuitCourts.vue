<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <Hero title="Virginia State Police" kicker="Legacy Modernization.">
        <div v-parallax="0.4" class="cover-image service-header-image tinted"></div>
      </Hero>

      <section class="content-block" id="first">
        <div class="container">
          <WorkSummary
            content="Virginia State Police [VSP] is a statewide law enforcement agency for the Commonwealth of Virginia."
          >
            <ul>
              <li>Javat</li>
              <li>JEE</li>
              <li>Spring</li>
              <li>Struts</li>
              <li>Hibernate</li>
              <li>DB2</li>
              <li>IBM WebSphere</li>
              <li>Angular</li>
              <li>React</li>
            </ul>
          </WorkSummary>
          <Spacer/>
          <WorkRole>
            <li>Javat</li>
            <li>JEE</li>
            <li>Spring</li>
            <li>Struts</li>
            <li>Hibernate</li>
            <li>DB2</li>
            <li>IBM WebSphere</li>
            <li>Angular</li>
            <li>React</li>
          </WorkRole>
        </div>
      </section>
      <section class="content-block black">
        <div class="container">
          <WorkChallenge>
            <h1 data-aos="fade-up" data-aos-duration="600" class="challenge-header">CHALLENGE</h1>
            <p
              data-aos="fade-up"
              data-aos-duration="600"
              data-aos-delay="100"
              class="text-white"
            >The Legacy Mainframe System needed to be converted into a Web-Based Case Management Application that would allow judicial users to manage all phases of case documents.</p>
          </WorkChallenge>
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <WorkSolutionHeader>
            <h1
              data-aos="fade-up"
              data-aos-duration="600"
              class="section-header solution-header"
            >SOLUTION</h1>
            <p
              data-aos="fade-up"
              data-aos-duration="600"
              data-aos-delay="100"
            >AN INTRICATE LEGACY MODERNIZATION INTO JAVA/JEE</p>
          </WorkSolutionHeader>
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <WorkSolution>
            <p
              data-aos="fade-up"
              data-aos-duration="600"
            >This was a high complexity, high risk large engagement completely managed and implemented by Data Concepts. It involved replacing a stable 20-year legacy system with a new web solution across the state.</p>
            <ul data-aos="fade-up" data-aos-duration="600" data-aos-delay="100">
              <li>- The Re-engineered system provided all business functions of the current legacy system while implementing additional improvements to increase productivity in courts.</li>
              <li>- Multilevel security controls for accessing non-public information such as Sealed Indictments.</li>
              <li>- Granular role-based security that scales to manage small, medium and large volume courts.</li>
              <li>- On-Demand Interactive Docket creation along other ad-hoc reporting capabilities.</li>
              <li>- Replace home grown services infrastructure with an industry solution based on open standards that provides both agility and flexibility.</li>
              <li>- Customizable reports that support a variety of document formats.</li>
              <li>- Comprehensive auditing capabilities to track any and all case inquiries and updates.</li>
            </ul>
          </WorkSolution>
        </div>
      </section>
      <section class="content-block light-grey">
        <div class="container">
          <WorkOutcome>
            <h1
              data-aos="fade-up"
              data-aos-duration="600"
              class="section-header medium outcome-header"
            >OUTCOME</h1>
            <p
              data-aos="fade-up"
              data-aos-duration="600"
              data-aos-delay="200"
            >Data Concepts managed and executed this complex, highly sensitive and critical modernization and successfully deployed the new web-based system.</p>
          </WorkOutcome>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import NavBarWhite from "../components/NavBarWhite.vue";
import ModalMenu from "../components/ModalMenu.vue";
import Spacer from "../components/Spacer.vue";
import Hero from "../components/Hero.vue";
import WorkSummary from "../components/WorkSummary.vue";
import WorkChallenge from "../components/WorkChallenge.vue";
import WorkRole from "../components/WorkRole.vue";
import WorkSolutionHeader from "../components/WorkSolutionHeader.vue";
import WorkSolution from "../components/WorkSolution.vue";
import WorkOutcome from "../components/WorkOutcome.vue";

export default {
  name: "WorkCircuitCourts",
  components: {
    NavBarWhite,
    ModalMenu,
    Spacer,
    Hero,
    WorkSummary,
    WorkChallenge,
    WorkRole,
    WorkSolutionHeader,
    WorkSolution,
    WorkOutcome
  }
};
</script>


<style lang="sass" scoped>
@import "../assets/sass/settings.sass"

.service-header-image
  background-image: url(../assets/background/work-large/circuit-courts.jpg)
  background-position: center

#first
    background-color: #FF2828

.challenge-header
    font:
        size: 1.8rem
    color: #FF2828
    margin-bottom: 30px

.outcome-header
    font:
        size: 2rem
        weight: 600
    letter-spacing: 4px
    color: #FF2828

.solution-header:after
    background-color: #FF2828

</style>