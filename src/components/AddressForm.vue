<template>
  <div class="col-lg-10 d-lg-block wow fadeInUp mx-auto">
    <div class="form-title">
      <h3 class="text-center">Enter additional info</h3>
    </div>
    <div class="shadow floating-animate">
      <form class="wow fadeInUp">
        <div class="form-group">
          <label class="control-label sr-only" for="address"></label>
          <input v-model="user.address" id="address" type="text" placeholder="Address" class="form-control" required>
        </div>
        <div class="form-group">
          <label class="control-label sr-only" for="city"></label>
          <input v-model="user.city" id="city" type="text" placeholder="City" class="form-control" required>
        </div>
        <div class="form-group">
          <label class="control-label sr-only" for="state"></label>
          <input v-model="user.state" id="state" type="text" placeholder="State" class="form-control" required>
        </div>
        <div class="form-group">
          <label class="control-label sr-only" for="country"></label>
          <input v-model="user.country" id="country" type="text" placeholder="Country" class="form-control" required>
        </div>
        <div class="form-group">
          <label class="control-label sr-only" for="zip"></label>
          <input v-model="user.zip" id="zip" type="text" placeholder="Zip" class="form-control" required>
        </div>
        <div class="d-flex justify-content-between">
          <button class="btn btn-dark">Next</button>
          <button @click.prevent="goBack" class="btn btn-dark">Back</button>
        </div>
      </form>
    </div>
    <p class="text-white mt-5">Not a member? <router-link to="/signup" class="text-yellow">Sign up</router-link><span class="pull-right">
        <router-link to="/" class="text-white">Back to Home</router-link>
      </span></p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      user: {
        address: null
      }
    }
  },

  methods: {
    goBack() {
      this.$emit("goback");
    }
  }
}
</script>
<style scoped>
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

.mobile-preview1 {
  width: 100%;
  height: auto;
  border-radius: 30px;
}

.hero-home-2 .mobile-preview1 {
  border-radius: 40px;
}
</style>