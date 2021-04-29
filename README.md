# NHSCompSci
NHS Computer Science Q4 Project

var startRand = 4;
var playerState = false;
var yellowLit = rgb(255,255,0);
var redLit = rgb(255,0,0);
var blueLit = rgb(0,0,255);
var greenLit = rgb(124,252,0);

onEvent("playbutton", "click", function(event) {
  setScreen("gamescreen");
  function lightUp(id, rgbCode) {
    console.log(id + " lit");
    var x = 0;
    setProperty(id, "background-color", rgbCode);
    timedLoop(30, function() {
    setProperty(id, "background-color", rgbCode);
    x++;
    if(x == 13) {
      setProperty(id, "background-color", rgbCode);
      resetAll();
    }
    }); 
  }
});  



onEvent("playbutton", "click", function( ) {
  setScreen("Gamescreen");
  
  function arrayfinder() {
    function Randomarray() {
      var pattern;
      for (var x = 0; x < randSize; x++) {
        Pattern(randomNumber(1, 4));
      }
      console.log("Pattern Made: " + pattern);
      return pattern;
    }
    var patternarray = Randomarray(startrand - 1);
    return patternarray;
  }
});

