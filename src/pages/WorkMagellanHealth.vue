<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <Hero title="Magellan Health" kicker="Single Sign On.">
        <div v-parallax="0.4" class="cover-image hero-background tinted"></div>
      </Hero>

      <section class="content-block" id="first">
        <div class="container">
          <WorkSummary
            content="Our client provides innovative, integrated healthcare to one out of every ten Americans by delivering behavioral health and employee assistance program services; specialty health, including musculoskeletal, cardiac, advanced imaging management and physical medicine; and integrated care management to health plans, employers, Medicaid, Medicare and the Federal government."
          />
          <Spacer/>
          <WorkRole>
            <li>Java</li>
            <li>JEE</li>
            <li>OpenIG</li>
            <li>ADFS</li>
            <li>Oauth</li>
            <li>SSO</li>
            <li>SAML</li>
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
            >Magellan was in the process of replacing its existing authentication solutions that were implemented using CAS, F5 authentication and WebLogic authentication with a Microsoft AEGIS solution. Magellan was also in the process of replacing its identity repository – Novell eDirectory with the Active Directory platform. The migration of users from eDirectory to Active Directory as well as the replacement of its authentication solution with AEGIS, required modifications and enhancements to the existing Java applications that were currently reliant on the legacy platform.</p>
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
            >A SEAMLESSLY DESIGNED SINGLE SIGN ON</p>
          </WorkSolutionHeader>
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <WorkSolution>
            <p data-aos="fade-up" data-aos-duration="600">
              Data Concepts implemented an Enterprise Single Sign On [SSO] and Centralized Identity Management and Governance solution for all existing Java/JEE based applications in production.
              Data Concepts migrated over 33 Java web applications to the new platform based on Microsoft AEGIS solution. The team designed, developed and tested to integrate a multitude of web applications on the new platform.
            </p>
            <ul data-aos="fade-up" data-aos-duration="600" data-aos-delay="100">
              <li>- Migration of existing authentication solution.</li>
              <li>- Replacing identity repository with Active Directorys.</li>
              <li>- Enhanced existing Java-based applications in a production environment.</li>
              <li>- Implementation of an enterprise-wise SSO with strict Governance rules.</li>
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
            >Data Concepts replaced Magellan Health’s authentication solution and successfully replaced its identity repository. Data Concepts enhanced and rewrote many Java-based applications. This was a deliverable based, fixed price project.</p>
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
  name: "WorkMagellanHealth",
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
  background-image: url(../assets/background/work-large/magellan-health.jpg)
  background-position: center


#first
    background-color: #ca0853

.challenge-header
    font:
        size: 1.8rem
    color: #ca0853
    margin-bottom: 30px

.outcome-header
    font:
        size: 2rem
        weight: 600
    letter-spacing: 4px
    color: #ca0853

.solution-header:after
    background-color: #ca0853

</style>