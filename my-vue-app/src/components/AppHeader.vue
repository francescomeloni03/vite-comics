<script>
export default {
    name: "AppHeader",
    props: ["linkHeader"],
}
</script>


<template>
    <header>
        <div class="container-lg ">

            <div class="navbar">
                <div class="logoContainer">
                    <img class="headerLogo" src="src/assets/img/dc-logo.png" alt="">
                </div>
                <div class="linkHeader">
                    <div v-for="link in linkHeader" class="link">
                        {{ link }}
                    </div>
                </div>
            </div>

        </div>
    </header>
</template>


<style scoped>
header {
    height: 130px;
}

.navbar {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.headerLogo {
    height: 75px;
}


.linkHeader {
    height: 115px;
    line-height: 110px;
    display: flex;
    align-items: center;
}

div.link {
    margin: 0 10px;
    height: 115px;
    font-size: 14px;
    font-weight: 500;
    ;
}

.link:hover {
    color: #0282f9;
    border-bottom: 4px solid #0282f9;

}
</style>