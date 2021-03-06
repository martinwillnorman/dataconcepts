<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <Hero title="Virginia State Police" kicker="Sex Offender Registry.">
        <div v-parallax="0.4" class="cover-image hero-background tinted"></div>
      </Hero>

      <section class="content-block" id="first">
        <div class="container">
          <WorkSummary
            content="Virginia State Police [VSP] is a statewide law enforcement agency for the Commonwealth of Virginia."
          />
          <Spacer/>
          <WorkRole>
            <li>Portal Development</li>
            <li>Web Services</li>
            <li>JavaScript</li>
            <li>XML</li>
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
            >VSP owns and maintains the Sex Offender Registry [SOR] public website for the Commonwealth of Virginia. VSP awarded Data Concepts the entire project to redesign, rewrite and replace the Sex Offender Registry application with an elegant, flexible and user-friendly custom web portal for the citizens of the Commonwealth, so that they can have better control of searches, and develop their own customized views of information.</p>
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
            >A VITAL PUBLIC RESOURCE MADE USER-FRIENDLY</p>
          </WorkSolutionHeader>
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <WorkSolution>
            <p
              data-aos="fade-up"
              data-aos-duration="600"
            >Data Concepts redesigned and developed the new Sex Offender [SOR] Registry portal website based on VSP’s Requirements and integrated it with the existing SOR backend applications. Major functional additions in the portal included:</p>
            <ul data-aos="fade-up" data-aos-duration="600" data-aos-delay="100">
              <li>- Statewide Sex-Offender Notification.</li>
              <li>- Radius Offender Search.</li>
              <li>- Interface with Google Maps.</li>
              <li>- Map View.</li>
              <li>- Captcha.</li>
              <li>- Supports approximately 284 hits per second.</li>
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
            >The SOR application was dramatically enhanced in usability, features and sophistication, and was successfully deployed in production by Data Concepts.</p>
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
  name: "WorkVehicleInspection",
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

.hero-background
  background-image: url(../assets/background/work-large/sex-registry.jpg)
  background-position: center

#first
    background-color: #ffc200

.challenge-header
    font:
        size: 1.8rem
    color: #ffc200
    margin-bottom: 30px

.outcome-header
    font:
        size: 2rem
        weight: 600
    letter-spacing: 4px
    color: #ffc200

.solution-header:after
    background-color: #ffc200

</style>