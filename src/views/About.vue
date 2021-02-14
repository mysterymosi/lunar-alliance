<template>
  <div class="about">
    <TheHeader />
    <div class="page-hero-section bg-image hero-mini">
      <div class="overlay"></div>
      <div class="hero-caption">
        <div class="container fg-white h-100">
          <div class="row justify-content-center align-items-center text-center h-100">
            <div class="col-lg-6">
              <h3 class="mb-4 fw-medium">About Us</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="page-section pt-5">
      <div class="container-fluid">
        <div class="row justify-content-center">
          <div class="col-lg-8">
            <div class="card-page">
              <h5 class="fg-primary">About Us</h5>
              <hr>
              <p>Lunar Alliance, founded in 2015, CI is a trading platform managed by a private trader, Mr. Wesley Hargraves, who trades mostly Cryptocurrency. Mr. Wesley Hargraves has been trading for more than 6 years now and has a vast knowledge of the Crypto Online Market and Cryptocurrency Trading Investment. Lunar Alliance is being known for it's transparency and accountability of managing finance in the world of Cryptocurrency Trading Investment and Account Management. We had a breakthrough in the market during the middle of 2016.</p>
              <p>Lunar Alliance is a global market place for people to trade Currencies, Commodities, Indices and CFD Stock online in a simple and transparent way. Our goal is to make trading accessible to all investors regardless of age, location, investment, technical knowledge or experience. Investing in Lunar Alliance involves the Daily Packages where profits are paid directly to our client's wallet every day, Weekly Packages where profits are paid directly to our client's wallet every week, the Monthly Compounding Investments and the NFP.</p>
              <p>The company is successful thanks to the big amount of profitable trades and some of the best specialists. We are existing on the market since 2015 and still give our investors significant profits till now. There are no unrealistic promises presented here, just steady and consistent results with the best possible and achievable returns at minimun risk.</p>
              <p>We believe every client is different and requires a unique approach. Our mission is to help people navigate through changing market conditions and several kinds of investment opportunities in order to find a strategic plan that best fits their trading goals.</p>
            </div>
            <div class="page-section no-scroll">
                <h2 class="text-center wow fadeIn">Why Us?</h2>
                <div class="row justify-content-center mt-5">
                  <div class="col-lg-10">
                    <div class="row justify-content-center">
                      <div class="col-md-6 col-lg-4 py-3 wow fadeInLeft">
                        <div class="card card-body border-0 text-center shadow pt-5">
                          <div class="svg-icon mx-auto mb-4">
                            <i class="pe-7s-target is-large"></i>
                          </div>
                          <h5 class="fg-gray">Our Mission</h5>
                          <p class="fs-small">It is our mission to offer top notch services to all our traders. We offer strategic ideas to our clients, we also provide the best possible support for realizing individual investment ideas.</p>
                        </div>
                      </div>
                      <div class="col-md-6 col-lg-4 py-3 wow fadeInUp">
                        <div class="card card-body border-0 text-center shadow pt-5">
                          <div class="svg-icon mx-auto mb-4">
                            <i class="pe-7s-video is-large"></i>
                          </div>
                          <h5 class="fg-gray">Our Vision</h5>
                          <p class="fs-small">Our Vision, in line with Our Mission, is to carefully analyse each individual's financial situation and work with them in order to optimise results within their parameters.</p>
                        </div>
                      </div>
                      <div class="col-md-6 col-lg-4 py-3 wow fadeInRight">
                        <div class="card card-body border-0 text-center shadow pt-5">
                          <div class="svg-icon mx-auto mb-4">
                            <i class="pe-7s-rocket is-large"></i>
                          </div>
                          <h5 class="fg-gray">Our Goals</h5>
                          <p class="fs-small">Our core values of integrity and innovation are a keystone in us, as we always put the customer in the first place, and all efforts are centered on making him a successful and profitable investor.</p>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <TheFooter />
  </div>
</template>
<script>
// @ is an alias to /src
import TheHeader from "@/components/TheHeader.vue";
import TheFooter from "@/components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheFooter
  }
};
</script>
<style scoped>
.bg-image {
  background-image: url(../assets/img/meeting_1.jpg);
}

.is-large {
	font-size: 60px;
	color: #3d58f3;
}
</style>