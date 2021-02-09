<template>
  <div class="page-hero-section bg-image hero-home-2">
    <div class="overlay"></div>
    <div class="hero-caption">
      <div class="container fg-white h-100">
        <div class="row align-items-center h-100">
          <div class="col-lg-6 d-lg-block wow fadeInUp mx-auto">
          	<div class="form-title">
          		<h3 class="text-center">Sign in</h3>
          	</div>
            <div class="img-place mobile-preview1 shadow floating-animate">
              <!-- <img src="../assets/img/app_showcase.svg" alt=""> -->
              <form>
                <div class="form-group">
                  <label class="control-label sr-only" for="email"></label>
                  <input v-model="user.email" id="email" type="text" name="email" placeholder="Email" class="form-control" required>
                </div>
                <div class="form-group">
                  <label class="control-label sr-only" for="password"></label>
                  <input v-model="user.password" id="password" type="password" name="password" placeholder="password" class="form-control" required>
                </div>
                <button class="btn btn-dark">Login</button>
              </form>
            </div>
            <p class="text-white mt-5">Not a member? <router-link to="/signup" class="text-yellow">Sign up</router-link><span class="pull-right"><router-link to="/" class="text-white">Back to Home</router-link> </span></p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      user: {
        email: null,
        password: null
      }
    }
  }
}
</script>
<style scoped>
.bg-image {
  background-image: url(../assets/img/deal_1.jpg);
}

.form-control {
	background: transparent;
	border-top: none;
	border-left: none;
	border-right: none;
	border-bottom: 2px solid #3D58F3;
	box-shadow: none;
}

.form-control:focus {
	background: transparent;
	border-top: none;
	border-left: none;
	border-right: none;
	border-bottom: 2px solid #3D58F3;
	box-shadow: none;
}

::placeholder {
	color: #ffffff;
}

.overlay {
	background: rgba(0, 0, 0, 0.75);
}

.mobile-preview1 {
  width: 100%;
  height: auto;
  border-radius: 30px;
}

.hero-home-2 .mobile-preview1 {
  border-radius: 40px;
}
</style>