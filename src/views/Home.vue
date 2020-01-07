<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <div v-for="student in students">
      <p>{{student.first_name}} {{student.last_name}}</p>
      <p>{{student.email}}</p>
      <p>{{student.phone_number}}</p>
      <p>{{student.linkedin_url}}</p>
      <p>{{student.github_url}}</p>
      <p>{{student.website_url}}</p>
      <p>{{student.twitter}}</p>
      <p>{{student.resume}}</p>
      <hr>

    </div>
  </div>
</template>

<style>
</style>

<script>
export default {
  data: function() {
    return {
      students: [{
        first_name: "Brian",
        last_name: "Rice",
        email: "brian@brian.com",
        phone_number: "123-456-7890",
        short_bio: "He's some guy who teaches coding",
        linkedin_url: "https://www.linkedin.com/in/brian_rice",
        twitter_handle: "http://twitter.com/handle/brian_rice",
        website_url: "https://www.brian_rice.com",
        resume_url: "https://www.brian_rice.com/resume",
        github_url: "https://www.github.com/brian_rice",
        photo: "This is an average-looking photo"
      }
      ]
    };
  },
  created: function() {},
  methods: {}
};
</script>
