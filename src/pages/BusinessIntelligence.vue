<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <section class="content-block fullpage">
        <div v-parallax="0.4" class="cover-image tinted"></div>
        <div class="container">
          <div class="row">
            <div @click="scrollDown" class="show-more">
              <svg
                fill="#fff"
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
            <div class="column col-2 no-content"></div>
            <div class="column col-4 responsive-8 responsive-12 center-content">
              <ServiceHeader
                title="Business Intelligence"
                kicker="In BI consulting, smart decisions start with your data."
              />
            </div>
          </div>
        </div>
      </section>
      <section id="first" class="content-block">
        <div class="container">
          <ServicePromise
            title="Business Intelligence"
            content="Regardless of where you store your data, we can leverage your existing investments in SQL, SharePoint, Office 365, Dynamics 365, and Microsoft Office to provide cost-effective solutions. With the latest tools and self-service functionality, you don’t have heavy upfront costs or need continuous IT involvement. As a Microsoft Partner, we consult on the use of Microsoft Power BI, SQL Server Reporting Services (SSRS), and custom-developed .NET & SQL tools. We also have a team of developers capable of integrating diverse databases, web services, and third-party platforms."
          />
          <Spacer/>
          <div class="row">
            <div class="column col-12 center-horizontal">
              <h1 class="section-header">Business Intelligence Services</h1>
            </div>
          </div>
          <div class="row padded-bottom">
            <div class="column col-12">
              <div class="content-wrapper services-wrapper">
                <SubService
                  title="Data Discovery, Warehousing and ETL"
                  content="Mapping out and integrating data sources that are most appropriate for your BI objectives, building up a warehouse, and getting your data ready for analysis."
                />
                <SubService
                  title="BI Audit: Data Analytics and Data Systems Review"
                  content="The BI Audit provides assurances that our clients are getting the most out of their deployments and are following best practices, ensuring efficiency."
                />
                <SubService
                  title="Reporting and Interactive Dashboards"
                  content="Delivering customizable, interactive reporting dashboards that will serve as convenient go-to tools with minimum adoption barriers even for non-tech users."
                />
                <SubService
                  title="OLAP and Data Visualization"
                  content="Translating analy­tical work into an organized, precise format, on robust dashboards with scalable back-ends."
                />
                <SubService
                  title="Mobile Business Intelligence"
                  content="Bringing the power of business intelligence to mobile platforms of your choice wherever and whenever you need it."
                />
                <SubService
                  title="Analytics and Reporting"
                  content="Measure business goals through automated reporting,	create ad-hoc or predefined reports and facilitate fast decision making."
                />
                <SubService
                  title="Predictive Analysis"
                  content="Predict trends through intuitive tools that utilize a historical view of business data. Protect margins through data-driven forecasting."
                />
              </div>
            </div>
          </div>
        </div>
      </section>
      <ServiceStack title="BI Stack"></ServiceStack>
      <WorkTogether/>
    </div>
  </div>
</template>

<script>
import NavBarWhite from "../components/NavBarWhite.vue";
import ModalMenu from "../components/ModalMenu.vue";
import ServiceHeader from "../components/ServiceHeader.vue";
import ServicePromise from "../components/ServicePromise.vue";
import Spacer from "../components/Spacer.vue";
import SubService from "../components/SubService.vue";
import ServiceAsideRight from "../components/ServiceAsideRight.vue";
import ServiceAsideLeft from "../components/ServiceAsideLeft.vue";
import ServiceLeft from "../components/ServiceLeft.vue";
import ServiceRight from "../components/ServiceRight.vue";
import ServiceApproach from "../components/ServiceApproach.vue";
import SubApproach from "../components/SubApproach.vue";
import WorkTogether from "../components/WorkTogether.vue";
import ServiceStack from "../components/ServiceStack.vue";

export default {
  name: "BusinessIntelligence",
  components: {
    NavBarWhite,
    ModalMenu,
    Spacer,
    ServiceHeader,
    ServicePromise,
    SubService,
    ServiceAsideRight,
    ServiceAsideLeft,
    ServiceLeft,
    ServiceRight,
    ServiceApproach,
    SubApproach,
    WorkTogether,
    ServiceStack
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
  background-image: url(../assets/background/insights/insight-1large.jpg)
  filter: brightness(0.35) contrast(1) sepia(100%) hue-rotate(140deg) saturate(6)

.reg-link
  margin: 20px 0 0
</style>
