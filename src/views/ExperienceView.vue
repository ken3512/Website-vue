
<template>
        <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Vertical Dark Timeline</title>
        <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.3.1/css/all.css">
    </head>
    <body>
        <div class="container">
            <div class="timeline">
                <div class="timeline-container">
                    <div class="timeline-icon">
                        <i class="fab fa-amazon"></i>
                    </div>
                    <div class="timeline-body">
                        <h4 class="timeline-title"><span class="badge">Software Engineer Intern at Amazon</span></h4>
                        <p style="font-weight: bold;">Seller Central - Software that helped Amazon sellers create and schedule discounts on Amazon products
                        </p>
                        <br>
                        <lu>
                            <li>Completed features in web application that went into production, which assisted customers with various tasks.</li>
                            <li>To complete features, I worked on creating APIs that called a database and UI components to use these APIs.</li>
                            <li>Wrote unit tests and integration tests for all APIs and functions created.</li>
                            <li>Worked with a team using agile development approach.</li>
                        </lu>
                        <p class="timeline-subtitle">July 2022 - August 2022</p>
                    </div>
                </div>
            </div>
        </div>
    </body>

</template>

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css?family=Niramit:300,300i,700');

// reset some browser default styles
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

// colors
$primary: #1d8cf8;
$secondary: #4f537b;
$info: #11cdef;
$success: #00bf9a;
$warning: #ff8d72;
$danger: #fd5d93;

// timeline variables
$body-bg: #1e1e2f;
$timeline-before-bg : #222a42;
$timeline-body-bg: #27293d;
$timeline-body-round: 3px;
$timeline-body-shadow: 1px 3px 9px rgba(0,0,0, .1);

body {
    font-family: 'K2D', sans-serif;
    letter-spacing: 1px;
}

// page container
.container {
    max-width: 650px;
    margin: 50px auto;
}

// typography
p {
    font-weight: 300;
    line-height: 1.5;
    font-size: 14px;
    opacity: .8;
}

// timeline style
.timeline {
    position: relative;
    padding-left: 4rem;
    margin: 0 30px  30px;
    color: white;

    &:before {
        content: '';
        position: absolute;
        left: 0;
        top: 0;
        width: 4px;
        height: 100%;
        background: $timeline-body-bg;
    }

    .timeline-container {
        position: relative;
        margin-bottom: 2.5rem;;

        .timeline-icon {
            position: absolute;
            left: -88px;
            top: 4px;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            text-align: center;
            font-size: 2rem;
            background: $secondary;

            i {
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, -50%);
            }

            img {
                width: 100%;
                height: 100%;
                border-radius: 50%;
            }
        }

        .timeline-body {
            background: $timeline-body-bg;
            border-radius: $timeline-body-round;
            padding: 20px 20px 15px;
            box-shadow: $timeline-body-shadow;

            &:before {
                content: '';
                background: inherit;
                width: 20px;
                height: 20px;
                display: block;
                position: absolute;
                left: -10px;
                transform: rotate(45deg);
                border-radius: 0 0 0 2px;
            }

            .timeline-title {
                margin-bottom: 1.4rem;

                .badge {
                    background: $secondary;
                    padding: 4px 8px;
                    border-radius: 3px;
                    font-size: 12px;
                    font-weight: bold;
                }
            }

            .timeline-subtitle {
                font-weight: 300;
                font-style: italic;
                opacity: .4;
                margin-top: 16px;
                font-size: 11px;
            }
        }

        // Primary Timeline
        &.primary {
            .badge,
            .timeline-icon {
                background: $primary !important;
            }
        }

        // Info Timeline
        &.info {
            .badge,
            .timeline-icon {
                background: $info !important;
            }
        }

        // Success Timeline
        &.success {
            .badge,
            .timeline-icon {
                background: $success !important;
            }
        }

        // Warning Timeline
        &.warning {
            .badge,
            .timeline-icon {
                background: $warning !important;
            }
        }

        // Dnager Timeline
        &.danger {
            .badge,
            .timeline-icon {
                background: $danger !important;
            }
        }

    }
}


.author{
	font-family: inherit;
	padding: 3em;
	text-align: center;
	width: 100%;
		color: white;
 
	a:link,
	a:visited{
		color: white;
		&:hover{
			text-decoration: none;
		}
	}
	.btn:link,
	.btn:visited{
		margin-top: 1em;
		text-decoration: none;
		display: inline-block;
		font-family: inherit;
		font-weight: 100;
		color: white;
		text-align: center;
		vertical-align: middle;
		user-select: none;
		background-color: black;
		padding: 1.5em 2rem;
		border-radius: 1em;
		transition: .5s all;
		&:hover,
		&:focus,
		&:active{
			background-color: lighten(black, 10%);
		}
	}
}
    .pic{
        width: 400px;
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;
    }
    
    .jobs{
        text-align: center;
        background-color: #F8F1F1;
        margin: auto;
        margin-top: 20px;
        width: min(90%, 1200px);
        border-radius: 10px;
    }
</style>