<template>
    <div class="about">
    <img class="pfp" src="../assets/Portfolio.jpeg"/>
        <h1>
            Kenaniah Subrahmanyam
        </h1>
        <div class="bio">
            <div class="left">
                <h2>
                    Hello there! My name is Kenaniah. I am a Full-Stack developer with an emphasis on server-side coding. This is my personal website which I created using Vue.js and Naive UI. Feel free to take a look around or reach out to me!
                </h2>
            </div>
        </div>
    </div>
</template>

<style lang="css" scoped>
    .pfp{
        margin-top: 30px;
        width: 200px;
        border-radius: 30px;
    }
    
    .about{
        text-align: center;
        background-color: #F8F1F1;
        margin: auto;
        margin-top: 20px;
        width: min(90%, 600px);
        border-radius: 10px;
    }

    .left{
        text-align: left;
        padding: min(50px, 50%);
        color: #F8F1F1;
        margin: auto;
    }

    .bio{
        margin-top: 10px;
        background-color: #243964;
        height: auto;
        border-bottom-left-radius: 10px;
        border-bottom-right-radius: 10px;
    }

    p{
        color: black;
    }
</style>