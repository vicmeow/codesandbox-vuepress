<template>
  <div class="special-layout">
    
    <nav class="nav">
      <p class="nav-heading">Special Layout Component</p>
      <a href="/guide/#custom-layouts">← Go Back</a>
    </nav>
    <Content />
  </div>
</template>

<style src="prismjs/themes/prism-tomorrow.css"></style>

<style scoped>
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

.nav {
  margin: 0 auto;
  text-align: center;
  max-width: 250px;
}

.nav-heading {
  font-size: 2rem;
  font-weight: bold;
}

a {
  background: #3eaf7c;
  padding: .5rem 1rem;
  border-radius: 4px;
  color: white;
}
</style>

