<template>
    <div>Test
        <h1>
            About Us
        </h1>
    </div>
</template>

<script>
export default {
  name: 'Homepage',
  props: {
    contactemail: String,
    contactphone: String
  }
}
</script>

<style scoped>
    h1 {
        width:90vw;
        margin-left:4vw;
        
    }
</style>