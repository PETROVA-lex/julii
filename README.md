
    
    h1 {
        color: rgb(19, 80, 75);
        text-shadow: 2px 2px 4px #360808;
    }

    button {
        background-color: rgb(60, 109, 93);
        margin: 5px;
        padding: 5px 5px;
        font-size: 1.2em;
        border-radius: 5px;
    }
    .card {
        background-color: #300505;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(82, 4, 4, 0.548);
        padding: 20px;
        margin: 20px;
        text-align: center;
    }
    img
    {
        width: 150px;
        height: auto;
        border-radius: 15px;
        margin: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }
    button:hover {
        background-color: rgb(34, 70, 60);
        color: rgb(66, 16, 16);
        cursor: pointer;
     }
    button:active {
        transform: scale(0.98);
    }
    button {
        width: auto;
        height: auto;
    }

</style>
</head>

  <body>
    <h1>¿Queres salir a algún lado conmigo?</h1>
    <div class="card">
        <img src="https://media.giphy.com/media/v1.Y2lkPWVjZjA1ZTQ3OTJ6Zm91MjUyZG0yZGVjdHdqOHo0M3oycmpjc2RoZmJnY2h4YnU4cSZlcD12MV9naWZzX3JlbGF0ZWQmY3Q9Zw/xAFIrLYSDMUa4/giphy.gif" alt="Salida">      
    </div>
    <div> 
    <button onclick="cambiarDePagina('jullii.html')">Si</button>
    <button onclick="cambiarDePagina('https://www.youtube.com/watch?v=btaPu76Z3mo')">No</button>
   </div>
    <script>
        function cambiarDePagina(pagina) {
            window.location.href = pagina;
        }
    </script>
    <div>
        <button onclick="alert('Que te enamores de mí, es mi sueño, es mi anhelo, es lo que más yo quiero, es por lo que lucho cada día de mi vida, es mi deseo secreto.')" alt ="Mensaje secreto">Poema</button>
        <button onclick="cambiarDePagina('https://www.youtube.com/watch?v=HiCIz-xU1P4&list=RDHiCIz-xU1P4&start_radio=1')">Canción</button>
    </div>
    
</body> 
</html>
