<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <div v-for="resume in resumes">
      <p>{{resume.first_name}} {{resume.last_name}}</p>
      <p>{{resume.email}}</p>
      <p>{{resume.phone_number}}</p>
      <p>{{resume.linkedin_url}}</p>
      <p>{{resume.github_url}}</p>
      <p>{{resume.website_url}}</p>
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
      resumes: [{
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
