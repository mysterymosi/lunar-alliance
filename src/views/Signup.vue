<template>
  <div class="page-hero-section bg-image hero-home-2">
    <div class="overlay"></div>
    <div class="hero-caption">
      <div class="container fg-white h-100">
        <div class="row align-items-center h-100">
          <div v-if="!isAddressForm" class="col-lg-10 d-lg-block wow fadeInUp mx-auto">
            <div class="form-title">
              <h3 class="text-center">Sign up</h3>
            </div>
            <div class="shadow floating-animate">
              <!-- <img src="../assets/img/app_showcase.svg" alt=""> -->
              <form>
                <div class="form-group">
                  <label class="control-label sr-only" for="name"></label>
                  <input v-model="user.name" id="name" type="text" name="name" placeholder="Name" class="form-control" required>
                </div>
                <div class="form-group">
                  <label class="control-label sr-only" for="email"></label>
                  <input v-model="user.email" id="email" type="email" name="email" placeholder="Email" class="form-control" required>
                </div>
                <div class="row">
                  <div class="col-lg-6">
                    <div class="form-group">
                      <label class="control-label sr-only" for="phone"></label>
                      <input v-model="user.phone" id="phone" type="tel" placeholder="Phone number" class="form-control" required>
                    </div>
                  </div>
                  <div class="col-lg-6">
                    <div class="form-group">
                      <label class="control-label sr-only" for="ssn"></label>
                      <input v-model="user.ssn" id="ssn" type="text" placeholder="SSN" class="form-control" required>
                    </div>
                  </div>
                </div>
                <div class="row">
                  <div class="col-lg-6">
                    <div class="form-group">
                      <select class="form-control" v-model="user.security_question">
                        <option v-for="(option, index) in options" :key="index">{{ option }}</option>
                      </select>
                    </div>
                  </div>
                  <div class="col-lg-6">
                    <div class="form-group">
                      <label class="control-label sr-only" for="answer"></label>
                      <input v-model="user.answer" id="answer" type="text" placeholder="Answer" class="form-control" required>
                    </div>
                  </div>
                </div>
                <div class="form-group">
                  <label class="control-label sr-only" for="password"></label>
                  <input v-model="user.password" id="password" type="password" placeholder="password" class="form-control" required>
                </div>
                <div class="form-group">
                  <label class="control-label sr-only" for="confirm_password"></label>
                  <input v-model="user.confirm_password" id="confirm_password" type="password" placeholder="Confirm password" class="form-control" required>
                </div>
                <button @click.prevent="showAddressForm" class="btn btn-dark">Next</button>
              </form>
            </div>
            <p class="text-white mt-5">Not a member? <router-link to="/signup" class="text-yellow">Sign up</router-link><span class="pull-right">
                <router-link to="/" class="text-white">Back to Home</router-link>
              </span></p>
          </div>
          <AddressForm @goback="closeAddressForm" v-else/>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import AddressForm from "@/components/AddressForm.vue"
export default {
  components: {
    AddressForm
  },
  data() {
    return {
      user: {
        email: null,
        password: null
      },

      options: ["beans", "food"],
      isAddressForm: false
    }
  },

  methods: {
    showAddressForm() {
      this.isAddressForm = true;
    },

    closeAddressForm() {
      this.isAddressForm = false;
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