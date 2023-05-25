<script>
export default {
    name: "AppBottomFooter"
}
</script>


<template>
    <div class="bottomFooter">
        <div class="container-lg containerFooter">
            <div>
                <button class="buttonSignUp">SIGN-UP NOW!</button>
            </div>
            <div class="boxRight">
                <h4 class="fontFollowUs">
                    <a href="">FOLLOW US</a>
                </h4>
                <img class="marginImg" src="src/assets/img/footer-facebook.png" alt="">
                <img class="marginImg" src="src/assets/img/footer-twitter.png" alt="">
                <img class="marginImg" src="src/assets/img/footer-youtube.png" alt="">
                <img class="marginImg" src="src/assets/img/footer-pinterest.png" alt="">
                <img class="marginImg" src="src/assets/img/footer-periscope.png" alt="">


            </div>

        </div>
    </div>
</template>


<style lang="scss">
@use "../main.scss" as *;

h4>a {
    font-weight: bold;
    text-decoration: none;
}

.containerFooter {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

button:hover {
    background-color: black;
}

.bottomFooter {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 110px;
    background-color: #303030;
    position: absolute;
}

.buttonSignUp {
    color: $color-white;
    padding: 10px;
    background-color: #303030;
    border: 2px solid $primaryColor;
    font-size: 20px;
}

.fontFollowUs {
    margin-top: 10px;
}

.boxRight {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.marginImg {
    margin-left: 10px;
}
</style>