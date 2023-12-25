 <!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="./date.css">
        
    </head> 
    <body>
        <div class="container">
            <div >
               
                <h1 class = "header_text">How Much Do You Love Me?</h1>
            </div>
            <div class="gif_container">
                <img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcDdtZ2JiZDR0a3lvMWF4OG8yc3p6Ymdvd3g2d245amdveDhyYmx6eCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/cLS1cfxvGOPVpf9g3y/giphy.gif" alt="Cute animated illustration">
            </div>
            <div class = "buttons">
                <button class="btn" id = "yesButton" onclick="nextPage()">So Much</button>
              
            
                <script>
                    function nextPage() {
                        window.location.href = "yes.html";
                    }
                    
                    function moveButton() {
                        var x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth) - 85;
                        var y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight) - 48;
                        document.getElementById('noButton').style.left = `${x}px`;
                        document.getElementById('noButton').style.top = `${y}px`;
                    }
                </script> 


                  <div class="container">
                    <div class="buttons">
                        
                        <button class="btn" id="noButton" draggable="true" onmousedown="moveButton(event)" ondblclick="openPage()">Sooo Sooo Much</button>
                    </div>
                    
                </div>
                <script>
                    var moveCount = 0;
            
                    function moveButton(event) {
                        if (moveCount < 69) {
                            // Move the button if the count is less than 69
                            var x = Math.random() * (window.innerWidth - event.target.offsetWidth);
                            var y = Math.random() * (window.innerHeight - event.target.offsetHeight);
                            event.target.style.left = `${x}px`;
                            event.target.style.top = `${y}px`;
                            moveCount++;
            
                            // Update the count bar
                            document.getElementById('moveCount').textContent = moveCount;
                        }
                    }
            
                    function openPage() {
                        // Double-click opens the next page
                        window.location.href = "no.html";
                    }
                </script>
            </div>
        </div>
       
    </body> 
</html>



body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 90vh;
    background-color: #F8C8DC;
}

#noButton {
    position: absolute;
    margin-left: 150px;
    transition: 0.5s;
}

#yesButton {
    position: absolute;
    margin-right: 150px;
}

.header_text {
    font-family: 'Nunito';
    font-size: 40px;
    font-weight: bold;
    color: white;
    text-align: center;
    margin-top: 20px;
    margin-bottom: 0px;
}

.buttons {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
    margin-left: 20px;
}

.btn {
    background-color: #FFB6C1;
    color: white;
    padding: 15px 32px;
    text-align: center;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
    border: none;
    border-radius: 12px;
    transition: background-color 0.3s ease;
}

.gif_container {
    display: flex;
    justify-content: center;
    align-items: center;
}

@media only screen and (max-width: 320px) and (max-height: 568px) {
    body {
        height: 100vh;
    }

    .header_text {
        font-size: 20px;
    }

    img {
        height: 60vh;
    }

    .btn {
        padding: 10px 18px;
        font-size: 12px;
    }
}

@media only screen and (max-width: 414px) and (max-height: 736px) {
    body {
        height: 90vh;
    }

    .header_text {
        font-size: 28px;
    }

    img {
        height: 60vh;
    }

    .btn {
        padding: 15px 25px;
        font-size: 14px;
    }
}


       <!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="./no.css">
        
    </head> 
    <body>
        <div class="container">
            <div class="gif_container">
                <img src="./ezgif.com-crop.gif" alt="Kissi Kisssi">
                <div class="hover_text">Me Khup Khup Sara Pyarr Karto Mi Janu tula❣️</div>
            </div>
    </body> 
</html>




body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f18e5b;
    margin: 0;
}

.header_text {
    font-family: 'Nunito';
    font-size: 27px;
    font-weight: bold;
    color: black;
    text-align: center;
    margin-top: 20px;
    margin-bottom: 0px;
}

.container {
    position: relative
}

.gif_container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 300px; /* Adjust the height based on your design */
    position: relative;
}


.hover_text {
    position: absolute;
    top: 180%;
    left: 50%;
    transform: translate(-50%, -50%);
    color:cyan;
    font-size: 20px;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.container:hover .hover_text {
    opacity: 1;
}




<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="./yes.css">
        
    </head> 
    <body>
        <div class="container">
            <div >
                <h1 class = "header_text">Yeeeyyyy!!</h1>
            </div>
            <div class="gif_container">
                <img src="https://media0.giphy.com/media/T86i6yDyOYz7J6dPhf/giphy.gif" alt="Cute animated illustration">
            </div>
        </div>
       
    </body> 
</html>





body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #F8C8DC;
}

.header_text {
    font-family: 'Nunito';
    font-size: 50px;
    font-weight: bold;
    color: white;
    text-align: center;
    margin-top: 20px;
    margin-bottom: 0px;
}

.gif_container {
    display: flex;
    justify-content: center;
    align-items: center;
}
