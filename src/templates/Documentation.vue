<template>
  <div>
    <Header
      :id="$page.documentation.id"
      :title="$page.documentation.title"
      :date="$page.documentation.date"
      :img="$page.documentation.image.path.src"
    />
    <VueRemarkContent />
  </div>
</template>

<page-query>
query Documentation ($id: ID!) {
  documentation(id: $id) {
    id
    title
    date
    image {
      path
    }
  }
}
</page-query>

<script>
import Header from "./../components/Header.vue";

export default {
  components: {
    Header,
  },
};
</script>

<style>
body {
  margin: 30px auto;
  max-width: 50%;
}

blockquote {
  color: blue;
}
</style>
