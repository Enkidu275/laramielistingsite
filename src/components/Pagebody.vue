<template>
    <div>
        <Homepage contactemail="enkidu275@gmail.com" contactphone="(307)343-3247"/>
    </div>
</template>

<script>
export default {
  name: 'Pagebody',
  props: {
    route: String
  }
}
</script>

<style scoped>
    div {
        position:absolute;
        width:100%;
        height:calc(100vh-10vw);
        top:0;
        left:0;
        margin-top:0;
        margin-left:0;
        background:pink;
        overflow-y:scroll;
        overflow-x:none;
    }
</style>