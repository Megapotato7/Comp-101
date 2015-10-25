int[] sliderX = new int [100];
int[] sliderY = new int [100];
//Group the V project
//Members Nathan Ross, Adam , Andrew, Hamdan (I can't remember your name and I probably butchered it I'm sorry), and Sean



/* We need to work on the sliders first so we can at least look at shit
 hud should come next and then display as it will take us the longest
 
 The slider stuff is kinda difficult and the display stuff is going to be crazy hard until I have it all set up.
 The hud isnt too bad you just write and display images
 We need to maybe change up some of the methods for the game text but we can talk about that Sunday
 if you want to write some of the text box and diologe stuff throw it into gametext for now as comments and we can sort it out later
 
 if you want to work on your mini games just make a new tab and write all your functions there
 we can add it to display and it will work. Dont fuck with the setup and draw too much
 
 I might misname some stuff while I'm working on it so you can go through and rename them if you want
 
 Have fun!
 */

//All of the slider arrays
int[] sliderValue = new int [100];
int[] sliderContext = new int [100];
float[] buttonX = new float [100]; 
float[] buttonY = new float [100];
int currentSlider = 0;

int gameState = 0;

int weekHours = 24;

PFont font;

void setup() {
  size(500, 500);
  //These are just for testing
  makeSlider(1);
  makeSlider(1);
  makeSlider(1);
  makeSlider(1);
  makeSlider(1);

  //This lets us writes stuff
  font = createFont("Arial", 16, true);
}

void draw() {
  background(255);
  drawSlider();
  hud();
  display();
}
