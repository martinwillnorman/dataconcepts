<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <section class="content-block fullpage">
        <div v-parallax="0.4" class="cover-image tinted"></div>
        <div class="container">
          <div class="row">
            <div class="column col-3 no-content"></div>
            <div class="column col-8 responsive-12">
              <div class="content-wrapper header__content">
                <h1
                  data-aos="fade-up"
                  data-aos-duration="900"
                >Here's a little insight into what we do</h1>
              </div>
            </div>
            <div @click="scrollDown" class="show-more">
              <svg
                fill="#000"
                version="1.1"
                id="Ebene_2_1_"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                x="0px"
                y="0px"
                width="53px"
                height="20px"
                viewBox="0 0 53 20"
                enable-background="new 0 0 53 20"
                xml:space="preserve"
              >
                <g>
                  <polygon
                    points="26.5,17.688 9.114,3.779 10.303,2.312 26.5,15.269 42.697,2.313 43.886,3.779 	"
                  ></polygon>
                </g>
              </svg>
            </div>
          </div>
        </div>
      </section>
      <section class="content-block intruding">
        <div class="container">
          <div class="row">
            <div class="column col-4 responsive-8 responsive">
              <div
                data-aos="fade-in"
                data-aos-duration="900"
                class="content-wrapper intruding-kicker"
              >
                <h3>Share Knowledge</h3>
                <p>We think it's important to provide our clients with key insights into the solutions that could help your business succeed.</p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <Spacer/>
        </div>
      </section>
      <section id="first" class="content-block grey">
        <div class="container">
          <div class="row">
            <div class="column col-12">
              <div class="content-wrapper insights-wrapper">
                <Insight
                  link="/insights/quick-peek"
                  category="Data"
                  title="A Quick Peek At Our World Helping Clients with Data Strategy"
                  summary="Every business and organisation has its own unique set of goals, KPIs and targets, and we believe that everything that we do should be devised, planned and executed with these objectives in mind."
                ></Insight>
                <Insight
                  link="/insights/blockchain-world"
                  category="Blockchain"
                  title="Our Insights on the World of Blockchain"
                  summary="Blockchain is one of the most dynamic inventions of this century. Though this revolutionary technology is still in its infancy, it has the potential to disrupt almost every industry and to change how the world works."
                ></Insight>
                <Insight
                  link="/insights/data-mining"
                  category="Big Data"
                  title="Extracting Actionable Insights from Data"
                  summary="Data mining is the extraction of actionable insights from data."
                ></Insight>
                <Insight
                  link="/insights/analytics-is-popular"
                  category="Data & Analytics"
                  title="The Popularity of Analytics"
                  summary="Ten imperatives for successfully developing an analytics capability."
                ></Insight>
                <Insight
                  link="/insights/modern-utility"
                  category="IoT"
                  title="The Needs of Modern Utility Consumers"
                  summary="The digital era has ushered in the trend of information being available at fingertips on-demand."
                ></Insight>
                <Insight
                  link="/insights/azure-machine-learning"
                  category="Machine Learning"
                  title="5 Reasons Why We Love Azure ML for Machine Learning Solutions"
                  summary="From virtual assistants to chatbots and automation to smart homes, Artificial Intelligent (AI) and Machine Learning have become prominent in our daily life."
                ></Insight>
                <Insight
                  link="/insights/agile-transformation"
                  category="Agile"
                  title="Agile Transformation: It's a New Way of Thinking!"
                  summary="Many of the world’s biggest companies struggle to be nimble, efficient, and data-driven, which then makes them less productive than they should be."
                ></Insight>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import NavBarWhite from "../components/NavBarWhite.vue";
import ModalMenu from "../components/ModalMenu.vue";
import Spacer from "../components/Spacer.vue";
import Insight from "../components/Insight.vue";

export default {
  name: "Insights",
  components: {
    NavBarWhite,
    ModalMenu,
    Spacer,
    Insight
  },
  methods: {
    scrollDown() {
      document.getElementById("first").scrollIntoView({
        behavior: "smooth",
        block: "start"
      });
    }
  }
};
</script>

<style lang="sass" scoped>
@import "../assets/sass/settings.sass"

.cover-image
  filter: brightness(0.7) contrast(1.2) sepia(100%) hue-rotate(160deg) saturate(3.5)
  background-image: url(../assets/background/insights/insight-1large.jpg)

.insights-wrapper
  display: flex
  flex-wrap: wrap
  padding-top: 100px

@media only screen and (max-width: 450px)
  .insights-wrapper
    padding-top: 60px

</style>



