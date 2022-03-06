<template>
    <div :class="(active==true)?'active':''">
        <div class="greyout"></div>
        <a v-on:click="toggle" href="" class="sidebarselect">
            <svg viewBox="0 0 20 20">
                <path d="M4 4L16 4L16 8L4 8Z"/>
                <path d="M4 12L16 12L16 16L4 16Z"/>
            </svg>
        </a>
        <div class="sidebarmenu">

        </div>
    </div>
</template>

<script>
export default {
    name:'Sidebar',
    props:{
        active:Boolean
    },
    methods:{
        toggle:function(){
            this.active=!this.active;
        }
    }
}
</script>

<style scoped>
    .greyout {
        position:absolute;
        left:0;
        top:0;
        width:100%;
        height:100vh;
        transition-duration:200ms;
        transition-props:background;
    }
    .active .greyout {
        background:#2225;
    }
    .sidebarselect {
        position:absolute;
        width:10vw;
        height:10vw;
        left:90vw;
        top:0;
        background:#AAAAFF;
        transition-duration:200ms;
    }
    .sidebarselect:hover {
        background:#BBBBFF;
    }
    .active .sidebarselect {
        left:50vw;
    }
    .sidebarselect path {
        fill:#DDDDFF;
    }
    .active .sidebarselect path:nth-child(1) {
        d:path("M5 3L17 15L15 17L3 5Z");
    }
    .active .sidebarselect path:nth-child(2) {
        d:path("M3 15L15 3L17 5L5 17Z");
    }
    .sidebarmenu {
        position:absolute;
        width:0;
        height:100%;
        left:100%;
        top:0;
        background:#BBBBFF;
        transition-duration:200ms;
    }
    .active .sidebarmenu {
        left:60vw;
        width:40vw;
    }
</style>