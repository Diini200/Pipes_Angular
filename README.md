Pipes(|) in angular:
================
Angular supports pipes.The main objective of pipes in angular is to tranform 
the data or information as per the application reqn.Angular supports two types of
pipes

->Predefine pipes
->Custom pipes

->Predefine pipes:
=================
Angular supports following predefine pipes 

->uppercase
->lowercase
->currency
->date

application4---->src---->app---->Players--->Players.compoment.html
==================================================================
<!doctype html>
<html lang="en">
  <head>
 
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">


    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
    <title>PAGE LAYOUTS</title>
  </head>
  <body>
    <div class="container">
        <div class="row">
            <div class="col-md-12">
                <h1 class="text-center text-white bg-danger">International Cricket Players</h1>
                <hr>
                <table class="table table-bordered table-striped table-hover">
                    <tr>
                        <th>Name</th>
                        <th>DOB</th>
                        <th>TEAM</th>
                        <th>FOURS</th>
                        <th>SIXES</th>
                        <th>OTHERS</th>
                        <th>Prices</th>
                    </tr>
                    <tr *ngFor="let P1 of Players">
                        <td>{{P1.Name|uppercase}}</td>
                        <td>{{P1.DOB|date:'dd-MM-yyyy'}}</td>
                        <td>{{P1.Team|lowercase}}</td>
                        <td>{{P1.Fours}}</td>
                        <td>{{P1.Sixes}}</td>
                        <td>{{P1.Others}}</td>
                        <td>{{P1.Price|currency:'INR'}}</td>

                    </tr>

                </table>
                <hr>
            </div>
        </div>
    </div>
  

 

 <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
  </body>
</html>


Working on Custome or user_define pipes:
=======================================
Angular supports Custom pipes or user_define pipes.Custom pipes or user_define pipes can be represent as
if the angular developers are create their own pipes as per the applicaiton requirement or user_define pipes.

ng generate pipe pipe_name

or 

ng g p pipe_name

