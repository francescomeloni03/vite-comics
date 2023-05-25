<script>
export default {
    name: "AppMainLink",
    props: ["icons"]
}
</script>


<template>
    <div class="linkMain">
        <div v-for="icon in icons" class="imgbox">
            <img class="img" :class="icon.dscrpt" :src="icon.img">
            <a>{{ icon.dscrpt }}</a>
        </div>
    </div>
</template>

<style lang="scss">
@use "../main.scss" as *;

.linkMain {
    display: flex;
    justify-content: center;
    width: 100%;
    height: 150px;
    background-color: $primaryColor;
    position: relative;
    z-index: 2;
}

.imgbox {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 230px;
    font-size: 15px;
    color: white;
}

.img {
    height: 60px;
    padding-right: 15px;
    color: white;
}
</style>