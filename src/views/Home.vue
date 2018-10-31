<template>
	<div class="home">
		<!--<img alt="Vue logo" src="../assets/logo.png">-->
		<p>复现chrome翻译成中文视图不更新：{{test}}</p>
		<!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
	</div>
</template>

<script>
  // @ is an alias to /src
  // import HelloWorld from '@/components/HelloWorld.vue'

  export default {
    name: 'home',
    data() {
      return {
        test: 0
      }
    },
    components: {
      // HelloWorld
    },
    mounted() {
      setInterval(() => {
        this.test += 1
      }, 1000)
    }
  }
</script>
