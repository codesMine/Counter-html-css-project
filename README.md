
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    
}
body{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    

}
.container{
    width: 250px;
    height: 250px;
    background: #185AD8;
    color: WHITE;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    position: relative;
    border-radius: 20px 55px ;
}
.counter{
    font-size: 4rem;
    font-family: 'Ubuntu',sans-serif;

}
.heading{
    font-family:segoe print,cursive;
font-size: 2rem;
}
button{
    width: 60px;
    height: 60px;
    position: absolute;
    cursor: pointer;
    font-size: 1.2rem;
    background: #FDDB3A;
    color: rgb(34,34,34);
    box-shadow: 2 2 10px rgb(51, 51, 51, 0.158);
    border: none;
    border-radius: 50px;
    box-shadow: 0 9px #52575d;
}


button:hover {background-color: #29de92}

button:active {
  background-color: #1d566e;
  box-shadow: 0 5px #363940;
  transform: translateY(4px);
}
























.decr{
    bottom: 10%;
    left: -15%;
}
.incr{
    bottom: 10%;
    right: -15%;
}
    </style>
</head>
<body>
    <div class="container">
        <p class="heading">Counter</p>
        <p class="counter" id="counter">0</p>
        <button class="incr"><i class="fas fa-plus">+</i></button>
        <button class="decr"> <i class="fas fa-minus"><b>-</b></i></button>
        
    </div>
    <script>
        const counter = document.getElementById( 'counter');
        const incr = document.querySelector( '.incr');
        const decr = document.querySelector( '.decr');

        let count = 0;
        incr.addEventListener("click", ()=>{
            count++;
            counter.innerHTML = count;

        });



        decr.addEventListener("click", ()=>{
            count--;
            counter.innerHTML = count;

        });
        
        
        


    </script>
</body>
</html>
