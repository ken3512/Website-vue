<script setup>
</script>

<template>
        <br>
        <div class="projects">
            <section>
                <h1 class="project_title"><span class="badge">Dimension - Game Engine & Game</span></h1>
                <p class="timeline-subtitle">March 2022 - December 2022, Electron.js, Node.js, and P5.js</p>
                <h4 class="project_info">Hello my name is Kenaniah Subrahmanyam. I first started coding at about 13 and I am currently a senior at UCF as a Computer Science major. I have managed to keep a 3.97 GPA throughout my degree while working part time. I have learned many skills along the way!</h4>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Club Event Organizer  - Social Media</span></h1>
                <p class="timeline-subtitle">March 2022 – April 2022, HTML & CSS, PHP, JavaScript, and MySQL</p>
                <h4 class="project_info">Hello my name is Kenaniah Subrahmanyam. I first started coding at about 13 and I am currently a senior at UCF as a Computer Science major. I have managed to keep a 3.97 GPA throughout my degree while working part time. I have learned many skills along the way!</h4>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Dungoen Run - Web Game</span></h1>
                <p class="timeline-subtitle">November 2021 – December 2021, MongoDB, Express.js, React, Node.js, and P5.js</p>
                <h4 class="project_info">Hello my name is Kenaniah Subrahmanyam. I first started coding at about 13 and I am currently a senior at UCF as a Computer Science major. I have managed to keep a 3.97 GPA throughout my degree while working part time. I have learned many skills along the way!</h4>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Compiler</span></h1>
                <p class="timeline-subtitle">June 2021 – July 2021, C</p>
                <h4 class="project_info">Hello my name is Kenaniah Subrahmanyam. I first started coding at about 13 and I am currently a senior at UCF as a Computer Science major. I have managed to keep a 3.97 GPA throughout my degree while working part time. I have learned many skills along the way!</h4>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Command line</span></h1>
                <p class="timeline-subtitle">November 2021 – December 2021, C</p>
                <h4 class="project_info">Hello my name is Kenaniah Subrahmanyam. I first started coding at about 13 and I am currently a senior at UCF as a Computer Science major. I have managed to keep a 3.97 GPA throughout my degree while working part time. I have learned many skills along the way!</h4>
            </section>
        </div>
</template>

<style lang="scss" scoped>
$secondary: #4f537b;
    .project_info{
        color: white;
    }

    .project_title{
        font-weight: bold;
        color: white;
        margin-bottom: 0px;
        .badge {
            background: $secondary;
            padding: 4px 8px;
            border-radius: 3px;
            font-size: 18px;
            font-weight: bold;
        }
    }

    .project_headers{
        font-weight: bold;
        color: white;
    }

    .timeline-subtitle {
        color: white;
        margin-top: 0px;
        font-weight: 300;
        font-style: italic;
        opacity: .4;
        font-size: 13px;
    }

    .projects{
        border-radius: 3px;
        background-color: #27293d;
        margin: auto;
        width: min(800px, 85%);
        padding: 15px;
    }
</style>