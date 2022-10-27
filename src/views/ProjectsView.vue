<script setup>
</script>

<template>
        <br>
        <div class="projects">
            <section>
                <h1 class="project_title"><span class="badge">Dimension - Game Engine & Game</span> | <span class="badge"><a href="/">Demo</a></span>  | <span class="badge"><a href="/">GitHub</a></span></h1>
                <p class="timeline-subtitle">March 2022 - December 2022, Electron.js, Node.js, and P5.js</p>
                <h4 class="project_info">Engine built completely from scratch without any collision or physics libraries. <br>Includes 2D game engine which loads images, animates through frames, and drives world physics. </h4>
                <img class="pfp" src="../assets/Dimension1.png"/>
                <h4 class="project_info">Includes a UI for creating AI actions</h4>
                <img class="pfp" src="../assets/Dimension2.png"/>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Club Event Organizer  - Social Media</span> | <span class="badge"><a href="/">Demo</a></span>  | <span class="badge"><a href="/">GitHub</a></span></h1>
                <p class="timeline-subtitle">March 2022 – April 2022, HTML & CSS, PHP, JavaScript, and MySQL</p>
                <h4 class="project_info">Contains account management features, such as changing password/username, etc.</h4>

                <img class="pfp" src="../assets/ClubEvent1.png"/>
                <h4 class="project_info">Contains social media features, such as posting, liking, commenting, creating RSOs, etc.</h4> 
                <img class="pfp" src="../assets/ClubEvent2.png"/>
                <img class="pfp" src="../assets/ClubEvent3.png"/>
                <img class="pfp" src="../assets/ClubEvent4.png"/>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Dungoen Run - Web Game</span> | <span class="badge"><a href="/">Demo</a></span> | <span class="badge"><a href="/">GitHub</a></span></h1>
                <p class="timeline-subtitle">November 2021 – December 2021, MongoDB, Express.js, React, Node.js, and P5.js</p>
                <h4 class="project_info"></h4>
                <img class="pfp" src="../assets/DungeonRun1.png"/>
                <img class="pfp" src="../assets/DungeonRun2.png"/>
                <img class="pfp" src="../assets/DungeonRun3.png"/>
                <img class="pfp" src="../assets/DungeonRun4.png"/>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Compiler</span> | <span class="badge"><a href="/">GitHub</a></span></h1>
                <p class="timeline-subtitle">June 2021 – July 2021, C</p>
                <h4 class="project_info"></h4>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Command line</span> | <span class="badge"><a href="/">GitHub</a></span></h1>
                <p class="timeline-subtitle">November 2021 – December 2021, C</p>
                <h4 class="project_info"></h4>
            </section>
        </div>
        <br>
</template>

<style lang="scss" scoped>
$secondary: #4f537b;
    .project_info{
        color: white;
        font-size: min(0.9rem, 2.6vw);
    }

    .project_title{
        font-weight: bold;
        color: white;
        margin-bottom: 0px;
        .badge {
            background: $secondary;
            padding: 4px 8px;
            border-radius: 3px;
            font-size: min(18px, 3vw);
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
        font-size: min(13px, 2.4vw);
    }

    .projects{
        border-radius: 3px;
        background-color: #27293d;
        margin: auto;
        width: min(800px, 85%);
        padding: 15px;
    }

    a{
        text-decoration: none;
        color: white;
    }

    .pfp{
        width: 200px;
    }
</style>