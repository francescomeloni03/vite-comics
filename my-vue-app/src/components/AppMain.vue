<script>
export default {
    name: "AppMain",
    props: ["comics"],
}
</script>


<template>
    <main>
        <div class="main">

            <div class="boxCurrent">
                CURRENT SERIES
            </div>
            <div class="boxComics">
                <div v-for="comic in comics">
                    <div class="boxComic">
                        <img class="comicImg" :src="comic.thumb" alt="">
                        <!-- Dinamicamente scriviamo le "series" con aggiunta di "toUpperCase" (Modifica la stringa in MAIUSCOLO) -->
                        <p class="textBoxComic">{{ comic.series.toUpperCase() }}</p>
                    </div>
                </div>
            </div>
            <div class="buttonMain">
                <button class="textButton">LOAD MORE</button>
            </div>

        </div>
    </main>
</template>




<style lang="scss">
@use "../main.scss" as *;

.main {
    width: 100%;
    background-color: $secondaryColor;
    padding: 50px;
}

.boxCurrent {
    width: 250px;
    background-color: $primaryColor;
    position: absolute;
    margin-top: -75px;
    font-size: 28px;
    color: white;
    display: flex;
    justify-content: center;
    padding: 7px;
}

.textButton {
    background-color: $primaryColor;
    color: white;
    margin-top: 60px;
    padding-left: 50px;
    padding-right: 50px;
}
</style>

<style scoped>
.boxComics {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.boxComic {
    width: 180px;
    height: 240px;
    margin-top: 2em;
    margin-left: 1em;
}

.comicImg {
    width: 100%;
    height: 190px;
    object-fit: cover;
    object-position: top;
}

.textBoxComic {
    color: white;
    margin-top: 10px;
}


.buttonMain {
    width: fit-content;
    margin: auto;
}
</style>