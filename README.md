# dise-o-Responsive-con-css
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diseño Responsive con CSS</title>
    <link rel="stylesheet" href="../css/ejercicioresponsive.css">
</head>
<body>
    <div class="lateral">
        <div class="elemento"></div>
        <div class="elemento"></div>
        <div class="elemento"></div>
</div>
<main class="principal">
    
</main>
</body>
</html>



*{
    margin: 0;
    padding: 0;
}

body {
    display: flex;
}

.lateral {
    width: 30%;
    background-color: #2C3639;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 20px;
}

.principal {
    flex-grow: 2;
    background-color: #A27B5C;
    min-height: 100vh;
}

.elemento {
    width: 150px;
    height: 150px;
    background-color: #3F4E4F;
}

@media (max-width:640px) {

    body {
        flex-direction: column;
    }

   .lateral {
    flex-direction: row;
    align-items: flex-start;
    width: 100%;
    order: 2;
   }

}



