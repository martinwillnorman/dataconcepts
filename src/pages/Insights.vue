<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBarWhite/>
    <div class="sections">
      <section class="content-block fullpage">
        <div class="show-more"></div>
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
            <div class="column col-12 responsive">
              <div class="content-wrapper intruding-kicker-arrow-holder">
                <svg
                  data-aos="fade-in"
                  data-aos-duration="900"
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
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <div class="row">
            <div class="column col-12">
              <div class="spacer"></div>
            </div>
          </div>
        </div>
      </section>
      <section class="content-block">
        <div class="container">
          <div class="row">
            <div class="column col-12">
              <div class="content-wrapper insights-wrapper">
                <div
                  class="insight"
                  data-aos="fade-up"
                  data-aos-delay="100"
                  data-aos-duration="900"
                >
                  <router-link class="insight-link" to="/insights">
                    <img src="../assets/logo/cloud-computing.svg" alt="logo">
                    <h3>Understanding What It Means To Be Agile</h3>
                    <p>Agile, as it relates to project management for software development, is sometimes used as synonym for Scrum, Kanban or other type of framework..
                      <br>
                      <br>
                      <span>Read More</span>
                    </p>
                  </router-link>
                </div>
                <div
                  class="insight"
                  data-aos="fade-up"
                  data-aos-delay="200"
                  data-aos-duration="900"
                >
                  <router-link class="insight-link" to="/insights">
                    <img src="../assets/logo/cloud-computing (2).svg" alt="logo">
                    <h3>Understanding What It Means To Be Agile</h3>
                    <p>Agile, as it relates to project management for software development, is sometimes used as synonym for Scrum, Kanban or other type of framework..
                      <br>
                      <br>
                      <span>Read More</span>
                    </p>
                  </router-link>
                </div>
                <div
                  class="insight"
                  data-aos="fade-up"
                  data-aos-delay="400"
                  data-aos-duration="900"
                >
                  <router-link class="insight-link" to="/insights">
                    <img src="../assets/logo/cloud-computing (3).svg" alt="logo">
                    <h3>Understanding What It Means To Be Agile</h3>
                    <p>Agile, as it relates to project management for software development, is sometimes used as synonym for Scrum, Kanban or other type of framework..
                      <br>
                      <br>
                      <span>Read More</span>
                    </p>
                  </router-link>
                </div>
                <div
                  class="insight"
                  data-aos="fade-up"
                  data-aos-delay="100"
                  data-aos-duration="900"
                >
                  <router-link class="insight-link" to="/insights">
                    <img src="../assets/logo/cloud-computing.svg" alt="logo">
                    <h3>Understanding What It Means To Be Agile</h3>
                    <p>Agile, as it relates to project management for software development, is sometimes used as synonym for Scrum, Kanban or other type of framework..
                      <br>
                      <br>
                      <span>Read More</span>
                    </p>
                  </router-link>
                </div>
                <div
                  class="insight"
                  data-aos="fade-up"
                  data-aos-delay="200"
                  data-aos-duration="900"
                >
                  <router-link class="insight-link" to="/insights">
                    <img src="../assets/logo/cloud-computing (2).svg" alt="logo">
                    <h3>Understanding What It Means To Be Agile</h3>
                    <p>Agile, as it relates to project management for software development, is sometimes used as synonym for Scrum, Kanban or other type of framework..
                      <br>
                      <br>
                      <span>Read More</span>
                    </p>
                  </router-link>
                </div>
                <div
                  class="insight"
                  data-aos="fade-up"
                  data-aos-delay="400"
                  data-aos-duration="900"
                >
                  <router-link class="insight-link" to="/insights">
                    <img src="../assets/logo/cloud-computing (3).svg" alt="logo">
                    <h3>Understanding What It Means To Be Agile</h3>
                    <p>Agile, as it relates to project management for software development, is sometimes used as synonym for Scrum, Kanban or other type of framework..
                      <br>
                      <br>
                      <span>Read More</span>
                    </p>
                  </router-link>
                </div>
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

export default {
  name: "Insights",
  components: {
    NavBarWhite,
    ModalMenu
  }
};
</script>

<style lang="sass" scoped>
@import "../assets/sass/settings.sass"

.cover-image
  background-image: url(../assets/background/insights/insight-1large.jpg)
  filter: brightness(0.7) contrast(1.2) sepia(100%) hue-rotate(160deg) saturate(3.5)

.insights-wrapper
  display: flex
  flex-wrap: wrap

.insight
  flex-basis: 33.3333%
  width: 33.3333%
  max-width: 33.3333%
  padding-bottom: 100px

.insight-link
  display: flex
  flex-direction: column
  padding: 20px
  position: relative
  transition: box-shadow 200ms cubic-bezier(.29,.29,.42,1.01)

.insight-link h3
  color: $font-c-1
  line-height: 1.4

.insight-link p
  color: $font-c-p-2

img
  height: 40px
  width: 40px

span
  color: $font-c-1

.insight-link::after
  content: ""
  position: absolute
  top: -10px
  left: 0
  height: 1px
  width: 100%
  transform: translatey(10px)
  background: $dataconcepts-red
  opacity: 0
  transition: transform 400ms cubic-bezier(.29,.29,.42,1.01), opacity 600ms ease-in-out, color 600ms ease-in-out

.insight-link:hover:after 
  opacity: 1  
  transform: translatey(2px)

.insight-link:hover
  box-shadow: 0px 0px 40px rgba(0,0,0,.1)

@media only screen and (max-width: 1000px)
  .insight
    flex-basis: 50%
    width: 50%
    max-width: 50%
  .insight-link
    padding: 10px

@media only screen and (max-width: 678px)
  .insight
    flex-basis: 100%
    width: 100%
    max-width: 100%
  .insight-link
    padding: 5

</style>



