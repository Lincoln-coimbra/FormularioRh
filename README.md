# FormularioRh

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">

    <title>formulario de ferias</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: grid;
            place-items: center;
            height: 100vh;
            margin: 0;
            background:rgb(187, 243, 155)
        }
        form {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-template-rows: repeat(3, auto);
            grid-gap: 10px;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 8px;
            background-color: #f9f9f9;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        label {
            grid-column: 1;
            grid-row: span 1;
            font-weight: bold;

        }
        input[type="text"],
        input[type="date"],
        select,
        input[type="number"] {
            grid-column: span 2;
            width: calc(100% - 20px);
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #d9d3d3;
            border-radius: 4px;
            box-sizing: border-box;
        }
        input[type="submit"] {
            grid-column: span 3;
            background-color: #4CAF50;
            color: rgb(255, 255, 255)55, 255, 255);
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #45a049;
        }
        .warning {
            grid-column: span 3;
            background-color: #f2dede;
            border: 1px solid #ebccd1;
            color: #a94442;
            padding: 10px;
            border-radius: 4px;
        }
         
        
        
        
.gg-calendar-dates {
 box-sizing: border-box;
 position: relative;
 display: block;
 transform: scale(var(--ggs,3));
 width: 30px;
 height: 30px;
 border: 3px solid;
 border-radius: 3px
}

.gg-calendar-dates::after,
.gg-calendar-dates::before {
 content: "";
 display: block;
 box-sizing: border-box;
 position: absolute;
 border-radius: 5px;
 height: 2px;
 left: 2px
}

.gg-calendar-dates::before {
 background: currentColor;
 width: 4px;
 box-shadow:
 4px 0 0,8px 0 0,0 4px 0,
 4px 4px 0,8px 4px 0;
 top: 15px
}

.gg-calendar-dates::after {
 width: 20px;
 top: -4px;
 box-shadow: 0 8px 0 0
} 
select[name="status"] option[value="Pendente"] {
    
    background-color: #f00707c3;
}
select[name="status"] option[value="Solicitando"] {
    background-color: #07f00fc3;
}
input[text=option] option[value="Solicitando"]{
  background-color: #3CBC8D;
  color: rgb(128, 8, 8);
}
.status {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 0px 14px;
    gap: 8px;
    width: 300px;
    height: 56px;
    flex: none;
    order: 0;
    align-self: stretch;
    flex-grow: 0;
    background: rgba(255, 0, 0, 0.0);
    border-radius: 8px;
    border: none;
    backface-visibility
}

    </style>
</head>
<body>
    <i class="gg-calendar-dates"></i>
<h1>SOLICITAÇÃO DE FÉRIAS</h1>
    <form action="#">
        <label for="colaborador">Colaborador:</label>
        <input type="text" id="colaborador" name="colaborador">
        <label for="data">Data:</label>
        <input type="date" id="data_entrada" name="data_entrada" placeholder="Data de Entrada">

        <label for="status">Status:</label>
        <select id="status" name="status"class"status">
        </select> id="solicitando" name="solicitando" class
            <option value="Solicitando">Solicitando</option>
            <option value="Pendente">Pendente</option>
        </select>

        <label for="departamento">Departamento:</label>
        <input type="text" id="departamento" name="departamento">

        <label for="centro_custo">Centro de Custo:</label>
        <input type="text" id="centro_custo" name="centro_custo">

        <label for="unidade_negocio">Unidade de Negócio:</label>
        <input type="text" id="unidade_negocio" name="unidade_negocio">

        <label for="periodo_aquisitivo_inicio">Período Aquisitivo (Início):</label>
        <input type="date" id="periodo_aquisitivo_inicio" name="periodo_aquisitivo_inicio">

        <label for="periodo_aquisitivo_fim">Período Aquisitivo (Fim):</label>
        <input type="date" id="periodo_aquisitivo_fim" name="periodo_aquisitivo_fim">

        <label for="dias_saldo">Dias de Saldo:</label>
        <input type="number" id="dias_saldo" name="dias_saldo" min="0">

        <label for="limite">Limite:</label>
        <input type="date" id="limite" name="limite">

        <label for="inicio_ferias">Início das Férias:</label>
        <input type="date" id="inicio_ferias" name="inicio_ferias">

        <label for="final_ferias">Final das Férias:</label>
        <input type="date" id="final_ferias" name="final_ferias">

        <label for="abono">Abono:</label>
        <select id="abono" name="abono">
            <option value="sim">Sim</option>
            <option value="nao">Não</option>
        </select>

        <label for="decimo_terceiro">1° PARC. DO 13° SALÁRIO:</label>
        <select id="decimo_terceiro" name="decimo_terceiro">
            <option value="SIM">SIM</option>
            <option value="nao">Não</option>
        </select>

        <input type="submit" value="Enviar">
    </form>

    <div class="warning">
        Por favor, não esqueça de entregar sua carteira de trabalho para assinar as férias.
    </div>
</body>
</html>
