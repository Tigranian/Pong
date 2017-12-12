<!doctype html> 
<html lang="en">
<head>
    <title>PingPong</title>
    <style>
        #canvasboard {
            margin: auto;
            position: absolute;
            top: 0;
            bottom: 0;
            left: 0;
            right: 0;
            background-image: url("https://www.walldevil.com/wallpapers/w07/simple-simple-background-hd-background.jpg");
            background-size: 100% 100%;
        }

    </style>

</head>

<body>
    <canvas id="canvasboard" width=550 height=300></canvas> 
    <canvas id="canvasbackground" width=1500 height=500></canvas>
    
    <script> 

      const rand = function (num) {
        return  + 1;
      };

      
      const gameboard = document.getElementById('canvasboard');
      const canvasboard = gameboard.getContext('2d');
      const bkgr = document.getElementById('canvasbackground');
      const canvasbackground = bkgr.getContext('2d');
      
      var boardw = gameboard.width;
      var boardh = gameboard.height;
      var bckgrw = bkgr.width;
      var bckgrh = bkgr.height;
      
      
      const RectCircleIntersection = function(rectX, rectY, rectW, rectH, circleX, circleY, circleR) {
        const deltaX = circleX - Math.max(rectX, Math.min(circleX, rectX + rectW));
        const deltaY = circleY - Math.max(rectY, Math.min(circleY, rectY + rectH));
        return (deltaX * deltaX + deltaY * deltaY) < (circleR * circleR);
      };
      
      const gameData = {};
      gameData.player1 =
        {
          x: 30,
          y: (boardh / 2) - 25,
          width: 10,
          height: 50,
          yDelta: 15,
       
        }      
      gameData.player2 = 
        {
          x: boardw - 40,
          y: (boardh / 2) - 25,
          width: 10,
          height: 50 ,
          yDelta: 15,
         
        };     
      gameData.ball = [{
        
        x: boardw / 2,
        y: boardh / 2,
        r: 15,
        xDelta : 10,
        yDelta : 10,
        color : 'red'
        }
      ]
    

var player1score = 0;
var player2score = 0;
var ballcount = 0; 
var random = 0;

      const forEach = function ( ball , f ) {
        for ( i = 0; i < ball.length; i++){
          f(ball[i]);
        } 
      };
      const add1 = function() {
        gameData.ball.push ({
          
          x: boardw / 2,
          y: boardh / 2,
          r: 15,
          xDelta : 10,
          yDelta : 10,
          color : 'red'
          
        });
        return;
      };
      
      
      const update = function () {

        forEach(gameData.ball, function(ball) {
          
          if (ball.y + ball.yDelta > boardh - ball.r || ball.y + ball.yDelta < ball.r) {
            ball.yDelta = -ball.yDelta;
          }
          if (RectCircleIntersection(gameData.player1.x, gameData.player1.y, gameData.player1.width, gameData.player1.height, ball.x, ball.y, ball.r)) {
            ball.xDelta = Math.abs(ball.xDelta);
            if(keyPressed[w]) {
              ball.yDelta = -Math.abs(ball.yDelta);
            } else if(keyPressed[s]) {
              ball.yDelta = Math.abs(ball.yDelta);
            }
          }
          if (RectCircleIntersection(gameData.player2.x, gameData.player2.y, gameData.player2.width, gameData.player2.height, ball.x, ball.y, ball.r)) {
            ball.xDelta = -1 * Math.abs(ball.xDelta);
            if(keyPressed[downKey]) {
              ball.yDelta = Math.abs(ball.yDelta);
            } else if(keyPressed[upKey]) {
              ball.yDelta = -Math.abs(ball.yDelta);
            }
          }

          ball.x += ball.xDelta;
          ball.y += ball.yDelta;
          
        }) 


        for (i = 0; i < gameData.ball.length ; i++){
          if (gameData.ball[i].x + gameData.ball[i].xDelta > boardw - gameData.ball[i].r) {
         
          var removed = gameData.ball.splice(i, 1);
          return player1score++,removed,ballcount--;
          }
          
          if (gameData.ball[i].x + gameData.ball[i].xDelta < gameData.ball[i].r) {
      
            var removed = gameData.ball.splice(i, 1);
          return player2score++,removed,ballcount--;
          }
        }

      };

      const draw = function () {

        canvasbackground.clearRect(0, 0, bckgrw, bckgrh);
        canvasboard.clearRect(0, 0, boardw, boardh);

        canvasbackground.fillStyle = 'red';
          canvasbackground.font = "100px Primitive";
          canvasbackground.fillText(player1score , 500 , 100 );
          canvasbackground.fillText(player2score , 800 , 100 );

          canvasbackground.fillStyle = 'red';
          canvasbackground.font = "45px Primitive";
          canvasbackground.fillText(' Balls', 20 , 790 ); 
          
        
        forEach(gameData.ball, function(ball){
          canvasboard.beginPath();
          canvasboard.fillStyle = 'red';
          canvasboard.arc(ball.x, ball.y, ball.r, 0, 2 * Math.PI, false);
          
          canvasboard.fill(); 
        });
        
        canvasboard.fillStyle = 'red';
        canvasboard.fillRect(gameData.player1.x, gameData.player1.y, gameData.player1.width, gameData.player1.height);
        
        canvasboard.fillStyle = 'red';
        canvasboard.fillRect(gameData.player2.x, gameData.player2.y, gameData.player2.width, gameData.player2.height);
        
        
        
      };
      
      const w = 87;
      const s = 83;
      const upKey = 38;
      const downKey = 40; 
      const space = 32; 
      const keyPressed = {}
      
      document.addEventListener('keydown', function(event) {
        keyPressed[event.keyCode] = true;
        event.preventDefault()
        if(event.keyCode === space){
          add1(); 
        }
      }, false);
      document.addEventListener('keyup', function(event) {
        keyPressed[event.keyCode] = false;
        event.preventDefault()
      }, false);
      
      
      const loop = function () { 
        
        // PLayer 1
        if(keyPressed[w] && gameData.player1.y > 0) {
          gameData.player1.y -= gameData.player1.yDelta;
        } 
        
        if(keyPressed[s] && gameData.player1.y + gameData.player1.height < boardh ) {
          gameData.player1.y += gameData.player1.yDelta;
        }
        
        // Player 2 
        
        if(keyPressed[upKey] && gameData.player2.y > 0) {
          gameData.player2.y -= gameData.player2.yDelta;
        } 
        
        if(keyPressed[downKey] && gameData.player2.y + gameData.player2.height < boardh ) {
          gameData.player2.y += gameData.player2.yDelta;
        }
        
        update();
        draw ();
        
        
        window.requestAnimationFrame(loop);
      };
      
      loop(); 
      
    </script>
    
  </body>