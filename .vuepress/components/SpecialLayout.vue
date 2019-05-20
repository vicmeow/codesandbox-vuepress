<template>
  <div class="special-layout">
    <aside class="side">
      <p><strong>Component File Name:</strong></p>
      <p class="side-heading">{{ $options.fileName }}</p>
      <div class="frontmatter">
        <p><strong>Frontmatter:</strong></p>
        <p>{{ $frontmatter }}</p>
      </div>
      <a href="/guide/#custom-layouts">← Go Back</a>
    </aside>
    <Content />
  </div>
</template>

<script>
export default {
  fileName: 'SpecialLayout.vue'
}
</script>


<style src="prismjs/themes/prism-tomorrow.css"></style>

<style scoped>

p {
  margin: 0;
}

.special-layout {
  box-sizing: border-box;
  margin: 2rem auto;
  padding: 1rem 0;
  display: flex;
  flex-wrap: wrap;
  padding: 0 1rem;
  align-items: center;
  max-width: max-content;
}

.content {
  padding: 0;
  max-width: 740px;
  padding-bottom: 3.5rem;
}

.side {
  margin: 0 auto;
  padding: 0 2rem;
  text-align: center;
  max-width: 250px;
}

.side-heading {
  font-size: 1.5rem;
  font-weight: bold;
  margin: 0;
}

.frontmatter {
  margin-bottom: 1rem;
}

.frontmatter p {
  margin: 0;
}

a {
  display: inline-block;
  background: #3eaf7c;
  padding: .5rem 1rem;
  border-radius: 4px;
  color: white;
}
</style>

