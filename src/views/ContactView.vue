<script setup>
</script>

<template>
    <div class="about">
        <div class="contact">
            <h2 class="left">
                321-263-7871
            </h2>
        </div>

        <div class="contact">
            <h2 class="left">
                kenaniah.subrahmanyam@outlook.com
            </h2>
        </div>
    </div>
</template>

<style scoped>
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
        height: 300px;
        border-radius: 10px;
        padding: 20px;
    }

    .left{
        text-align: left;
        color: #F8F1F1;
        padding: 10px;
        margin: auto;
        font-size: min(20px, 120%);
    }

    .contact{
        width: min(400px, 90%);
        margin: auto;
        color: white;
        margin-top: 45px;
        background-color: #243964;
        border-radius: 10px;
    }

    p{
        color: black;
    }
</style>