<template>
  <div id="career">
    <h1>career</h1>
    <v-timeline align-top>
      <v-timeline-item v-for="(item, i) in items" :key="i" :color="item.color" :icon="item.icon">
        <template v-slot:opposite>
          <span :class="`title font-weight-light ${item.color}--text`" v-text="item.dates"></span>
        </template>
        <div class="py-3">
          <h2 :class="`title font-weight-bold mb-3 ${item.color}--text`">{{item.title}}</h2>
          <div>{{item.description}}</div>
        </div>
      </v-timeline-item>
    </v-timeline>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: [
      {
        color: "green",
        icon: "work",
        title: "software engineer @ Microsoft",
        dates: "March 2020 - Present",
        description:
          "Azure front-end using ReactViews and TypeScript"
      },
      {
        color: "orange",
        icon: "work",
        title: "software engineer @ Collins Aerospace",
        dates: "July 2019 - March 2020",
        description:
          "Unmanned Aerial Vehicle (UAV) mission processor load modules"
      },
      {
        color: "blue",
        icon: "work",
        title: "software engineer @ Capital One",
        dates: "February 2018 - July 2019",
        description:
          "Transaction Underwriting and Deployment Pipeline Compliance (Java, Python)"
      },
      {
        color: "orange",
        icon: "school",
        title: "graduated from University of Virginia",
        dates: "December 2017",
        description: "finished undergraduate studies with distinction"
      },
      {
        color: "blue",
        icon: "star_border",
        title: "intern @ Capital One",
        dates: "Summer 2017",
        description:
          "developed Apache Spark application for Rewards Earn Engine (Java)"
      },
      {
        color: "purple",
        icon: "star_border",
        title: "intern @ Leidos",
        dates: "Summer 2016",
        description:
          "Reduction of Data using Compression Enhancement (RDUCE), a LIDAR real-time application (C++)"
      },
      {
        color: "blue",
        icon: "star_border",
        title: "intern @ Fairfax Collegiate",
        dates: "Summer 2015",
        description: "taught (rowdy) 4-8th grade students Lego Mindstorms"
      },
      {
        color: "orange",
        icon: "school",
        title: "started school @ University of Virginia",
        dates: "August 2014",
        description: "began undergraduate studies in engineering"
      },
      {
        color: "green",
        icon: "mood",
        title: "birthday",
        dates: "August 10, 1996",
        description: "James Wu has entered the world"
      }
    ]
  })
};
</script>

<style>
</style>
