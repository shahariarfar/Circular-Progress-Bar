# Circular-Progress-Bar
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Circular Progress Bar</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="skill">
        <div class="outer">
            <div class="inner">
                <div id="number">
                    
                </div>
            </div>
        </div>

        <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="160px" height="160px">
            <defs>
               <linearGradient id="GradientColor">
                  <stop offset="0%" stop-color="#e91e63" />
                  <stop offset="100%" stop-color="#673ab7" />
               </linearGradient>
            </defs>
            <circle cx="80" cy="80" r="70" stroke-linecap="round" />
        </svg>

    </div>


    <script>
        let number = document.getElementById("number");
        let counter = 0;
        setInterval(() => {
            if(counter == 65){
                clearInterval();
            }
            else{
                counter += 1;
                number.innerHTML = counter + "%";
            }
        }, 30);
    </script>

</body>
</html>
