<script setup>
</script>

<template>
        <br>
        <div class="projects">
            <section>
                <h1 class="project_title"><span class="badge">Dimension - Game Engine & Game</span></h1>
                <p class="timeline-subtitle">March 2022 - December 2022, Electron.js, Node.js, and P5.js</p>
                <h4 class="project_info">This project consists of a game engine and a game created with that engine. It was created for my UCF Senior Design Project, in other words my final project to finish up my degree. Below is a snip of the game/engine in developer mode, where you can see all the collision and mesh boxes:</h4>
                <div class="aline"><img class="pics" src="../assets/Dimension1.png"/></div><br/>
                <h4 class="project_info">For the duration of the project, I worked on a team with 5 members. My role on the project was to create the game engine, a system for state machine driven AIs and a method for switching animations. Additionally, I worked on python scripts to automate tedious task, and worked on the system for loading in assets. The game engine also consisted of a UI for world building and a UI for adding meshboxes onto various animations. The UI components can be seen below, with the world building UI on the left and the action editor on the right:</h4>
                <div class="aline"><img style="width: min(60px, 10vw); height: min(330px, 50vw); margin: auto; margin-right:0px; border: solid white 1px;" src="../assets/Dimension3.png"/><img class="pics" style="margin-left:6px;" src="../assets/Dimension2.png"/></div>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Club Event Organizer  - Social Media</span> | <span class="badge"><a target="_blank" href="http://147.182.141.121/">Demo</a></span>  | <span class="badge"><a target="_blank" href="https://github.com/ken3512/DB_Application">GitHub</a></span></h1>
                <p class="timeline-subtitle">March 2022 – April 2022, HTML & CSS, PHP, JavaScript, and MySQL</p>
                <h4 class="project_info">This project was an event organizer centered around student registered organizations that I created for my database class. On the project I worked with one other person to complete the application. The goal of the project was to create a complex database and intricate interactions between tables.  Users could only see events that were public to their university or private to their RSOs. In the project we implemented security in the form of encryption and prepared statements. My role on the project was to implement encryption, create the database structure, and assist with API creation.</h4>
                <h4 class="project_info">Contains social media features, such as posting, liking, commenting, creating RSOs, etc.</h4> 
                <div class="aline"><img class="pics" src="../assets/ClubEvent2.png"/></div>
                <h4 class="project_info">Application also allowed users to edit website appearance and manage account, as seen below:</h4> 
                <div class="aline"><img class="pics" src="../assets/ClubEvent4.png"/></div>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Dungoen Run - Web Game</span> | <span class="badge"><a target="_blank" href="https://dungeonrun.herokuapp.com/">Demo</a></span> | <span class="badge"><a target="_blank" href="https://github.com/Group14-COP4331/large-project">GitHub</a></span></h1>
                <p class="timeline-subtitle">November 2021 – December 2021, MongoDB, Express.js, React, Node.js, and P5.js</p>
                <h4 class="project_info">This project implemented a game that allowed users to login/signup, save progress, and buy in game assets. Signup form shown below:</h4>
                <div class="aline"><img class="pics" src="../assets/DungeonRun4.png"/></div>
                <h4 class="project_info">This project was created with 6 members.  On the project I was tasked with creating the game logic and integrating APIs into frontend UI components Login system was built with full capabilities such as email verification, forget/change password, etc. Login form can be seen below:</h4>
                <div class="aline"><img class="pics" src="../assets/DungeonRun1.png"/></div>
                <h4 class="project_info">Game was an infinite running game, that allowed users to earn high scores and get on the global leader board. A screenshot of the game can be seen below:</h4>
                <div class="aline"><img class="pics" src="../assets/DungeonRun3.png"/></div>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Compiler</span> | <span class="badge"><a target="_blank" href="https://github.com/ken3512/Compiler">GitHub</a></span></h1>
                <p class="timeline-subtitle">June 2021 – July 2021, C</p>
                <h4 class="project_info">This project I created for my System Software class. The project consists of a virtual machine, lexer, parser and assembler. All components come together and work to compile a language described in the class.</h4>
            </section>

            <section>
                <h1 class="project_title"><span class="badge">Command line</span> | <span class="badge"><a target="_blank" href="https://github.com/ken3512/CommandLine">GitHub</a></span></h1>
                <p class="timeline-subtitle">November 2021 – December 2021, C</p>
                <h4 class="project_info">This project I created for my Operating Systems class. It acts as a command line, allowing users to enter various commands.</h4>
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

    .aline{
        display: flex;
        justify-content: center;
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

    .pics{
        border: solid white 1px;
        margin: auto;
        width: min(90%, 500px);
    }

    h4{
        margin: 0px;
        margin-bottom: 10px;
        margin-top: 5px;
    }
</style>