<template>
  <v-app>
    <v-content>
      <v-container class="fill-height"  fluid>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="8">
            <v-card class="elevation-12">
              <v-window v-model="step">
              <v-window-item :value="1">
                <v-row>
                  <v-col cols="12" md="7" class="grey lighten-4">
                    <v-card-text>
                      <h1 class="text-center display-1 primary--text mx-1 font-weight-bold" >Log in </h1>
                      <div class="text-center mt-3" >
                        <v-btn class="mx-1" shaped rounded color="cyan darken-2" outlined
                        width="150" height="50" >
                          <v-icon class="icon">fab fa-facebook-f</v-icon>
                          <!-- <h5>Facebook</h5> -->
                        </v-btn>

                        <v-btn class="mx-1" shaped rounded color="cyan darken-2" outlined
                        width="150" height="50">
                          <v-icon class="icon">fab fa-google</v-icon>
                          <!-- <h5 class="text-center">Google</h5> -->
                        </v-btn>
                      </div>
                      <v-divider class="mt-4 mx-1" width="97%" light></v-divider>

                      <v-form >
                        <v-text-field class="mt-4"
                        id="email"
                        label="Email"
                        name="Email"
                        type="text"
                        color="cyan darken-2"
                        rounded
                        outlined
                        
                        />

                        <v-text-field
                        id="password"
                        label="Password"
                        name="Password"
                        type="password"
                        color="cyan darken-2"
                        light
                        rounded
                        outlined/>
                        
                      </v-form>
                      <h3 class="text-end">Forgot your password?</h3>
                    </v-card-text>

                    <div class="text-center mt-4">
                      <v-btn  width="250" height="50" rounded color="cyan darken-2" dark to="/dashboard">Log in</v-btn>
                    </div>
                    <div class="text-center mt-4">
                      <v-btn outlined width="250" height="50" rounded color="cyan darken-2" dark>Continue as a guest</v-btn>
                    </div>

                    
                    
                  </v-col>

                  <v-col cols="12" md="5" class="cyan darken-2">
                    <h1 class="white--text text-start display-1 mt-5">Hello Friends,</h1>
                    <h5 class="white--text text-start mt-3">Enter your personal details and start journey with us</h5>
                    <v-img class="mt-5" src="../assets/login_clipart.png" height="300px" width="450px"></v-img>
                    <div class="text-center signup">
                      <v-btn outlined width="250" height="50" shaped rounded class="grey lighten-4 mt-6" color="cyan darken-2"  @click="step++">Signup</v-btn>
                    </div>
                  </v-col>
                </v-row>
              </v-window-item>

              <v-window-item :value="2">
                <v-row>
                  <v-col cols="12" md="5" class="cyan darken-2">
                    <h1 class="white--text text-start display-1 mt-5">Hello Friends,</h1>
                    <h5 class="white--text text-start mt-3">Already Have an Account?</h5>
                    <v-img class="mt-5" src="../assets/login_clipart.png" height="300px" width="450px"></v-img>
                    <div class="text-center signup">
                      <v-btn outlined width="250" height="50" shaped rounded class="grey lighten-4 mt-6" color="cyan darken-2"  @click="step--">Login</v-btn>
                    </div>
                  </v-col>
                  
                  <v-col cols="12" md="7" class="grey lighten-4">
                    <v-card-text>
                      <h1 class="text-center display-1 primary--text mx-1 font-weight-bold" >Create a Fixmy account</h1>
                      <div class="text-center mt-3" >
                        <v-btn class="mx-1" shaped rounded color="cyan darken-2" outlined
                        width="150" height="50" >
                          <v-icon class="icon">fab fa-facebook-f</v-icon>
                          <!-- <h5>Facebook</h5> -->
                        </v-btn>

                        <v-btn class="mx-1" shaped rounded color="cyan darken-2" outlined
                        width="150" height="50">
                          <v-icon class="icon">fab fa-google</v-icon>
                          <!-- <h5 class="text-center">Google</h5> -->
                        </v-btn>
                      </div>
                      <v-divider class="mt-4 mx-1" width="97%" light></v-divider>

                      <v-form >
                        <v-text-field class="mt-4"
                        id="email"
                        label="Email"
                        name="Email"
                        type="text"
                        color="cyan darken-2"
                        rounded
                        outlined
                        
                        />

                        <v-text-field
                        id="password"
                        label="Password"
                        name="Password"
                        type="password"
                        color="cyan darken-2"
                        light
                        rounded
                        outlined/>
                        
                      </v-form>
                      
                    </v-card-text>

                    <div class="text-center mt-4">
                      <v-btn  width="250" height="50" rounded color="cyan darken-2" dark>Create an account</v-btn>
                    </div>
                    <div class="text-center mt-4">
                      <v-btn outlined width="250" height="50" rounded color="cyan darken-2" dark>Continue as a guest</v-btn>
                    </div>

                    
                    
                  </v-col>

                  
                </v-row>

              </v-window-item>
              </v-window>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<style scoped>


</style>


<script>

 
export default {
  data: () => ({
    step: 1
  }),

  props:{
    source: String
  }
  };

</script>
