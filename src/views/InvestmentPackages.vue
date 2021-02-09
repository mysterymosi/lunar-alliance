<template>
  <div>
    <TheHeader />
    <div class="page-hero-section bg-image hero-mini">
    	<div class="overlay"></div>
      <div class="hero-caption">
        <div class="container fg-white h-100">
          <div class="row justify-content-center align-items-center text-center h-100">
            <div class="col-lg-6">
              <h3 class="mb-4 fw-medium">Investment Packages</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="page-section">
      <div class="container">
        <div class="pricing-table mt-5 wow fadeInUp">
          <div class="pricing-item active no-transform">
            <div class="pricing-header text-center">
              <h5 class="fw-normal">Daily Investment Package</h5>
              <h6>Bronze</h6>
            </div>
            <div class="pricing-body">
              <ul class="theme-list">
                <li class="list-item">Minimum Investment of $2500</li>
                <li class="list-item">Maximum Investment of $4999</li>
                <li class="list-item">RETURNS 1%</li>
                <li class="list-item">REFERRAL BONUS 5%</li>
              </ul>
            </div>
            <hr>
            <h6 class="text-center">Silver</h6>
            <div class="pricing-body">
              <ul class="theme-list">
                <li class="list-item">Minimum Investment of $2500</li>
                <li class="list-item">Maximum Investment of $4999</li>
                <li class="list-item">RETURNS 1%</li>
                <li class="list-item">REFERRAL BONUS 5%</li>
              </ul>
            </div>
            <hr>
            <h6 class="text-center">Gold</h6>
            <div class="pricing-body">
              <ul class="theme-list">
                <li class="list-item">Minimum Investment of $2500</li>
                <li class="list-item">Maximum Investment of $4999</li>
                <li class="list-item">RETURNS 1%</li>
                <li class="list-item">REFERRAL BONUS 5%</li>
              </ul>
            </div>
            <div class="pricing-btn text-center">
            	<button class="btn btn-dark">Choose Plan</button>
            </div>
          </div>
        </div>
        <div class="pricing-table mt-5 wow fadeInUp">
          <div class="pricing-item">
            <div class="pricing-header text-center">
            	<h5 class="fw-normal">Non-farm Payroll</h5>
              <h6>Platinum</h6>
            </div>
            <div class="pricing-body">
              <ul class="theme-list">
                <li class="list-item">Minimum Investment of $3,000</li>
                <li class="list-item">Maximum Investment of $1,000,000</li>
                <li class="list-item">Get monthly returns of up to 50% profit</li>
                <li class="list-item">Every first Saturday of the month is the payday for NFP</li>
                <!-- <li class="list-item">24/7 Support</li> -->
              </ul>
            </div>
            <div class="pricing-btn text-center">
            	<button class="btn btn-dark">Choose Plan</button>
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
	hr {
		border-color: #3d58f3 !important;
		width: 250px;
	}

	.bg-image {
		background-image: url(../assets/img/bitcoin-pocket_1.jpg);
	}
</style>