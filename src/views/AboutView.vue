<template>
    <div class="about">
    <img class="pfp" src="../assets/Portfolio.jpeg"/>
        <h1>
            Kenaniah Subrahmanyam
        </h1>
        <div class="bio">
            <div class="left">
                <h2>
                    Hello my name is Kenaniah Subrahmanyam. I first started coding at about 13 and I am currently a senior at UCF as a Computer Science major. I have managed to keep a 3.97 GPA throughout my degree while working part time. I have learned many skills along the way!
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