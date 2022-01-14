<!-- PROYECTO TRIVIA - LABORATORIA-->

# triviaproject.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=2.0">
  <title>Inicio</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
  <script src="https://unpkg.com/sweetalert/dist/sweetalert.min.js"></script>
</head>
<body>

  <section class="firtsScreen" id="firtsScreen">
    <img src="https://static.emol.cl/emol50/Fotos/2020/05/14/file_20200514150603.jpg" alt="" width="100%" height="300">
    <br>
    <h1 style="color: white;
    background-color: blue;
    font-family: cursive;
    border-radius: 10px;"> ¿CUANTO SABES DE CINE? </h1>
      <p> ¡Pon a prueba tu cinefilia! </p> 

    <h3><p> Escribe tu nombre: </p></h3>
    <form >
      
  <!--linea de codigo para que este en Mayuscula lo que se ingrerse en el cuadro de texto-->
      
      <input type="text" class="normal" 
       name="Name" id="nameUser" size="20" maxlength="20" 
       style="text-transform:uppercase" /> 

      <!--<input type="text" id="nameUser" placeholder="Escribe tu nombre">-->
      
       <br> <br>
      <!--linea de codigo para limpiar cuadro de texto-->
      <input type="reset" class="btnclean" value="Limpiar formulario">
        <a href="" class="btnStart" id="btnStart">Comenzar el juego</a>
        <br>      
    </form>
  </section>

<section class="optionScreen" id="optionScreen">
    <p class="textCategory">ESCOGE UNA CATEGORIA</p>
    <div>
      <a href="" id="btnCatTerror">TERROR</a>
      <a href=""id="btnCatAction">ACCIÓN</a>
    </div>

</section>

<section id="welcomeScreen">
  <p>BIENVENIDO</p>
    <p id="result" class="result"></p>
    <br>
    <a href="" class="btnReturn" id="btnReturn">Volver</a>
    <br><br>
</section>

<section class="secondScreen"  id="flotante" >
  <div class="boxSecondScreen">
    <form name="option">
      <h2>¿Cuantas veces Arnold Schwarzenegger ha interpretado al Terminator T800?</h2>
          <div class="cuadro box2">
          <input type="radio" name="answer" value="7" onclick="answerVoid()" id="valIncorrect">7
            </div>  
          <div class="cuadro box">
          <input type="radio" name="answer" value="6" onclick="answerVoid()" id="valCorrect" >6
            </div>  
          <div class="cuadro box3">
          <input type="radio" name="answer" value="3" onclick="answerVoid()" id="valIncorrect">3
        </div> 
    </form>
  </div> 
  <div class="boxSecondScreen1">
    <form name="option1">
        <h2>¿Que película de Pedro Almodóvar ha ganado un Oscar?</h2>
          <div class="cuadro box4">
            <input type="radio" name="answer1" value="Volver" onclick="answerVoid1()" id="valIncorrect">Volver
          </div>   
            <div class="cuadro box5">
            <input type="radio" name="answer1" value="Dolor y Gloria" onclick="answerVoid1()" id="valCorrect">Dolor y gloria
          </div> 
              <div class="cuadro box1"> 
          <input type="radio" name="answer1" value="Todo sobre mi madre" onclick="answerVoid1()" id="validation">Todo sobre mi madre
          </div>   
      </form>
    </div> 
    <div class="boxSecondScreen2">
      <form name="option2">
        <h2>¿Como se llama el creador de las trampas en la franquicia de Jigsaw?</h2>
          <div class="cuadro box6">
            <input type="radio" name="answer2" value="Logan Nelson" onclick="answerVoid2()" id="answer2">
            <label for="answer2">Logan Nelson</label>
            
          </div>   
            <div class="cuadro box7">
            <input type="radio" name="answer2" value="Lawrence Gordon" onclick="answerVoid2()">
            <label for="answer2">Lawrence Gordon</label>           
          </div> 
              <div class="cuadro box8"> 
          <input type="radio" name="answer2" value="John Krame" onclick="answerVoid2()">
          <label for="answer2">John Krame</label>
          </div>
      </form>
    </div>  
    <br>
    <button id="bntAnswer" value="green">Enviar Respuesta</button>

    <div id="tableScore">

        <table border="1">
		<caption>Calificacion</caption>
		<tr>
			<th>Respuestas Correctas</th>
			<th>Respuestas Incorrectas</th>
      <th>Total</th>
		</tr>
		<tr>
			<td id="amountOfScoreCor"></td>
			<td id="amountOfScoreInc"></td>
      <td id="amountOfScoreFinal"></td>
		</tr>
		</table>

    </div>
</section>
	
<!--Segunda OPCION => TERROR -->
	
<section class="threeScreen"  id="threeScreen" > 
  <div class="boxSecondScreen3">
    <form name="alternative">
      <h2>¿En qué película se pronunció la famosa frase: “¿Te gustan la películas de terror?”</h2>
          <div class="cuadroAlt boxAlt1">
            <input type="radio" value="Sé lo que hicieron el verano pasado" name="answerAlt" onclick="answerVoid3()"><label for="">Sé lo que hicieron el verano pasado</label>
          </div>
          <div class="cuadroAlt boxAlt2">
            <input type="radio" value="Scream: La máscara de la muerte" name="answerAlt"  onclick="answerVoid3()"><label for="">Scream: La máscara de la muerte</label>
          </div>
           <div class="cuadroAlt boxAlt3">
            <input type="radio" name="answerAlt" value="Viernes 13" onclick="answerVoid3()"><label for="">Viernes 13</label>
          </div> 
    </form>
  </div>
  <div class="boxSecondScreen4">
    <form name="alternative1">
      <h2>¿Cómo se llama la chica tenebrosa de The Ring en la versión japonesa?</h2>
      <div class="cuadroAlt boxAlt4">
       <input type="radio" name="answerAlt1" value="Keiko" onclick="answerVoid4()"><label for="">Keiko</label>
      </div>
      <div class="cuadroAlt boxAlt5">
       <input type="radio" name="answerAlt1" value="Sadako" onclick="answerVoid4()"><label for="">Sadako</label>
      </div>
      <div class="cuadroAlt boxAlt6">
       <input type="radio" name="answerAlt1" value="Sakura" onclick="answerVoid4()"><label for="">Sakura</label>
      </div>  
    </form>
  </div> 
  <div class="boxSecondScreen5">  
    <form name="alternative2">
      <h2>¿Cuántas películas de Halloween existen?</h2>
      <div class="cuadroAlt boxAlt7">
        <input type="radio" name="answerAlt2" value="10" onclick="answerVoid5()"><label for="">10</label>
      </div>
      <div class="cuadroAlt boxAlt8">
         <input type="radio" name="answerAlt2" value="13" onclick="answerVoid5()"><label for="">13</label>
      </div>
      <div class="cuadroAlt boxAlt9">
       <input type="radio" name="answerAlt2" value="5" onclick="answerVoid5()"><label for="">5</label>
      </div>
    </form>
  </div>  
    <br>
    <button id="bntAnswer2" value="green">Enviar Respuesta</button>

    <div id="tableScore1">
      <table border="1">
        <caption>Calificacion</caption>
        <tr>
          <th>Respuestas Correctas</th>
          <th>Respuestas Incorrectas</th>
          <th>Total</th>
        </tr>
        <tr>
          <td id="scoreCorrect"></td>
          <td id="scoreIncorrect"></td>
          <td id="scoreTotal"></td>
        </tr>
	  	</table>
    </div>
</section>


  <script src="script.js"></script>
</body>
</html>
