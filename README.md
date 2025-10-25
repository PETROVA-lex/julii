# julii
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lugares</title>
    <link rel="stylesheet" href="styles.css">
 <style>
    body {
        background-image: url(https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExaDZ2YnB6cGx3b3FkcjNtcXJmNTVvaXRqZTd6YWo1OGhlNXcyZjgxYyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/26wkGyLXBYFuwnE6A/giphy.gif);
        background-size: cover;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 100px;
    }
    img {
        width:100px;
        padding:10px;
        border-radius: 15px;
    }
    button {
        background-color: #ce84ad;
        color: #020001;
        border: 4px solid #81597c;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 1.5em;
        padding: 10px 20px;
        margin: 10px;

    }
    button:hover {
        background-color: #4d1305;
        color: #04021b;
        cursor: pointer;
        transform: scale(1.05);
    }
    button:focus {
        outline: none;
        box-shadow: 0 0 5px #751508;
    }
    button:active {
        background-color: #961212;
        color:#065a4fe7
    }
    .card {
        background-color: #125847dc;
        border-radius: 2x;
        box-shadow: 5px 10px 16px rgba(78, 5, 60, 0.815);
        margin: 1px auto;
        padding: 50px;
        display: inline-block;
    }
    h1 {
        color: #0e021a;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 10px;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        font-size: 2.5em;
    }
    h2 {
        color: #09010e;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 10px;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        font-size: 2em;

    }

    .submenu {
        display: none;
        margin-top: 15px;
        padding: 15px;
        background-color: #8d4b9e;
        border-radius: 20px
    }
    .submenu a {
        display: block;
       text-decoration: none;
       margin: 5px;
       width: 20px;
       padding: 25;

    }
    .submenu a:hover {
         text-decoration: underline;
    }
    footer {
        margin-top: 20px;
    }
    #explotaBtn {
        background-color: #81597c;
        border: #020001;
        padding: 5px;

    }
    @keyframes explotar {
        0% { transform: scale(1); opacity:  1; }
        50% { transform: scale(4); opacity: 1; }
        100% { transform: scale(1); opacity:  0;}
    }
   </style>
</head>


 <body>
    <h1>¿Dónde quieres ir?</h1>

    <div class="card">
        <h2 id="Lugares">Lugares</h2>

    <button onclick="toggleMenu('plazas')">Plazas</button>
     <div id="plazas" class="submenu">
    <button onclick="sendWhatsapp('quiero ir a la plaza pedernera')">Pedernera</button>
    <button onclick="sendWhatsapp('quiero ir a la plaza finur')">Finur</button>
    <button onclick="sendWhatsapp('quiero ir a la plaza cultural')">Cultural</button>
 </div>

   
    <button onclick="toggleMenu('pool')">Pool</button>
    <div id="pool" class="submenu">
    <button onclick="sendWhatsapp('quiero ir a la pool')">Pool</button>
 </div>
 
    <button onclick="toggleMenu('centro')">Centro</button>
    <div id="centro" class="submenu">
    <button onclick="sendWhatsapp('quiero ir al centro')">Centro</button>
    </div>

 <footer>
    <button onclick="cambiarDePagina('juliii.html')">Volver</button>
</footer>

<button id="explotaBtn">Tocame</button>
</div>

   <script>

    function sendWhatsapp(message)  {
        var phoneNumber = "5492657675467";
        var url = "https://wa.me/" + phoneNumber + "?text=" + encodeURIComponent(message);
        window.open(url, "_blank"); 
    }

    function cambiarDePagina(pagina) {
    window.location.href = pagina;

    }

    function toggleMenu(menuId) {
    var menu = document.getElementById(menuId);
    if (menu.style.display === "block") {
        menu.style.display = "none";
    } else {
        menu.style.display = "block";
    }
}
    const boton = document.getElementById("explotaBtn");
    boton.addEventListener("click",() => {
        let tamaño = 1;
        const crecer = setInterval(() => {
            tamaño +=0.2;
            boton.style.transform = `scale(${tamaño})`;

        if (tamaño >= 5) {
            clearInterval(crecer);
            boton.style.animation = "explotar 0.6s forwards";
            setTimeout(() => {
              boton.style.display = "none";
              document.body.innerHTML +="<h1>decime q no y te corto una teta</h1>";
              
            },600);
     }
    },100);
});

    </script>
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lugares</title>
    <link rel="stylesheet" href="styles.css">
 <style>
    body {
        background-image: url(https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExaDZ2YnB6cGx3b3FkcjNtcXJmNTVvaXRqZTd6YWo1OGhlNXcyZjgxYyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/26wkGyLXBYFuwnE6A/giphy.gif);
        background-size: cover;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 100px;
    }
    img {
        width:100px;
        padding:10px;
        border-radius: 15px;
    }
    button {
        background-color: #ce84ad;
        color: #020001;
        border: 4px solid #81597c;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 1.5em;
        padding: 10px 20px;
        margin: 10px;

    }
    button:hover {
        background-color: #4d1305;
        color: #04021b;
        cursor: pointer;
        transform: scale(1.05);
    }
    button:focus {
        outline: none;
        box-shadow: 0 0 5px #751508;
    }
    button:active {
        background-color: #961212;
        color:#065a4fe7
    }
    .card {
        background-color: #125847dc;
        border-radius: 2x;
        box-shadow: 5px 10px 16px rgba(78, 5, 60, 0.815);
        margin: 1px auto;
        padding: 50px;
        display: inline-block;
    }
    h1 {
        color: #0e021a;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 10px;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        font-size: 2.5em;
    }
    h2 {
        color: #09010e;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 10px;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        font-size: 2em;

    }

    .submenu {
        display: none;
        margin-top: 15px;
        padding: 15px;
        background-color: #8d4b9e;
        border-radius: 20px
    }
    .submenu a {
        display: block;
       text-decoration: none;
       margin: 5px;
       width: 20px;
       padding: 25;

    }
    .submenu a:hover {
         text-decoration: underline;
    }
    footer {
        margin-top: 20px;
    }
    #explotaBtn {
        background-color: #81597c;
        border: #020001;
        padding: 5px;

    }
    @keyframes explotar {
        0% { transform: scale(1); opacity:  1; }
        50% { transform: scale(4); opacity: 1; }
        100% { transform: scale(1); opacity:  0;}
    }
   </style>
</head>


 <body>
    <h1>¿Dónde quieres ir?</h1>

    <div class="card">
        <h2 id="Lugares">Lugares</h2>

    <button onclick="toggleMenu('plazas')">Plazas</button>
     <div id="plazas" class="submenu">
    <button onclick="sendWhatsapp('quiero ir a la plaza pedernera')">Pedernera</button>
    <button onclick="sendWhatsapp('quiero ir a la plaza finur')">Finur</button>
    <button onclick="sendWhatsapp('quiero ir a la plaza cultural')">Cultural</button>
 </div>

   
    <button onclick="toggleMenu('pool')">Pool</button>
    <div id="pool" class="submenu">
    <button onclick="sendWhatsapp('quiero ir a la pool')">Pool</button>
 </div>
 
    <button onclick="toggleMenu('centro')">Centro</button>
    <div id="centro" class="submenu">
    <button onclick="sendWhatsapp('quiero ir al centro')">Centro</button>
    </div>

 <footer>
    <button onclick="cambiarDePagina('juliii.html')">Volver</button>
</footer>

<button id="explotaBtn">Tocame</button>
</div>

   <script>

    function sendWhatsapp(message)  {
        var phoneNumber = "5492657675467";
        var url = "https://wa.me/" + phoneNumber + "?text=" + encodeURIComponent(message);
        window.open(url, "_blank"); 
    }

    function cambiarDePagina(pagina) {
    window.location.href = pagina;

    }

    function toggleMenu(menuId) {
    var menu = document.getElementById(menuId);
    if (menu.style.display === "block") {
        menu.style.display = "none";
    } else {
        menu.style.display = "block";
    }
}
    const boton = document.getElementById("explotaBtn");
    boton.addEventListener("click",() => {
        let tamaño = 1;
        const crecer = setInterval(() => {
            tamaño +=0.2;
            boton.style.transform = `scale(${tamaño})`;

        if (tamaño >= 5) {
            clearInterval(crecer);
            boton.style.animation = "explotar 0.6s forwards";
            setTimeout(() => {
              boton.style.display = "none";
              document.body.innerHTML +="<h1>decime q no y te corto una teta</h1>";
              
            },600);
     }
    },100);
});

    </script>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lugares</title>
    <link rel="stylesheet" href="styles.css">
 <style>
    body {
        background-image: url(https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExaDZ2YnB6cGx3b3FkcjNtcXJmNTVvaXRqZTd6YWo1OGhlNXcyZjgxYyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/26wkGyLXBYFuwnE6A/giphy.gif);
        background-size: cover;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 100px;
    }
    img {
        width:100px;
        padding:10px;
        border-radius: 15px;
    }
    button {
        background-color: #ce84ad;
        color: #020001;
        border: 4px solid #81597c;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 1.5em;
        padding: 10px 20px;
        margin: 10px;

    }
    button:hover {
        background-color: #4d1305;
        color: #04021b;
        cursor: pointer;
        transform: scale(1.05);
    }
    button:focus {
        outline: none;
        box-shadow: 0 0 5px #751508;
    }
    button:active {
        background-color: #961212;
        color:#065a4fe7
    }
    .card {
        background-color: #125847dc;
        border-radius: 2x;
        box-shadow: 5px 10px 16px rgba(78, 5, 60, 0.815);
        margin: 1px auto;
        padding: 50px;
        display: inline-block;
    }
    h1 {
        color: #0e021a;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 10px;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        font-size: 2.5em;
    }
    h2 {
        color: #09010e;
        font-family: Georgia, 'Times New Roman', Times, serif;
        text-align: center;
        padding: 10px;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        font-size: 2em;

    }

    .submenu {
        display: none;
        margin-top: 15px;
        padding: 15px;
        background-color: #8d4b9e;
        border-radius: 20px
    }
    .submenu a {
        display: block;
       text-decoration: none;
       margin: 5px;
       width: 20px;
       padding: 25;

    }
    .submenu a:hover {
         text-decoration: underline;
    }
    footer {
        margin-top: 20px;
    }
    #explotaBtn {
        background-color: #81597c;
        border: #020001;
        padding: 5px;

    }
    @keyframes explotar {
        0% { transform: scale(1); opacity:  1; }
        50% { transform: scale(4); opacity: 1; }
        100% { transform: scale(1); opacity:  0;}
    }
   </style>
</head>


 <body>
    <h1>¿Dónde quieres ir?</h1>

    <div class="card">
        <h2 id="Lugares">Lugares</h2>

    <button onclick="toggleMenu('plazas')">Plazas</button>
     <div id="plazas" class="submenu">
    <button onclick="sendWhatsapp('quiero ir a la plaza pedernera')">Pedernera</button>
    <button onclick="sendWhatsapp('quiero ir a la plaza finur')">Finur</button>
    <button onclick="sendWhatsapp('quiero ir a la plaza cultural')">Cultural</button>
 </div>

   
    <button onclick="toggleMenu('pool')">Pool</button>
    <div id="pool" class="submenu">
    <button onclick="sendWhatsapp('quiero ir a la pool')">Pool</button>
 </div>
 
    <button onclick="toggleMenu('centro')">Centro</button>
    <div id="centro" class="submenu">
    <button onclick="sendWhatsapp('quiero ir al centro')">Centro</button>
    </div>

 <footer>
    <button onclick="cambiarDePagina('juliii.html')">Volver</button>
</footer>

<button id="explotaBtn">Tocame</button>
</div>

   <script>

    function sendWhatsapp(message)  {
        var phoneNumber = "5492657675467";
        var url = "https://wa.me/" + phoneNumber + "?text=" + encodeURIComponent(message);
        window.open(url, "_blank"); 
    }

    function cambiarDePagina(pagina) {
    window.location.href = pagina;

    }

    function toggleMenu(menuId) {
    var menu = document.getElementById(menuId);
    if (menu.style.display === "block") {
        menu.style.display = "none";
    } else {
        menu.style.display = "block";
    }
}
    const boton = document.getElementById("explotaBtn");
    boton.addEventListener("click",() => {
        let tamaño = 1;
        const crecer = setInterval(() => {
            tamaño +=0.2;
            boton.style.transform = `scale(${tamaño})`;

        if (tamaño >= 5) {
            clearInterval(crecer);
            boton.style.animation = "explotar 0.6s forwards";
            setTimeout(() => {
              boton.style.display = "none";
              document.body.innerHTML +="<h1>decime q no y te corto una teta</h1>";
              
            },600);
     }
    },100);
});

    </script>

</body>
</html>
