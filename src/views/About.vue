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
              <h5 class="fg-primary text-center">WHO WE SERVE</h5>
              <hr>
              <p>We help over 32 million people feel more confident in their most important financial goals, manage employee benefit programs for over 22,000 businesses, and support more than 13,000 financial institutions with innovative cryptocurrency investment and technology solutions to grow their businesses.</p>
              <p>Our diverse businesses and independence give us insight into the entire market and the stability needed to think and act for the long term as we deliver value to you.</p>
            </div>

            <div class="card-page mt-5">
              <h5 class="fg-primary text-center">DIVERSITY AND INCLUSION</h5>
              <hr>
              <p>We know that a diverse and inclusive workforce is the key to creating a relevant and differentiated customer experience. Building a connected and collaborative workforce that reflects the broader society will help us help our customers.</p>
            </div>

            <div class="card-page mt-5">
              <h5 class="fg-primary text-center">CORPORATE SPONSORSHIP</h5>
              <hr>
              <p>Fidelity partners with organizations that do good work locally and nationally, support shared corporate and community goals, and provide opportunities to strengthen relationships with key stakeholders.</p>
            </div>

            <div class="card-page mt-5">
              <h5 class="fg-primary text-center">SUSTAINABILITY</h5>
              <hr>
              <p>We foster innovation to achieve positive environmental change, while empowering customers, associates, and communities to reduce our global footprint.</p>
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

hr {
  width: 200px;
  border-top: 1px solid #3D58F3;
  margin: 1rem auto;
}
</style>