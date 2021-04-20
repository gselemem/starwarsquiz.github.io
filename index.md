<!Doctype html>
<html lang= "en">
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta charset="utf-8"/>
        <title> Gustavo Selemem | 3042264 </title>
        <link rel = "styleSheet" href ="Style.css"/>
    </head>

<div>

<body>

<section id="intro">

    <h3> A <strong> quiz </strong> from a galaxy far, far away. </h3>

    <p> Do you think you know the STAR WARS universe? </p>
    <p id="highlight"> <strong> Test your knowledge now! </strong> </p>
    <a href="#first-question"> <button> <b> Start Quiz </b> </button> </a>

</section>



<section id="first-question">

    <h1> 1. </h1>

       <img src="Images/Question1.png" width="300" height="300">

    <h2> What is the first line spoken on STAR WARS: a new hope? </h2>

<div id="options">

      <button id="btn1"> R2-D2 where are you? </button>

      <button id="btn2" onClick="onClick()"> Did you hear that? They shut down the main reactor. </button>

      <button id="btn3"> A long time ago, in a galaxy far, far away... </button>

      <div id="container"> </div>

      <a href="#second-question"> <button id="Next"> Next </button> </a>
</div>

<script>

      var btn1 = document.getElementById("btn1"),
          btn2 = document.getElementById("btn2"),
          btn3 = document.getElementById("btn3"),

          container = document.getElementById("container");

      var content1 = "Right it is not! Again, you should try.",
          content2 = "Correct you are! Strong is the force within you.",
          content3 = "Right it is not! Again, you should try.";

          btn1.addEventListener("click", () => container.innerHTML = content1);
          btn2.addEventListener("click", () => container.innerHTML = content2);
          btn3.addEventListener("click", () => container.innerHTML = content3);

      var score = 0;
          function onClick() { 
          score ++;
          document.getElementById("score").innerHTML = score;
          };

</script>


</section>



<section id="second-question">
    <h1> 2. </h1>

       <img src="Images/Question2.png" width="300" height="300">

    <h2> Which race is Ashoka Tano? </h2>

<div id="options">

      <button id="btn4" onClick="onClick()"> Togruta </button>

      <button id="btn5"> Wookie </button>
      
      <button id="btn6"> Gungan </button>

      <div id="container2"> </div>

      <a href="#third-question"> <button id="Next"> Next </button> </a>

</div>

<script>
        
      var btn4= document.getElementById("btn4"),
          btn5 = document.getElementById("btn5"),
          btn6 = document.getElementById("btn6"),

          container2 = document.getElementById("container2");

      var content4 = "Correct you are! Strong is the force within you.",
          content5 = "Right it is not! Again, you should try.",
          content6 = "Right it is not! Again, you should try.";

          btn4.addEventListener("click", () => container2.innerHTML = content4);
          btn5.addEventListener("click", () => container2.innerHTML = content5);
          btn6.addEventListener("click", () => container2.innerHTML = content5);

</script>


</section>


<section id="third-question">

     <h1> 3. </h1>

        <img src="Images/Question3.png" width="300" height="300">

     <h2> Which one of this characters is Princess Leia's foster father? </h2>

<div id="options">

        <button id="btn7"> <img src="Images/1.jpg" width="300" height="80" alt = "Windu" title = "Windu"> </button>

        <button id="btn8" onClick="onClick()"> <img src="Images/2.jpg" width="300" height="80" alt = "Organa" title = "Organa"> </button>

        <button id="btn9"> <img src="Images/3.jpg" width="300" height="80" alt = "Kenobi" title = "Kenobi"> </button>

        <div id="container3"> </div>

        <a href="#fourth-question"> <button id="Next"> Next </button> </a>

</div>

<script>
        
      var btn7 = document.getElementById("btn7"),
          btn8 = document.getElementById("btn8"),
          btn9 = document.getElementById("btn9"),

          container3 = document.getElementById("container3");

      var content7 = "Right it is not! Again, you should try.",
          content8 = "Correct you are! Strong is the force within you.",
          content9 = "Right it is not! Again, you should try.";

          btn7.addEventListener("click", () => container3.innerHTML = content7);
          btn8.addEventListener("click", () => container3.innerHTML = content8);
          btn9.addEventListener("click", () => container3.innerHTML = content9);

</script>

</section>


<section id="fourth-question">

    <h1> 4. </h1>

        <img src="Images/Question4.png" width="300" height="300">

    <h2> What is the Order 66? </h2>

<div id="options">

      <button id="btn10" onClick="onClick()"> An order that identifies all Jedi as traitors. </button>

      <button id="btn11">  An order that identifies all Rebels as traitors. </button>

      <button id="btn12">  An order that identifies all Sith as traitors. </button>

      <div id="container4"> </div>

      <a href="#fifth-question"> <button id="Next"> Next </button> </a>

</div>

<script>
        
      var btn10 = document.getElementById("btn10"),
          btn11 = document.getElementById("btn11"),
          btn12 = document.getElementById("btn12"),

          container4 = document.getElementById("container4");

      var content10 = "Correct you are! Strong is the force within you.",
          content11 = "Right it is not! Again, you should try.",
          content12 = "Right it is not! Again, you should try.";

          btn10.addEventListener("click", () => container4.innerHTML = content10);
          btn11.addEventListener("click", () => container4.innerHTML = content11);
          btn12.addEventListener("click", () => container4.innerHTML = content12);

</script>

</section>


<section id="fifth-question">

    <h1> 5. </h1>

        <img src="Images/Question5.png" width="300" height="300">

    <h2> Complete the sentence: “Only a

        <select id="select1">

        <option value="-">-</option>

        <option value="jedi">Jedi</option>

        <option value="sith" onClick="onClick()">Sith</option>

        <option value="rebel">Rebel</option>

        </select>

        deals in absolute." </h2>

        <button id="Check" onclick="getOption()">
        Check Answer
        </button>

        <p id="demo1"><span class="output"> </span></p>

        <a href="#sixth-question"> <button id="Next"> Next </button> </a>


<script type="text/javascript">

        function getOption() {

        selectElement = document.querySelector('#select1');

        output = selectElement.value;

        document.querySelector('.output').textContent = output;


        switch(selectElement.value) {

        case "jedi":
           document.getElementById("demo1").innerHTML = "Right it is not! Again, you should try.";
        break;

        case "sith":
           document.getElementById("demo1").innerHTML = "Correct you are! Strong is the force within you.";
           score ++;
        break;

        case "rebel":
           document.getElementById("demo1").innerHTML =  "Right it is not! Again, you should try.";
        break;

        default:
           document.getElementById("demo1").innerHTML = "Select Something";
        }

        }

</script>


</section>


<section id="sixth-question">

    <h1> 6. </h1>

        <img src="Images/Question6.png" width="300" height="300">

    <h2 id="Question6"> What is Baby Yoda's real name? </h2>

        <form id="frm1">
        <input id = "q6" type="text" name="answer" value=""> <br>
        </form> 

    <button onclick="myFunction()"> Check Answer </button>

    <p id="container6"></p>

    <a href="#ending"> <button id="Next"> Next </button> </a>

<script>
        
        function myFunction() {
        var q6ans = document.getElementById("q6").value;

        if (q6ans == "Grogu") {

        score ++;
        document.getElementById("container6").innerHTML = "Correct you are! Strong is the force within you.";
        } 

        else {
        document.getElementById("container6").innerHTML = "Right it is not! Again, you should try.";
        }
        console.log(q6ans)

        document.getElementById("score").innerHTML = score;
        }

</script>

</section>

<section id="ending">

        <h1> <strong> You've got <a id="score">0</a> questions right! </strong> </h1>

        <p> <strong> Gustavo Selemem | 3042264 | gustavo.selemem@griffith.ie </strong> </p>

</section>

</body>

</div>
