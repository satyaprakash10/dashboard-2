<template>
  <div>
    <div class="container-fluid seconadary">
      <nav aria-label="breadcrumb">
          <!-- <div> -->
            <div>
              <h1 class="title-2">FormPage</h1>
              <ul class="lists-2">
                <li><a href="#" class="home">  Home</a></li>
                <li><a href="#" class="db">  >  Profile</a></li>
              </ul>
            </div>
              <!-- <button class="btn btn-danger upgradebtn">Upgrade to pro</button> -->
          <!-- </div> -->
      </nav>
    </div>
    <div class="sub-section mt-5 ">
        <div class="container"  >
          <div class="row">
              <div class="col-md-12">
                <div class="card-header bg-white mt-4">
                  <h1 style="font-size:30px;">Vuelidate - Form  </h1> <hr> <span class="span-style">Registration page for your work</span>
                  <div>
                    </div>
                      <form @submit.prevent="handleSubmit" style="margin-top:20px;">
                        <div class="card bg-grey">
                          <div class="form-group">
                              <label for="firstName" style="font-size:20px;">First Name</label>
                              <input type="text" v-model="user.firstName" id="firstName" name="firstName" class="form-control" :class="{ 'is-invalid': submitted && $v.user.firstName.$error }" />
                              <div v-if="submitted && !$v.user.firstName.required" class="invalid-feedback">First Name is required</div>
                          </div>
                          <div class="form-group">
                              <label for="lastName" style="font-size:20px;">Last Name</label>
                              <input type="text" v-model="user.lastName" id="lastName" name="lastName" class="form-control" :class="{ 'is-invalid': submitted && $v.user.lastName.$error }" />
                              <div v-if="submitted && !$v.user.lastName.required" class="invalid-feedback">Last Name is required</div>
                          </div>
                          <div class="form-group">
                              <label for="email" style="font-size:20px;">Email</label>
                              <input type="email" v-model="user.email" id="email" name="email" class="form-control" :class="{ 'is-invalid': submitted && $v.user.email.$error }" />
                              <div v-if="submitted && $v.user.email.$error" class="invalid-feedback">
                                  <span v-if="!$v.user.email.required">Email is required</span>
                                  <span v-if="!$v.user.email.email">Email is invalid</span>
                              </div>
                          </div>
                          <div class="form-group">
                              <label for="password" style="font-size:20px;">Password</label>
                              <input type="password" v-model="user.password" id="password" name="password" class="form-control" :class="{ 'is-invalid': submitted && $v.user.password.$error }" />
                              <div v-if="submitted && $v.user.password.$error" class="invalid-feedback">
                                  <span v-if="!$v.user.password.required">Password is required</span>
                                  <span v-if="!$v.user.password.minLength">Password must be at least 6 characters</span>
                              </div>
                          </div>
                          <div class="form-group">
                              <label for="confirmPassword" style="font-size:20px;">Confirm Password</label>
                              <input type="password" v-model="user.confirmPassword" id="confirmPassword" name="confirmPassword" class="form-control" :class="{ 'is-invalid': submitted && $v.user.confirmPassword.$error }" />
                              <div v-if="submitted && $v.user.confirmPassword.$error" class="invalid-feedback">
                                  <span v-if="!$v.user.confirmPassword.required">Confirm Password is required</span>
                                  <span v-else-if="!$v.user.confirmPassword.sameAsPassword">Passwords must match</span>
                              </div>
                          </div>
                          <div class="form-group">
                              <button class="btn btn-primary "style="font-size:20px;">Register</button>
                          </div>

                        </div>
                      </form>
                  </div>
              </div>
          </div>
     </div>
  </div>
</div> 
</template>

<script>
    import { required, email, minLength, sameAs } from "vuelidate/lib/validators";

    export default {
        name: "app",
        data() {
            return {
                user: {
                    firstName: "",
                    lastName: "",
                    email: "",
                    password: "",
                    confirmPassword: ""
                },
                submitted: false
            };
        },
        validations: {
            user: {
                firstName: { required },
                lastName: { required },
                email: { required, email },
                password: { required, minLength: minLength(6) },
                confirmPassword: { required, sameAsPassword: sameAs('password') }
            }
        },
        methods: {
            handleSubmit(e) {
                this.submitted = true;

                // stop here if form is invalid
                this.$v.$touch();
                if (this.$v.$invalid) {
                    return;
                }

                alert("SUCCESS!! :-)\n\n" + JSON.stringify(this.user));
            }
        }
    };
</script>

<style>
.sub-section  {
  position: relative;
  
}
.title-2 {
  margin-right: 919px;
  margin-top: 20px;
  font-size: 30px;
}
.seconadary {
  background:rgb(231, 224, 224);
  top: 0%;
  margin-top: -20px;
}
.lists-2 {
  list-style: none;
  padding-left: 255px;
  display: flex;
  text-decoration: none;
  font-size: 15px;
  flex-wrap: nowrap;
}
.home {
  color: rgb(79, 50, 211);
  padding-right: 10px;
}
.db {
  color: grey;
} 
.span-style {
  color: grey;
  font-size: 14px;
}
.form-group {
  background: rgb(250, 250, 250);
}
 @media screen and (max-width: 780px) {
   .title-2  {  
    margin-right: 100px;
   }
   .lists-2 {
     padding-left: 141px;
   }
 }
</style>