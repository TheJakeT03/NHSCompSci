# NHSCompSci
NHS Computer Science Q4 Project

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

