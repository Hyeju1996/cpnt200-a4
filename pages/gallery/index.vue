<template>
  <v-main>
    <header>
      <Header :title="info.title" :subHeading="info.tagline" />
    </header>
    <section>
      <h2>Photos</h2>
      <p>Here is photo of my dog</p>
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
        title: "food blog",
        author: "Hyeju",
        tagline: "when you wish apon a star",
      },
      references: {
        name: "Hyeju",
        location: "Calgary",
      },
      topics: ["frontend", "backend", "cms"],
    };
  },
};
</script>

