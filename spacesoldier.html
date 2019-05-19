<!DOCTYPE HTML>
<html lang="en-US">

<head>
    <meta charset="UTF-8">
    <title>Space Soldier</title>
    <script type="text/javascript" src="simpleGame.js"></script>
    <script type="text/javascript">
        var game;
        var ship;
        var bg;
        var missile;
        var meteor;
        var enemy;
        var score=0;
        var fireMissile;
        var boomsound;
        var enginesound;
        function init() {
            buildSounds();
            game = new Scene();
            bg = new Sprite(game,"bg.jpg",1200,800);
            bg.setSpeed(0);
            ship = new Ship();
            missile = new Missile();
            setMeteor();
            setEnemy();
            game.start();
        } // end init
        buildSounds = function () {
            fireMissile = new Sound("missile.wav");
            boomsound = new Sound("boom.wav");
            enginesound = new Sound("engine.wav");
        }
        function setMeteor(){
            meteor = new Array(3);
            for (var i = 0; i < 3; i++) {
                meteor[i] = new Meteor();
            }
        }
        function Meteor(){
            tMeteor = new Sprite(game,"meteor.png",50,50);
            tMeteor.setAngle(180);
            tMeteor.setSpeed(8);
            tMeteor.reset = function(){
                tMeteor.setPosition(Math.random()*1200,0);
            }
            tMeteor.reset();
            return tMeteor;
        }
        function setEnemy(){
            enemy = new Array(6);
            for (var i = 0; i < 6; i++) {
                enemy[i] = new Enemy();
            }
        }
        function Enemy(){
            tEnemy = new Sprite(game,"enemy.png",70,70);
            tEnemy.setAngle(180);
            tEnemy.setSpeed(3);
            tEnemy.reset = function(){
                tEnemy.setPosition(Math.random()*1200,0);
            }
            tEnemy.reset();
            return tEnemy;
        }
        function Ship() {
            tShip = new Sprite(game, "ship.png", 100, 100);
            tShip.setPosition(400,550);
            tShip.setSpeed(0);
            tShip.hSpeed = 0;
            tShip.checkKeys = function () {
                if (keysDown[K_SPACE]) {
                    fireMissile.play();
                    missile.fire();
                }if (keysDown[K_LEFT]) {
                    if (this.hSpeed < -15) {
                        this.hSpeed = -15;
                    } else {
                        this.hSpeed -= 2;
                    }
                }if (keysDown[K_RIGHT]) {
                    if (this.hSpeed > 15) {
                        this.hSpeed = 15;
                    } else {
                        this.hSpeed += 2;
                    }
                }
                this.changeXby(this.hSpeed);
            }
            return tShip;
        }
        function setMissile(){
            missile = new Array(100);
            for (var i = 0; i < 100; i++) {
                missile[i] = new Missile();
            }
        }
        function Missile(){
            tMissile = new Sprite(game,"bullet.png",40,40);
            tMissile.setAngle(0);
            tMissile.hide();
            tMissile.fire = function(){
                this.show();
                this.setSpeed(20);
                this.setPosition(ship.x,ship.y);
                this.setAngle(-1)
                this.setBoundAction(DIE);
            }
            return tMissile;
        }
        function update() {
            enginesound.play();
            game.clear();
            bg.update();
            ship.update();
            ship.checkKeys();
            missile.update();
            for (var i = 0; i < 3; i++) {
                if(meteor[i].y >= 600){
                    meteor[i] = new Meteor();
                }
                if(ship.collidesWith(meteor[i])){
                    boomsound.play();
                    game.stop();
                    alert("You lose");
                    break;
                }
                meteor[i].update();
            }
            for (var i = 0; i < 6; i++) {
                if(enemy[i].y >= 600){
                    enemy[i] = new Enemy();
                }if(missile.collidesWith(enemy[i])){
                    boomsound.play();
                    score++;
                    enemy[i] = new Enemy();
                }if(ship.collidesWith(enemy[i])){
                    boomsound.play();
                    game.stop();
                    alert("You lose");
                    break;
                }
                enemy[i].update();
            }
            updatescore();
        }
        function updatescore(){
            var s = document.getElementById("score");
            s.innerHTML="Score : "+score;
        }
        function restart(){
            window.location.href = "spacesoldier.html"
        }
    </script>
</head>

<body onload="init()">
<div id="score">Score : 0</div><br>
<button onclick="restart()">RESTART</button><br>
</body>

</html>