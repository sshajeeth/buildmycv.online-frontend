<template>
    <nav>
        <v-navigation-drawer
          v-model="drawer"
          dark
          app
          mini-variant
          mini-variant-width="190"
          class="cyan darken-2"
        >
          <v-ist>
            <v-list-item class="mb-12">
              <v-list-item-action></v-list-item-action>
            </v-list-item>
          </v-ist>

          <v-list flat>
              <v-list-item router to="/">
              <v-list-item-content>
                  <v-icon class="mb-2">dashboard</v-icon>
                  <v-list-item-subtitle align="center">Dashboard</v-list-item-subtitle>  
              </v-list-item-content>
              </v-list-item>
          </v-list>

          <v-list flat>
              <v-list-item router to="/">
              <v-list-item-content>
                  <v-icon class="mb-2">check_circle</v-icon>
                  <v-list-item-subtitle align="center">Review My Resume</v-list-item-subtitle>  
              </v-list-item-content>
              </v-list-item>
          </v-list>

          <v-list flat>
              <v-list-item router to="/">
              <v-list-item-content>
                  <v-icon class="mb-2">create</v-icon>
                  <v-list-item-subtitle align="center">Write My Resume</v-list-item-subtitle>  
              </v-list-item-content>
              </v-list-item>
          </v-list>

          <v-list flat>
              <v-list-item router to="/">
              <v-list-item-content>
                  <v-icon class="mb-2">videocam</v-icon>
                  <v-list-item-subtitle >Guide</v-list-item-subtitle>  
              </v-list-item-content>
              </v-list-item>
          </v-list>

          <v-list flat>
              <v-list-item router to="/">
              <v-list-item-content>
                  <v-icon class="mb-2">person</v-icon>
                  <v-list-item-subtitle align="center">My Profile</v-list-item-subtitle>  
              </v-list-item-content>
              </v-list-item>
          </v-list>

          <v-list flat>
              <v-list-item router to="login">
              <v-list-item-content>
                  <v-icon class="mb-2">logout</v-icon>
                  <v-list-item-subtitle align="center">Logout</v-list-item-subtitle>  
              </v-list-item-content>
              </v-list-item>
          </v-list>
        </v-navigation-drawer>
      </nav>
</template>
