<template>
  <div class="home">
    <h1 class="home--title">tools.ipassby</h1>
    <div class="tools--container">
      <div class="tool--item" v-for="item in tools" :key="item.label">
        <a :href="item.path">{{ item.label }}</a>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  data() {
    return {
      tools: [
        {
          path: '/unlockmusic',
          label: 'Unlock Music'
        }
      ]
    }
  }
}
</script>
