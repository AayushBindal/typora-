# my daily notes



## Pong Game 

#### day 0 

I learnt how to built rectangles using p5 editor 

    rect(xPosition,yPosition,width,height);     // to create a rectangle



#### day1

I learnt how to write a code using oops (object oriented programming) in p5.editor

    class class_name
    {
        constructor(){
         this.xPosition=?;
         this.yPosition=?;
         this.width=?;
         this.height=?;
        }
        
        display(){
         rect(this.xPosition,this.yPosition,this.width,this.height);
        }
    }
    
    var variable_name;
    function setup(){
        createCanvas(width,height);
        variable_name=new class_name();
    }
    function draw(){
        background("color");
        variable_name.xPosition=?;
        variable_name.yPosition=?;
        variable_name.display();
    }



#### day2

I learnt using cord.org the code 

    //comments to make readable the code
    
        var variable_name(X_Axis,Y_Axis,Width,height);
        object.velocityX=?;
        object.velocityY=?;
        
        sprite.bounceOff(target);  	 // to let sprite only move
        sprite.bounce(target); 		 // to let sprite and target both move 
     function draw(){
        background("color"); 		 // to add background 
        createEdgeSprite(); 	     // to create edges 
        sprite.shapeColor= "white";  // to have any sprite colored  
        sprite.positionY=?;   		 // to change the Y position of a sprite
        drawSprites();
     }



#### day3

I learnt to put conditions to the program by using if in function draw and also I learnt many small functions in code.org

    function draw(){
        textSize(?); 										// to have a text size 						
    	textFont(?);										// to have a text font 
        text("text",X_Axis,Y_Axis);							// to have a text 
        noFill();											// to fill no color in any shape 
        fill("color");										// to fill color in text
        stroke("color");									// to fill color in outline in any text
        
      if(situation){                                      
          the result
        }
        if(keyDown/keyWentDown/KeyWentUp("key")){
          the result 
        }
    }





#### day4

I learnt small functions like RGB and have a practice of previous concepts in code.org

    function draw(){
       rgb("theRedColor","theGreenColor","theBlueColor")    		//to add color of different types
        //the color shouldn't extend 225
    }



#### day5

I learnt about functions and loops  in code.org

    //to call function
    
    function function_name(){       			
      //body of the function for ex-
       sprite.bounceoff(target);
    }
    
    function draw(){
        function_name();
    }
    
    for(var variable_name relation value?,variable_name _relation_value,variable_name = variable_name+ value?){   //order to computerto execute a line no of times;
     }
        ( note--value can be different and relation means +,=,>,< etc.) for ex-
          
    for(var i=10,i>400,i=i+20){
        text("text",X_Axis,Y_Axis);
    } 
    function draw(){
        //other code
    }



#### day6

I learnt to store different game states in a variable and to make 2 player games in code.org

    var gameState = name_of_gameState;           
    // for ex-
    var gameState = serve;
    function draw(){
        //other code 
        gameState===serve                        // to compare a thing we use 3 equal to 
    }



#### day7

I learnt to have different animations and sounds in code.org

    var variable_name(X_Axis,Y_Axis,width,height)   					// to create a sprite
        variable_name.setAnimation("url_of_animation");                 // to label any sprite    
    
    function draw(){
        //other code
    }
    
    function draw(){
        if(situation){
           playSound("url", false/true);
           }
    }
    (note-true will repeat the sound forever and for that you need not to write that in if condition)



#### day8

I learnt to create the world hardest game in code.org and setting scale in code.org

    //create the game such that it is impossible to win for the player  
    
    var variable_name(X_Axis,Y_Axis,width,height)					   // to create a sprite
    																   // more obstacles 
    function draw(){
        background("color");										   // to have a background 
        variable_name.velocityX/Y=?;								   // try to put a lesser value for player 
        sprite.scale=?;												   // to have a scale 
        drawSprites();                                                 // to draw sprites 
    }



## T-rex dinosaur game 

#### day9

I learnt to create infinite screen game , T-rex ,to have an animation,images etc. with p5.editor

    var variable_name1,variable_name2                                   // to have 2 variable for same 
    var variable_name3,variable_name4									// to have 2 variable for same 
    
    function preload(){
        //load animations here                                          
        variable_name1 = loadAnimation("file_name");
        //load images here
        variable_name3 = loadImage("file_name");
    }
    function setup(){
        createCanvas(width,height);
        //add animations here 
        variable_Name2 = createSprite(X_Axis,Y_Axis,width,height);
        variable_Name2.addAnimation("description",variable_name1);
        //add images here
        variable_name4 = createSprite(X_Axis,Y_Axis,width,height);
        variable_name4.addImage("description",variable_name3);
    }
    function draw(){
        //add background 
        background("color");
        //draw sprites
        drawSprites();
    }
    
    //to add gravity to trex
    trex.y = trex.y+value?;

````javascript
// to create edge sprites 
var variable_name   									// for assigning 
var variable_name2										// for edge sprites
function preload(){
    createCanvas(width,height)	
}
function draw(){
    variable_name = createEdgeSprites();				// to create edge sprites 
    variable_name2 _relation_ edge[1], edge[2]          // so on
}
````







#### day10

I learnt to intend the code and to fix 2 minor bugs in Trex game. Also to use console command in a different way  in p5.editor

     to add comments put 2 forward slashes so that computer doesn't read the statement
    // comment
    
       var variable_name(X_Axis,Y_Axis,width,height)
    function function_name(){
    tab//code1               
            //code1
            //code1
    
            //code2
            //code2
            //code2
    
            //code3
            //code3
            //code3
    }
    
    //to move trex on ground 
    var invisibleGround 
    function setup(){
        invisibleGround = createSprite(X_Axis,Y_Axis,width,height);
        invisibleGround.visible = false;
    }
    
    function draw(){
        trex.collide(invisibeGround)
    }
    
    //to have spacebar only once 
    function draw (keyDown(space) && trex.y<value){
        trex.y = -10;
    }
    
    //to use console 
    function draw(){
        console.time();
        //code
        console.timeEnd();
    }



#### day11

I learnt to add loops in different variable and to create random numbers and through them to create different values .

Also to have frame gap between clouds and to have them at different Y_Axis and the depth concept.

    //to create loops 
    var variable_name1
    var variable_name2
    
    function preload(){
        variable_name1.loadImage("file_name")   
    }
    function setup(){
       for(var i relation value?,i _relation_value,i = i+ value?) {
        variable_name2 = createSprite(X_Axis,Y_Axis,width,height);
        variable_name2.addImage("description",variable_name1);
        variable_name2.scale = value?;
        }
    }
    function draw(){
       background("color");
       drawSprite();
    }
    
    //for generating a random number and assigning to a variable 
    var variable_name	//for random
    var variable_name2	//for assigning 
    var variable_name3  
    
    function preload(){
      variable_name2 = loadImage("file_name")
    }
    function setup(){
      var variable_name = maths.round(random(least value, highest value))
      console.log(variable_name) //for checking
    }
    function draw(){
        background("color");
        if(divisor % dividend === remainder){
           assign(); 
         }
        drawSprite();
    }
    function assign(){
       variable_name3 = createSprite(X_Axis,Y_Axis,width,height);
       variable_name3.addImage("description",variable_name2);
       variable_name3.y = math.round(variable_name(least value, highest value));
       variable_name3.velocityX = value?;  
    }
    
    //for depth
    var variable_name
    var variable_name2
    
    function setup(){
      variable_name = createSprite(X_Axis,Y_Axis,width,height);
      variable_name2 = createSprite(X_Axis,Y_Axis,width,height);
    }
    function draw(){
      drawSprite();
      variable_name.depth = variable_name2.depth +1;
    }



#### day 12 

I learnt to give lifetime of any object , the string concatenation and switch statement.

````javascript
function draw(){
    object.lifetime = value?_time;    		// time is in milisecond
}
````

````javascript
// to add more statement for only text
function draw(){
	text("text" +variable_name,X_Axis,Y_axis)
}
````



#### day 13 

I learnt to create different states and group to assign them different behavior  and, if and else if condition.

````javascript
// to create different states 
var variable_name = value;                            // value like 0,1,2,3 etc.
var variable_name2 = value;                           // value like 0,1,2,3 etc.
var gameState = variable_name						  // the state which is at initial position 
````

````javascript
//to declare a group 
var group_name1										  // create the variable name for group name 
var group_name2 									  // create the variable name for group name 2 
function setup (){
    group_name1 = new Group();
    group_name2 = new Group();
}

function draw (){
    // to add a sprites to a group
       group_name1.add(spriteName);
    // to remove a sprite from a group 
       group_name1.remove(spriteName);
    // to clear a group but not it's sprite
       group_name1.clear();
    
    // to assign a single behavior and gameState to a group 
    if(group1._relation_group_name2){
       result 
       }												// for ex-
    if(group1.isTouching(group2)){
       gameState = end;
       }
}
````

````javascript
// to use if,else if statement 
var variable_name = value;                            // value like 0,1,2,3 etc.
var variable_name2 = value;                           // value like 0,1,2,3 etc.
var gameState = variable_name	        			  // the state which is at initial position 

function setup() {
    // other code 
}

function draw() {
    if( condition){
       result 
       }
    else if (another condition) {
        another result    
            }
    // the situation which will happen all thw time will be written outside this condition
}

````

````javascript
// to have single behavior to a group 		
function draw() {
    group_name1._behavior_each();
    // for ex- 
    group_name1.setVelocityEach(value);
    group_name2.destroyEach();
}
````



#### day 14 

I learnt to fix some bugs in our game by setting collider at different parameters 

````javascript
// to set collider 
var variable_name
var variable_name2
function setup(){
    variable_name2.setCollider(rectangle,xOffset,yoffset,width,height)	// for rectangle		
    variable_name2.debug = true;										// to display collider 
    variable_name.setCollider(circle,xOffset,yOffset,radius) 		    // for circle 
    variable_name.debug = true;										   	// to display collider  
}
function draw (){
    // other code 
}
````



#### day 15

I learnt to add sounds, to let the T-rex jump when it touches the cactus 

````javascript
// to add sounds 
var sound_name1;
var sound_name2;

function preload(){
    sound_name1 = loadSound("url of the sound");
    sound_name2 = loadSound("url of the sound");
}
function setup(){
    // other code 
}
function draw(){
    if(condition){
       sound_name1.play();
       sound_name2.play();
       }
}
````

````javascript
// to assign AI T-rex jump 
function setup(){
   variable_name1.setCollider("shape",xOffset,yoffset,width,height);      
   variable_name1.debug = true;
}
function draw(){
    if(variable_name1.isTouching(variable_name2)){
        variable_name1.velocityY = value?;
    }
}
````



#### day 16

I learnt the scope of local and global variable , and a function mousePressedOver 

local scope variable is a type of variable in which the variable is accessed by a particular function in which it is declared 

while in the global scope variable all functions are able to access it as it is declared on the top

````javascript
// to make restart button functional 
if(mousePressedOver(variable)) {
   // the result which you want 
   }
````



#### day 17 

I leant to work our code on local machine and to host our game online

````javascript
// to work oue code on local machine from p5.editor
1). Open p5 editor and in it open your project. From the file option download the file in a new folder with 	a name so there is no confution.
2). Extract all the files in that folder and delete the file from you extracted it 
3). Go to chrome and there( https://chrome.google.com/webstore/detail/web-server-for-			                 chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb?hl=en ) open the chrome web store and add 200 ok web server and 	 launch it.
4). Go to choose folder option and in dialog box select the file you want.
5). There will be a link provided under web server's url(s) click on that and enjoy your game in your 	         browser.
````

````javascript
// to host our game online via Github 
Now we have downloaded our game on our system so,
1). Go to github search in chrome and create an account and fill all the details in it with a safe account 
2). If already account is created then login to it (https://github.com/).
3). Click on start a project.
4). See weather owner name is correct and then type resporatory name (project name) and click on private 	     option or on public option. Then add a readme file and then click on create resporatory. 
5). Inside code add that file then go to make changes after that your all the files will be saved in code       option and then go to settings and then in settings option go to Githhub pages select main as branch and 
    then root one and click on save.
6). A link will appear there. Click on that and your game will be hosted online.

````



#### day 18 

I learnt to fit my game to all sizes, to use Thunkable and arrays

````javascript
// to fit your game all sizes 
// to fit the game according to the width of device use windowWidth
// to fit the game according to the height of device use windowHeight
for ex -
createCanvas(windowWidth,windowHeight);
variable_name.lifetime = Width-value?
etc.
````

````javascript
Array is a group of many things 
The number of elements present in a array is it's length and the position of the 1st element is 0 wheras the position of the last element is length-1.
to empty the array for once we use a predefined function array = []
````

````javascript
// to use thunkable 
Open thunkable and login/signup there 
(https://x.thunkable.com/projects)
 create a new project and then start
````

#### day 19

I made a ghost runner game through p5.editor 

````javascript
It is as same as t-rex game (for hints see from day 9)
````

#### visual code studio

#### day 20

I leant to design Alogrithms (designing our own command)

````javascript
// to design isTouching command

var variable_name1;
var variable_name2;
function setup(){
    createCanavs(width,height);
    variable_name1 = createSprite(X_Axis,Y_Axis,width,height);
    variable_name1.shapeColor = "color";
    variable_name1.debug = true;
    
    variable_name2 = createSprite(X_Axis,Y_Axis,width,height);
    variable_name2.shapeColor = "color";
    variable_name2.debug = true;
    
}
function draw(){
    background("color") or background(r(redColor),g(greenColor),b(blueColor))
    
    variable_name1.x = mouseX;
    variable_name1.y = mouseY;  
    isTouching();
    drawSprites();
}
    function isTouching(){
    if(variable_name1.x - variable_name2.x <( variable_name1.width + variable_name2.width)/2
     &&  variable_name2.x - variable_name1.x <( variable_name1.width + variable_name2.width)/2
      && variable_name1.y - variable_name2.y <( variable_name1.height + variable_name2.height)/2
      && variable_name2.y - variable_name1.y <( variable_name1.height + variable_name2.height)/2) {
           variable_name1.shapeColor = "color";
           variable_name2.shapeColor = "color";
    }
        else {
           variable_name1.shapeColor = "color";
           variable_name2.shapeColor = "color";    
                }
refer this link for more:- https://whjr-v2-prod-bucket.s3.ap-south-1.amazonaws.com/be22d03b-c7a2-4362-a4df-8c4fea3804df.pdf
````



#### day 21

I learnt to make is Touching and Bounce Off function  and to create and call our own library in visual studio. Also about boolean values 

````javascript
"true" and "false" as the two boolean values which are mostly used for yes and no in java script 
````

````javascript
// to make alogrithms 

var variable_name1;
var variable_name2;
function setup(){
    createCanavs(width,height);
    variable_name1 = createSprite(X_Axis,Y_Axis,width,height);
    variable_name1.shapeColor = "color";
    variable_name1.velocityX = value;
    variable_name1.debug = true;
    
    variable_name2 = createSprite(X_Axis,Y_Axis,width,height);
    variable_name2.shapeColor = "color";
    variable_name1.velocityX = -value;
    variable_name2.debug = true;
    
}
function draw(){
    background("color") or background(r(redColor),g(greenColor),b(blueColor))
    
    variable_name1.x = mouseX;
    variable_name1.y = mouseY;
    
    if(isTouching(variable_name1,variable_name3)){
        movingRect.shapeColor = "color";
        rect.shapeColor = "color";
    }
    else{
        movingRect.shapeColor = "color";
        rect.shapeColor = "color";
    }
    drawSprites();
}
    function isTouching(varible_name3, variable_name4){
    if(variable_name1.x - variable_name2.x <( variable_name1.width + variable_name2.width)/2
     &&  variable_name2.x - variable_name1.x <( variable_name1.width + variable_name2.width)/2
      && variable_name1.y - variable_name2.y <( variable_name1.height + variable_name2.height)/2
      && variable_name2.y - variable_name1.y <( variable_name1.height + variable_name2.height)/2) {
            return true;
    }
        else {
            return false;
                }
        
        function bounceOff(variable_name1, variable_name2){
        if(variable_name1.x - variable_name2.x <( variable_name1.width + variable_name2.width)/2
  		   &&  variable_name2.x - variable_name1.x <( variable_name1.width + variable_name2.width)/2){
            variable_name1.velocityX = variable_name1.velocityX * (-1);
            variable_name2.velocityX = variable_name2.velocityX * (-1);
        }            
        if(variable_name1.y - variable_name2.y <( variable_name1.height + variable_name2.height)/2
    	   && variable_name2.y - variable_name1.y <( variable_name1.height + variable_name2.height)/2){
            variable_name1.velocityY = variable_name1.velocityY * (-1);
            variable_name2.velocityY = variable_name2.velocityY * (-1);
        }
        }
````

````javascript
// to make our own library and call it and also add code to it 
make 1 more folder and name it 
in index.html file in 5th line write
<script src="./nameOfTheLibrary"></script>
refer this link for more:- https://whjr-v2-prod-bucket.s3.ap-south-1.amazonaws.com/cbf539f5-283f-4dad-902c-79cd65587b56.pdf
````

#### day 22

I learnt about physics engine and matter.js which is a library that helps us to use physics engine. 

// log in to console to print anything 

````javascript
const Engine = Matter.Engine;							// to lessen the words 
const world  = Matter.World;								//(note in const you can't change it's value)
const bodies = Matter.bodies;			

var engine, world; 
var object;

function setup(){
    createCanvas(width,height);							// to createCanvas
    
    engine = Engine.create();							// to createEngine
    world = engine.world();								// to create an world
    
    object = Bodies.rectangle(X_Axis,Y_Axis,width,height);   // to create an object 
    world.add(world,object);
}
function draw(){
    background("color");								// to add a background color
    Engine.update(engine);								// to update engine 
    rectMode(center);									// to display rectangle at centre
    rect(X_Axis,Y_Axis,width,height);					// create a rectangle
}
````

````javascript
// to have bounceOff and let it be static 
var variableName_Engine{
    isStatic: true;
}
var variableName_option = {
     restitution: value?
}
````

````javascript
var variable_name;

function setup(){
    variable_name = circle(X_Axis,Y_Axis,radius);
}
function draw(){
    ellipseMode(radius);
    ellipse(variable_name.position.x,variable_name.position.y);
}
refer this link for more:- https://whjr-v2-prod-bucket.s3.ap-south-1.amazonaws.com/6a07452f-91d5-4575-8477-280e6293b56e.pdf
````



#### day 23

I learnt to create blueprints , new box 

````javascript
1). Create a new file in the same folder called Box.js.      // remember to call all the files in index.html 
In it:-
 class class_name{
     constructor(x,y,width,height){
         options = {
		   'restitution': value;
              'friction': value;
               'density': value;
         }
         this.body = bodies.rectangle(x,y,width,height);
         world.add(world,this.body);
    }
    display(){
        var pos = this.body.position;
        var angle = this.body.angle;
        push();
        translate(pos.x,pos.y);
        rotate(angle);
        rectMode(CENTER);
        fill("color");
        rect = (pos.x,pos.y,this.width,this.height);
        pop();
    }
	}
2). In sketch.js file:-                                         // (note:- do all the code from above also)
 
    var variable_name
    var variable_name2
    
    function setup(){
    createCanvas(width,height);
    variable_name = new Box(x,y,width,height);
    variable_name2 = new Box(x,y,width,height);
    variable_name3 = new Ground(x,y,width,height);
   }
    
   function draw(){
    background("color");
    Engine.update(engine);
       
    variable_name.display();
    variable_name2.display();
   }
    
3). create a new file called ground
 in it:-
     class ground(){
         constructer(){
             var options = {
               isStatic: true;
             }
         this.body = bodies.rectangle(x,y,width,height,options);
         this.width = width;
         this.height = height;
         world.add(world,this.body);
         }
         display(){
             var pos = this.body.position;
             rectMode(CENTER);
             fill("color");
             rect(pos.x,pos.y,width,height);
         }
     }
refer this link for more:- https://whjr-v2-prod-bucket.s3.ap-south-1.amazonaws.com/1b57d2d8-6393-4f47-a09d-5184812cc024.pdf
````

