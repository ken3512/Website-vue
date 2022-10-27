<script setup>
</script>

<template>
        <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.3.1/css/all.css">
    <div class="about">
            <br><br>
            <div class="copy-text phone">
                <h2 class="left">
                    321-263-7871
                </h2>
                <button class="right" @:click="copy('.phone', '321-263-7871')"><i class="fa fa-clone"></i></button>
            </div>
            <br><br><br>
            <div class="copy-text email">
                <h2 class="left">
                    kenaniah.subrahmanyam@outlook.com
                </h2>
                <button class="right" @:click="copy('.email', 'kenaniah.subrahmanyam@outlook.com')"><i class="fa fa-clone"></i></button>
            </div>
    </div>
</template>

<script>
export default{
  name: 'ContactView',
  data(){
    return{
      
    }
  },
  methods:
  {
    copy(select, input)
    {
        let copyText = document.querySelector(select);
        copyText.classList.add("active");
        window.getSelection().removeAllRanges();
        setTimeout(function () {
            copyText.classList.remove("active");
        }, 2000);
    }
  },
}
</script>



<style scoped>
    .about{
        text-align: center;
        background-color: #F8F1F1;
        margin: auto;
        margin-top: 20px;
        width: min(90%, 600px);
        height: 320px;
        border-radius: 10px;
        padding: 20px;
    }

    .left{
        text-align: left;
        color: #F8F1F1;
        padding: 10px;
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

    .right{
        position: absolute;
        right: 10px;
    }
    

    * {
	margin: 0px;
	padding: 0px;
	box-sizing: border-box;
}
body {
	font-family: "Roboto", sans-serif;
	background: #f0f2f7;
}
.container {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
}
.label {
	padding: 10px;
	font-size: 18px;
	color: #111;
}
.copy-text {
    margin: auto;
    width: 90%;
	position: relative;
	padding: 10px;
	background: #243964;
	border-radius: 10px;
	display: flex;
}
.copy-text input.text {
	padding: 10px;
	font-size: 18px;
	color: #555;
	border: none;
	outline: none;
}
.copy-text button {
	padding: 10px;
	background: #465987;
	color: #fff;
	font-size: 18px;
	border: none;
	outline: none;
	border-radius: 10px;
	cursor: pointer;
}

.copy-text button:active {
	background: #243964;
}
.copy-text button:before {
	content: "Copied";
	position: absolute;
	top: -55px;
	right: -12px;
	background: #243964;
	padding: 8px 10px;
	border-radius: 20px;
	font-size: 15px;
	display: none;
}
.copy-text button:after {
	content: "";
	position: absolute;
	top: -30px;
	right: 14px;
	width: 10px;
	height: 10px;
	background: #243964;
	transform: rotate(45deg);
	display: none;
}
.copy-text.active button:before,
.copy-text.active button:after {
	display: block;
}

</style>