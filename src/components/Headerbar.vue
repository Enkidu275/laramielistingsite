<template>
    <div>
        <!--Use "a" to enable tabbing for ADA purposes-->
        <a href="">
            <span class="headerlogo1">
                <!--The following is the LAR house icon thing-->
                <svg width="10vw" viewBox="40 20 242 213">
                    <path fill="#CCCCFF" d="M74 116L90 116L90 209L157 209L157 224L74 224L74 116ZM157 29L157 202L141 202L141 60L99 89L141 89L141 105L113 105L113 202L97 202L97 105L48 105L157 29ZM251 224L227 105L274 105L168 31L169 224L185 224L185 62L223 89L185 89L185 105L211 105L236 224L251 224Z"/>
                </svg>
            </span>
            <span class="headerlogo2">
                aramie<br/>Restoration
            </span>
        </a>
        <a href="" class="headerlogo3">
            
        </a>
    </div>
</template>

<script>
    export default {
        name: 'Headerbar',
        props: {
            username: String
        }
    }
</script>

<style scoped>
    div {
        width:100%;
        margin-left:0;
        margin-top:0;
        height:10vw;
        background:linear-gradient(45deg,#9999FF 26%, transparent 25%),linear-gradient(-45deg,#9999FF 26%,transparent 25%),linear-gradient(45deg,transparent 75%, #9999FF 75%),linear-gradient(-45deg,transparent 75%, #9999FF 75%),linear-gradient(0deg,#8888FF,#8888FF);
        background-size:2vw 2vw;
        background-position:0 0,0 1vw,1vw -1vw,-1vw 0px;
        text-align:left;
    }
    .headerlogo1 {
        float:left;
        display:inline;
        width:10vw;
        height:10vw;
    }
    .headerlogo2 {
        float:left;
        height:10vw;
        color:#CCCCFF;
        font:4vw Cambria, sans-seif;
    }
    .headerlogo3 {
        text-decoration:none;
        font-style:none;
        height:10vw;
        margin-right:2vw;
        float:right;
        color:#CCCCFF;
        font:5vw Cambria, sans-serif;
    }
</style>