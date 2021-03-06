<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <Hero title="Moonlighting" kicker="Jobs Portal.">
        <div v-parallax="0.4" class="cover-image hero-background tinted"></div>
      </Hero>

      <section class="content-block" id="first">
        <div class="container">
          <WorkSummary
            content="Data Concepts’ client is one of the fastest growing on-demand marketplaces in the burgeoning gig economy. Moonlighting lets everyone participate in the new “on-demand economy” and collaborate to create and fill jobs in every state across United States."
          />
          <Spacer/>
          <WorkRole>
            <li>RESTful API</li>
            <li>Mobile Integration</li>
            <li>Portal Development</li>
            <li>Java</li>
            <li>AWS</li>
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
            >Our client sought to simplify the hiring process for individuals and small businesses and eliminate the anonymity of posting jobs and sharing favorite hires within trusted social networks like Facebook, Instagram, and LinkedIn.</p>
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
            >A DIGITAL SPACE FOR SEEKERS TO MEET</p>
          </WorkSolutionHeader>
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <WorkSolution>
            <p
              data-aos="fade-up"
              data-aos-duration="600"
            >Our client required a highly available, full featured, highly responsive and scalable enterprise web portal to meet their growing needs. The following solution was proposed:</p>
            <ul data-aos="fade-up" data-aos-duration="600" data-aos-delay="100">
              <li>- Develop the backend RESTful API(s)/Services for delivering consistent data across multiple interfaces such as Web and Mobile apps (Android & IOS).</li>
              <li>- Develop a responsive customer facing web portal by implementing critical requirements like view & filter by location, job application functionality, the ability to add new services, generate proposals and invoices, make payments, view and manage job feedback, real time job alerts and notifications.</li>
              <li>- Develop an Enterprise web portal using Java with the latest technologies such as Angularjs, Bootstrap, Spring Framework, Spring RESTful services, Spring Security, Spring Batch, Spring Data, MongoDB.</li>
              <li>- Provide high availability and scalability by deploying the API/Services backend and Angular web applications on Pivotal and Amazon cloud environments.</li>
              <li>- For deployment automation, use Maven to generate enterprise application archive files and integrate it with Jenkins for build automation and continuous integration.</li>
              <li>- Leverage big data technologies for rapidly growing volumes of data and users and employ the AWS cloud platform for fast scaling and speed to market.</li>
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
            >The MVP (Minimum Viable Product) was delivered to production within two months. The portal was key in generating 30K new Jobs and 20K new users in first six months.</p>
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
  background-image: url(../assets/background/work-large/moonlighting.jpg)
  background-position: center

#first
    background-color: #426EFF

.challenge-header
    font:
        size: 1.8rem
    color: #426EFF
    margin-bottom: 30px

.outcome-header
    font:
        size: 2rem
        weight: 600
    letter-spacing: 4px
    color: #426EFF

.solution-header:after
    background-color: #426EFF

</style>