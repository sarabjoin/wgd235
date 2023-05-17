
<html>

<head>
    <title>Week 2 Lab</title>

    <style>
        img{
            width: 50px;
        }

        body{
            background-color: #e4e4e4;
            padding: 0;
            margin: 0;
        }

        #container, h1, footer{
            margin: 20px;
            width: 97%;
            text-align: center;
        }

        .animations{
            margin: 20px;
            padding: 16px;
            height: 300px;
            border: 1px solid gray;
            border-radius: 15px;
            background-color: #f5f5f0;
        }

        .separator{
            height:15px;
        }

        .transitions{
            margin: 20px;
            padding: 16px;
            border: 1px solid gray;
            border-radius: 15px;
            background-color: #f5f5f0;
            text-align: left;
        }

        #btn1{
            width: 55px;
            height: 55px;
            display: inline-block;
            background-color: cornflowerblue;

            transition: all 0.1s ease-in-out;
            transform: translate3d(0, 0, 0)
        }

        #btn1:hover{
            cursor: pointer;
            background-color: #00ff00;
        }

        #btn2{
            width: 55px;
            height: 55px;
            display: inline-block;
            background-color: cornflowerblue;

            transition: all 0.1s ease-in-out;
            transform: translate3d(0, 0, 0);
        }

        #btn2:hover{
            cursor: pointer;
            filter: drop-shadow(8px 8px 5px gray);
        }

        #btn3{
            width: 55px;
            height: 55px;
            display: inline-block;
            background-color: cornflowerblue;

            transition: all 0.1s ease-in-out;
            transform: translate3d(0, 0, 0);
        }

        #btn3:hover{
            cursor:crosshair;
            transform: scale(1.5);
            background-color: fuchsia;
        }

        #btn4{
            width:55px;
            height:55px;
            display: inline-block;
            background-color: cornflowerblue;

            transition: all 0.1s ease-in-out;
            transform: translate3d(0, 0, 0);
        }

        #btn4:hover{
            cursor:grab;
            transform: scale(-0.5);
            filter:hue-rotate(120deg) drop-shadow(6px 8px 13px yellow);
            
        }

        #ball{
            width:50px;
            height: 50px;
            border-radius: 50%;
            background-color: #ff5722;
            display: inline-block;
            animation: bounce .5s;
            animation-direction: alternate;
            animation-timing-function: cubic-bezier(.5, 0.05, 1, .5);
            animation-iteration-count:infinite;
        }

        @keyframes bounce{
            from{
                transform: translate3d(0, 0, 0);
            }
            to{
                transform: translate3d(0, 275px, 0);
            }
        }
    </style>

</head>

<body>
    <h1>TIMING FUNCTIONS</h1>
    <div id="container">
        <h2>HOVER EFFECTS</h2>
        <div class="transitions">
            <div id ="btn1"></div>
            <div id ="btn2"></div>
            <div id="btn3"></div>
            <div id="btn4"></div>
        </div>

        <div class="separator"></div>

        <h2>MOVEMENT EFFECTS</h2>
        <div class="animations">
            <div id="ball"></div>
        </div>

    </div>
    <footer>Copyright 2018</footer>
</body>

</html>
