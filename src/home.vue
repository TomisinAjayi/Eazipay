<template>
    <nav>
        <button @click="home">Landing Page</button>
    </nav>
</template>

<script>
   export default {
    methods: {
        home () {
        $router.push("/")
    },
    }
   }
</script>