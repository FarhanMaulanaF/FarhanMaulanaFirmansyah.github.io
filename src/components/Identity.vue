<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img 
          :src="require('../assets/Profile_Photo.png')"
          alt="Farhan Firmansyah"
          class="my-3"
          contain
          height="200"
        />
      </v-col>
      
      <!-- Main Identity -->
      <v-col>
          <h2> Farhan Maulana Firmansyah </h2>
          <p class="font-weight-regular black--text title"> Mertoyudan District, Central of Java</p>
          <a
            class="font-weight-regular black--text title"
            style="text-decoration:none"
            href="mailto:farhanmaulanafirmansyah@mail.ugm.ac.id"
            target="_blank"> 
            farhanmaulanafirmansyah@gmail.com 
          </a>
            <br/>
          <a
            class="font-weight-regular black--text title"
            style="text-decoration:none"
            href="https://wa.me/085741430639"
            target="_blank"> 
            085741430639 
          </a>
      </v-col>
<!-- 
      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to My Personal Website
        </h1>

        <p class="subheading font-weight-regular">
          For help and collaboration with other Vuetify developers,
          <br>please join our online
          <a
            href="https://community.vuetifyjs.com"
            target="_blank"
          >Discord Community</a>
        </p>
      </v-col> -->

      <!-- More detail about my identity -->
      <v-col
        class="mb-5"
        cols="12"
      >
        <v-divider></v-divider>
        <br/>

        <!-- About me detail -->
        <h2 class="headline font-weight-bold mb-3">
          About Me
        </h2>
        <p>Hello! My name is Farhan Maulana Firmansyah. I'm 19th years old. At the time, I'm studied at Information Engineering program in Gadjah Mada University.</p>
        
        <!-- Work Experiences Detail -->
        <h2 class="headline font-weight-bold mb-3">
          Work Experiences
        </h2>
        <br/>
        <v-row justify="center">
          <table class="table table-striped table-bordered">
            <thead>
              <tr>
                <th> Company </th>
                <th> Role </th>
                <th> Status </th>
                <th> Period </th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="user in users" :key="user.id">
                <td>{{user.company}}</td>
                <td>{{user.role}}</td>
                <td>{{user.status}}</td>
                <td>{{user.period}}</td>
              </tr>
            </tbody>
          </table>
        </v-row>
        <br/>

        <!-- Education Detail -->
        <h2 class="headline font-weight-bold mb-3">
          Education
        </h2>
        <h4>Gadjah Mada University, Yogyakarta</h4>
        <p> Information Engineering <br/>
          2020 - until now
        </p>
        <br/>

        <!-- Skills detail -->
        <h2 class="headline font-weight-bold mb-3">
          Skills
        </h2>
        <li style="list-style-type: none;">HTML</li>
        <li style="list-style-type: none;">CSS</li>
        <li style="list-style-type: none;">Java Script</li>
        <li style="list-style-type: none;">Figma</li>
        <li style="list-style-type: none;">Object Oriented</li>
        <li style="list-style-type: none;">My SQL</li>
        <br/>

        <!-- Contact Detail -->
        <h2 class="headline font-weight-bold mb-3">
          Contact Me
        </h2>
        <Form/>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Form from './Form.vue';

  export default {
    name: 'HelloWorld',

    components:{
      Form,
    },

    data: () => ({
      users: [
        {company : 'Nightlogin UGM', 
        role: 'User Interface Designer', 
        status:'active', 
        period:'2021 - until now'}
      ]
    }),
  }
</script>
