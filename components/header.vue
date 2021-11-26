<template>
  <header>
    <h1>{{ title }}</h1>
    <p>{{ subHeading }}</p>
  </header>
</template>
<script>
export default {
  props: ["title", "subHeading"],