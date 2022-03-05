<template>
    <div class="header">
        
    </div>
</template>

<script>
export default {
  name: 'Sidebar',
  props: {
    selected: Boolean
  }
}
</script>

<style scoped>
    div {
        position:absolute;
        left:0;
        top:0;
        width:100%;
        height:100vh;
        cursor-events:none;
        background:#2225;
        transition-duration:200ms;
    }
</style>