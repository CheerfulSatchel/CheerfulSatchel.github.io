<template>
  <div id="content">
    <div id="about">
      <h1>about</h1>
      <img id="picture-of-me" src="../assets/james.jpg">
      <p>Hello! My name is James Wu, and thank you for visiting my website.</p>
      <p>My primary interests are in cloud computing, embedded and real-time systems.</p>
      <p>I received my Bachelor of Science degree in Computer Science from the University of Virginia in December 2017.</p>
      <p>I am proficient with TypeScript and Python. I am familiar with C/C++, Swift, and Java.</p>
      <p>I am currently a software engineer at Microsoft working on Azure.</p>
      <p>In my free time, I run long distances, go on hikes/long walks, and spend time with friends and family.</p>
    </div>
    <Career/>
    <SideProjects/>
    <div id="contact">
      <h1>contact</h1>
      <p>
        <v-icon>phone</v-icon>703-423-9577
      </p>
      <p>
        <v-icon>email</v-icon>therealjameswu@gmail.com
      </p>
      <p>
        <v-icon>group</v-icon>
        <a href="https://www.linkedin.com/in/therealjameswu/">Connect with me on Linkedin</a>
      </p>
    </div>
  </div>
</template>

<script>
import Career from "@/components/Career";
import SideProjects from "@/components/SideProjects";

export default {
  components: {
    Career,
    SideProjects
  }
};
</script>

<style>
/*Based on https://stackoverflow.com/a/38994837*/
#content {
  width: 80%;
  overflow-y: auto;
  -ms-overflow-style: none; /*IE 10+*/
  scrollbar-width: none; /*Firefox*/
}

#content::-webkit-scrollbar {
  display: none; /*Safari and Chrome*/
}

#picture-of-me {
  float: right;
  width: 24%;
  height: 24%;
  border-radius: 30px;
}

h1 {
  padding-top: 20px;
  padding-bottom: 20px;
}
</style>
