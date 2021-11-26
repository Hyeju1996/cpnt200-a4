<template>
  <v-main>
    <header>
      <Header :title="info.title" :subHeading="info.author" />
    </header>
    <section>
      <h2>food blogs</h2>
      <p>here are some recipes I make</p>
      <ul>
        <li>{{ topics[0] }}</li>
        <li>{{ topics[1] }}</li>
        <li>{{ topics[2] }}</li>
      </ul>
    </section>
    <section>
      <h2>Who inspired us</h2>
      <p>{{ references.name }}, {{ references.location }}</p>
    </section>
    <footer>
      <p>&copy; 2021 Jessica</p>
    </footer>
  </v-main>
</template>

<script>
export default {
  data() {
    return {
      info: {
        title: "food stuff",
        author: "Hyeju",
        tagline: "my favorite food",
      },
      references: {
        name: "Company's coming",
        location: "Korea",
      },
      topics: ["Kimchie", "noodle", "bibmbom"],
    };
  },
};
</script>