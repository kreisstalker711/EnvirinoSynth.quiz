<!DOCTYPE html>
<html lang="en">				
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Aladin&display=swap" rel="stylesheet">
    <meta charset="UTF-8">
    <meta content="author" description="Created by Kathiravan">
    <title>EnvironoSynth.welcome</title>
    <style>
        body { 
    	     background: linear-gradient(90deg, #008552 0%, #92FE9D 100%);
      	     font-family: Verdana, sans-serif;
             font-weight: bold;
             font-size: 50px;
             
         }

        h2 {
            color: #3857a5 ;
            font-size: px;
            font-family: "Aladin", system-ui;
            font-weight: 400;
            font-style: normal;
        }


        input#quiz {
            text-align: center;
            border: 3px solid #2e7d32;
            padding: 15px 10px;
            font-size: 17px;
            border-radius: 12px;
            width: 400px
       }

          
        button {
            background-color: (#f9fff6);
            color: rgb(6, 14, 87);
            padding: 6px;
            font-size: 17px;
            border-radius: 8px;
            border: 3px solid green;
        }
        
        button:hover {
            background-color: green;
   
        }
        
    </style>
</head>
<body style="text-align: center;">
    
    

<h2>🌍 EnvironoSynth- AI quiz App</h2>




    <input type="text" id="quiz" placeholder="Enter a topic">
    <button style="text-align: start;" onclick="getQuiz()">Move to Login page</button>

    <p id="quiz-output"></p>

    <script>
        function getQuiz() {
            const answer = document.getElementById("quiz").value.trim().toLowerCase();

            if (answer === "") {
                // Redirect to quiz page
                window.location.href = "acc.html";
            } else if (answer === "no") {
                document.getElementById("quiz-output").innerText = "Maybe next time!";
            } else {
                document.getElementById("quiz-output").innerText = "❌ Please type 'yes' or 'no'.";
            }
            
        }
    </script>
</body>
</html>
