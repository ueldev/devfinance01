# devfinance01
primeiro app/site de finanças. *em andamento*
/* ///////////////////////////////////////// */

<!DOCTYPE html>
<html lang="en">
    
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">

        

        
        <link rel="stylesheet" href="style.css">
        <link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
        <title>dev.finances$</title>

    <body>
        
        <header>
            <h1 id="logo">dev.balance$</h1>
        </header>
    
            

        <main class="caixa">
            <section id="balance">

                <h2>BALANCE</h2>


                <div class="card">
                    <h3>Entry</h3>
                    <p> R$ 8.000,00</p>
                </div>

                <div class="card">
                    <h3>Outings</h3>
                    <p> R$ 6.000,00</p>
                </div>

                <div class="card total">
                    <h3>Total</h3>
                    <p> R$ 2.000,00</p>

                </div>
            </section>
        </main>


    <main class="caixa">


            <section id="transactions">
            <h2>TRANSACTIONS</h2>
            </section>

            <section>
                <table id="data-table">
                    <thead>
                        <tr>
                            <th>Decription</th>
                            <th>Value</th>
                        <th>Date</th>
                        </tr>
                    </thead>

                    <tbody>
                        <tr>
                            <td class= "description">Luz</td>
                            <td class= "expense" > -R$230,00</td>
                            <td class= "date">14/05/2021</td>
                        </tr>
                        <tr>
                            <td class= "description">Website Create</td>
                            <td class= "income">R$ 8.000,00</td>
                            <td class= "date">15/05/2021</td>
                        </tr>
                        <tr>
                            <td class= "description">Internet</td>
                            <td class= "expense"> -R$ 110,00</td>
                            <td class= "date">05/05/2021</td>

                        </tr>
                    </tbody>
                </table>
            </section>
        </main>


        <footer>
            <p>dev.finances$</p>
        </footer>
    </body>

</html>

/* ----------- CSS ----------- */



/* global */

*{
    margin: 0px; 
    padding: 0;
    box-sizing: border-box;
    
}

body{
    background: rgb(242, 241, 255);
    font-family: 'Montserrat', sans-serif;
}

.caixa{
    width: min(90vw, 800px);

    margin: auto;
}

/* titles ///////////////////////// */

h2{
    margin-top: 3.2rem;
    margin-bottom: 0.8rem;

    color: rgb(0, 8, 78);
    font-weight: normal;
}


/* header ///////////////////////// */

header{
    background: rgb(0, 8, 78);
    padding: 2rem 0rem 10rem;
    font-family: 'Montserrat', sans-serif;
    text-align: center;
    font-size: 15px;
    
}

#logo{
    font-weight: 200;
    color: rgb(255, 255, 255);
}


/* balance ///////////////////////////// */

#balance{
    margin-top: -5rem;
}

#balance h2{
    color: white;
    margin-top: 0;
}

/* card ////////////////////////////// */

.card{
    background: rgb(241, 226, 255);
    padding: 1.5rem 2rem;
    border-radius: 0.30rem;
    margin-bottom: 2rem;
}

.card h3{
    font-weight: normal;
    font-size: 1.5rem;  
}

.card p{
    font-size: 2rem;
    line-height: 2.5rem;

    margin-top: 1rem;
}
.card.total{
    background: rgb(0, 201, 10);
    color: white;
}

/* table ////////////////////////////// */

#data-table{
    width: 100%;
    border-spacing: 0 0.5rem;
    color: rgb(80, 80, 80)
}

table th{
    background: rgb(230, 231, 255);
    
    font-weight: normal;
    padding: 1rem 2rem;

    text-align: left;
    color: rgb(0, 8, 78);
}

table td{
    background: white;
    padding: 1rem 2rem;
}

table thead tr th:first-child,
table tbody tr td:first-child{
    border-radius: 0.25rem 0 0 0.25rem;

}

table tbody tr {
    opacity: 0.7;
}

table tbody tr:hover {
    opacity: 1;
}

td.description{
    color: rgb(0, 8, 78);
}

td.income{
    color: rgb(0, 201, 10);
}
td.expense{
    color: red;
}

/* footer ///////////////////////////// */

footer{
    text-align: center;
    padding: 4rem 0rem 2rem;
    color: rgb(0, 8, 78);
    opacity: 0.8;
}
