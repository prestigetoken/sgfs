

 <html>

<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
        }
        /* Full-width input fields */
        
        input[type=text],
        input[type=password] {
            width: 100%;
            padding: 12px 20px;
            margin: 8px 0;
            display: inline-block;
            border: 1px solid #ccc;
            box-sizing: border-box;
        }
        /* Set a style for all buttons */
        
        button {
            background-color: #4CAF50;
            color: white;
            padding: 20px 40px;
            margin: 8px 0;
            border: none;
            cursor: pointer;
            width: 100%;
        }
        
        button:hover {
            opacity: 0.8;
        }
        /* Extra styles for the cancel button */
        
        .cancelbtn {
            width: auto;
            padding: 10px 18px;
            background-color: #f44336;
        }
        /* Center the image and position the close button */
        
        .imgcontainer {
            text-align: center;
            margin: 24px 0 12px 0;
            position: relative;
        }
        
        img.avatar {
            width: 40%;
            border-radius: 50%;
        }
        
        .container {
            padding: 16px;
        }
        
        span.psw {
            float: right;
            padding-top: 16px;
        }
        /* The Modal (background) */
        
        .modal {
            display: none;
            /* Hidden by default */
            position: fixed;
            /* Stay in place */
            z-index: 1;
            /* Sit on top */
            left: 0;
            top: 0;
            width: 100%;
            /* Full width */
            height: 100%;
            /* Full height */
            overflow: auto;
            /* Enable scroll if needed */
            background-color: rgb(0, 0, 0);
            /* Fallback color */
            background-color: rgba(0, 0, 0, 0.4);
            /* Black w/ opacity */
            padding-top: 60px;
        }
        /* Modal Content/Box */
        
        .modal-content {
            background-color: #fefefe;
            margin: 5% auto 15% auto;
            /* 5% from the top, 15% from the bottom and centered */
            border: 1px solid #888;
            width: 80%;
            /* Could be more or less, depending on screen size */
        }
        /* The Close Button (x) */
        
        .close {
            position: absolute;
            right: 25px;
            top: 0;
            color: #000;
            font-size: 35px;
            font-weight: bold;
        }
        
        .close:hover,
        .close:focus {
            color: red;
            cursor: pointer;
        }
        /* Add Zoom Animation */
        
        .animate {
            -webkit-animation: animatezoom 0.6s;
            animation: animatezoom 0.6s
        }
        
        @-webkit-keyframes animatezoom {
            from {
                -webkit-transform: scale(0)
            }
            to {
                -webkit-transform: scale(1)
            }
        }
        
        @keyframes animatezoom {
            from {
                transform: scale(0)
            }
            to {
                transform: scale(1)
            }
        }
        /* Change styles for span and cancel button on extra small screens */
        
        @media screen and (max-width: 300px) {
            span.psw {
                display: block;
                float: none;
            }
            .cancelbtn {
                width: 100%;
            }
        }
    </style>
</head>

<body>


    <button onclick="document.getElementById('id01').style.display='block'" style="width:auto;">Login</button>

    <div id="id01" class="modal">

        <form class="modal-content animate" action="/action_page.php">
            <div class="imgcontainer">
                <span onclick="document.getElementById('id01').style.display='none'" class="close" title="Close form">&times;</span>
                <img src=" " alt="Please Login" class="avatar">
            </div>

            <div class="container">
                <label for="uname"><b>Username</b></label>
                <input type="text" placeholder="Enter Username" name="uname" required>

                <label for="psw"><b>Password</b></label>
                <input type="password" placeholder="Enter Password" name="psw" required>

                <button type="submit">Login</button>
                <label>
        <input type="checkbox" checked="checked" name="remember"> Remember me
      </label>
            </div>

            <div align="center" class="container" style="background-color:#f1f1f1">
                <button type="button" onclick="document.getElementById('id01').style.display='none'" class="cancelbtn">Cancel</button>
            </div>
        </form>
    </div>

    <script>
        // Get the modal
        var modal = document.getElementById('id01');

        // When the user clicks anywhere outside of the modal, close it
        window.onclick = function(event) {
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
    </script>

</body>

</html>






























<h1>         </h1>
 <h1>         </h1>
 <h1>         </h1>
  <div>
 <html>
 <head>
<style>
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}

li {
    float: left;
}

li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}

li a:hover:not(.active) {
    background-color: #111;
}

.active {
    background-color: #7ffffd;
}
 </style>
 </head>
 <body>

 <ul>
  <li><a class="active" href="sgfs">Home</a></li>
  <li><a href="about.html">About</a></li>
</ul>

</body>
</html>
 </div>
 
 
 
 
 
 
 
 
 
 
  <p style="color:red;">
Play the Snake Game For Free
   </p>
   <p style="color:aqua;">
  With out it being blocked
    </p>
  <p style="color:purple;">
  @Squid Man </p>
<p sytle="color:purple;"><a href="https://discord.gg/cjVRptT">Visit the discord server</a></p>    
  <p style="color:purple;"> DONT GET COUGHT PLAYING OR IT MIGHT GET BLOCKED!</p>
 

 
 <html>
 <head>
  <title>Snake</title>
  <style>
  html, body {
    height: 100%;
    margin: 0;
  }
   body {
    background: white;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  canvas {
    border: 2px solid black;
  }
  </style>
</head>
<body>
<canvas width="400" height="400" id="game"></canvas>
<script>
var canvas = document.getElementById('game');
var context = canvas.getContext('2d');
var grid = 16;
var snake = {
  x: 160,
  y: 160,
  dx: grid,
  dy: 0,
  cells: [],
  maxCells: 4
};
var count = 0;
var apple = {
  x: 320,
  y: 320
};
function getRandomInt(min, max) {
  return Math.floor(Math.random() * (max - min)) + min;
}
// game loop
function loop() {
  requestAnimationFrame(loop);
  // slow game loop to 15 fps instead of 60 - 60/15 = 4
  if (++count < 4) {
    return;
  }
  count = 0;
  context.clearRect(0,0,canvas.width,canvas.height);
  snake.x += snake.dx;
  snake.y += snake.dy;
  // wrap snake position on edge of screen
  if (snake.x < 0) {
    snake.x = canvas.width - grid;
  }
  else if (snake.x >= canvas.width) {
    snake.x = 0;
  }
  if (snake.y < 0) {
    snake.y = canvas.height - grid;
  }
  else if (snake.y >= canvas.height) {
    snake.y = 0;
  }
  // keep track of where snake has been. front of the array is always the head
  snake.cells.unshift({x: snake.x, y: snake.y});
  // remove cells as we move away from them
  if (snake.cells.length > snake.maxCells) {
    snake.cells.pop();
  }
  // draw apple
  context.fillStyle = 'red';
  context.fillRect(apple.x, apple.y, grid-1, grid-1);
  // draw snake
  context.fillStyle = 'green';
  snake.cells.forEach(function(cell, index) {
    context.fillRect(cell.x, cell.y, grid-1, grid-1);
    // snake ate apple
    if (cell.x === apple.x && cell.y === apple.y) {
      snake.maxCells++;
      apple.x = getRandomInt(0, 25) * grid;
      apple.y = getRandomInt(0, 25) * grid;
    }
    // check collision with all cells after this one (modified bubble sort)
    for (var i = index + 1; i < snake.cells.length; i++) {
      
      // collision. reset game
      if (cell.x === snake.cells[i].x && cell.y === snake.cells[i].y) {
        snake.x = 160;
        snake.y = 160;
        snake.cells = [];
        snake.maxCells = 4;
        snake.dx = grid;
        snake.dy = 0;
        apple.x = getRandomInt(0, 25) * grid;
        apple.y = getRandomInt(0, 25) * grid;
      }
    }
});
}
document.addEventListener('keydown', function(e) {
  // prevent snake from backtracking on itself
  if (e.which === 37 && snake.dx === 0) {
    snake.dx = -grid;
    snake.dy = 0;
  }
  else if (e.which === 38 && snake.dy === 0) {
    snake.dy = -grid;
    snake.dx = 0;
  }
  else if (e.which === 39 && snake.dx === 0) {
    snake.dx = grid;
    snake.dy = 0;
  }
  else if (e.which === 40 && snake.dy === 0) {
    snake.dy = grid;
    snake.dx = 0;
  }
});
requestAnimationFrame(loop);
</script>
</body>
</html>

<html>
<body>

   
<h1 style="color:black;" align="center" id="demo"></h1>



<script>
var myVar = setInterval(myTimer, 1000);

function myTimer() {
    var d = new Date();
    document.getElementById("demo").innerHTML = d.toLocaleTimeString();
}
</script>

</body>
</html>

<p style="color:grey;">
  Made By Dale O'Beirne
    </p>

