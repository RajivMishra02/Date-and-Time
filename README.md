# Date-and-Time
This is a Website which is made using HTML, CSS to form and give a shape and JavaScript to make the Website dynamic and functional.  The Website provides the current date and time without having to refresh the page.
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css"
        integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">

    <title>Date and Time</title>
    <script>
        let a;
        let date;
        let time;
        const options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
        setInterval(() => {
            a = new Date(); 
            date = a.toLocaleDateString(undefined, options);
            time = a.getHours() + ':' + a.getMinutes() + ':' + a.getSeconds();
            document.getElementById('time').innerHTML = time + "<br>on " + date;
        }, 1000);
    </script>
    <style>
       .dropdown-item{
            color: blueviolet;
       }
       .navbar-brand{
        background-color: lightblue;
        border: 2px solid yellow;
        border-radius: 8px;
       }
       .nav-link{
        background-color: lightblue;
        border: 2px solid yellow;
        border-radius: 8px;
       }
    </style>
</head>

<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#">Date and Time</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                    <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Date</a>
                </li>
                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                        data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Countries
                    </a>
                    <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <a class="dropdown-item" href="#">USA</a>
                        <a class="dropdown-item" href="#">Australia</a>
                        <a class="dropdown-item" href="#">Norway</a>
                        <a class="dropdown-item" href="#">Switzerland</a>
                        <a class="dropdown-item" href="#">Canada</a>
                        <a class="dropdown-item" href="#">Pakistan</a>
                        <div class="dropdown-divider"></div>
                        <a class="dropdown-item" href="#">Type Your Country Name Here</a>
                    </div>
                </li>
                
            </ul>
            <form class="form-inline my-2 my-lg-0">
                <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
                <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
            </form>
        </div>
    </nav>



    <div class="container my-4">
        <div class="jumbotron">
            <h1 class="display-4">Current time Is: <span id="time"></span></h1>
            <p class="lead"><b>We have got you covered!!</b></p>
            <hr class="my-4">
            <p>Want to get updated with time! Check Here!</p>
            <a class="btn btn-primary btn-lg" href="#" role="button">Browse Time</a>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"
        integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj"
        crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js"
        integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo"
        crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js"
        integrity="sha384-OgVRvuATP1z7JjHLkuOU7Xw704+h835Lr+6QL9UvYjZE3Ipu6Tp75j7Bh/kR0JKI"
        crossorigin="anonymous"></script>
</body>

</html>
