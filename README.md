# WebApplication for Event Registration

## AIM:
To create a UX design and develop a web application for event registration.
## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Choosing the suitable color scheme
### Step 3:
Creating artboards for individual pages
### Step 4:
Designing layout for individual pages
### Step 5:
Creating links and linking it with artboards
### Step 6:
Preview the prototype.


## DESIGN SCREENS:
![output](./static/img/adobe1.PNG)

![output](./static/img/adobe2.PNG)

![output](./static/img/adobe3.PNG)

![output](./static/img/adobe4.PNG)

![output](./static/img/adobe5.PNG)



## WIREFRAME:
![output](./static/img/adobewire.PNG)



## PROTOTYPE:
![output](./static/img/adobeproto.PNG)


## PROGRAM:
### home.html

<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>

    <div class="jumbotron">
        <div class="container">
            <div class="jumbotron jumbotron-fluid" style="background-color:blue;">
                <div class="container  text-center">

                    <h1 class="display-4">Robotics Event</h1>
                    <p class="lead">An Interaction with Robotics</p>
                    <hr class="my-4">
                    <p>The participants will be exposed to problem-solving activities, infrastructure of Robotics and
                        future of
                        Robotics.</p>
                </div>
                <p class="lead">

                </p>

            </div>
            <div class="container">
                <div class="row">
                    <div class="col-12">

                        <h1>Join us and learn more about Robotics</h1>
                        <p class="lead">

                        </p>

                    </div>
                </div>



                <div class="container">
                    <div class="row">
                        <div class="col-12 text-centre">
                            <a href="/register/" class="btn btn-primary" role="button"
                                aria-disabled="true">Registration</button>






                                <!-- Optional JavaScript -->
                                <!-- jQuery first, then Popper.js, then Bootstrap JS -->
                                <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
                                    integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
                                    crossorigin="anonymous"></script>
                                <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
                                    integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
                                    crossorigin="anonymous"></script>
                                <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
                                    integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
                                    crossorigin="anonymous"></script>
</body>

</html>

### register.html

<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Event Management</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
            <div class="jumbotron jumbotron-fluid" style="background-color:blue;">
                <div class="container  text-center">
            <h1 class="display-4">Robotics Event</h1>
            <p class="lead">An Interaction with Robotics</p>
            <hr class="my-4">
            <p>The participants will be exposed to problem-solving activities, infrastructure of Robotics and future of
                Robotics.</p>
            <p class="lead">

            </p>
        </div>
    </div>
    <div class="container">
         <div class="container">
            <div class="jumbotron jumbotron-fluid" style="background-color:aqua;">
                <div class="container  text-center">

        <div class="row">
            <div class="col-12">
                <h1>Application</h1>
            </div>
        </div>

        <form method="POST" action="/register/">
            {% csrf_token %}


            <div class="form-group">
                <label for="name">Name</label>
                <input type="name" class="form-control" name="username" id="username" aria-describedby="emailHelp"
                    placeholder="Enter name">
            </div>
            <div class="form-group">
                <label for="phone">Phone</label>
                <input type="phone" class="form-control" name="phone" id="phone" placeholder="phone">
            </div>
            <div class="form-group">
                <label for="exampleInputEmail1">Email address</label>
                <input type="email" class="form-control" name="exampleInputEmail1" id="exampleInputEmail1"
                    aria-describedby="emailHelp" placeholder="Enter email">
                <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone
                    else.</small>
            </div>
            <div class="form-group">
                <label for="institutionname">Institution name</label>
                <input type="institutionname" class="form-control" name="institutionname" name="institutionname"
                    id="institutionname" placeholder="institutionname">
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
        </form>

    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>

### success.html

<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
             <div class="container">
            <div class="jumbotron jumbotron-fluid" style="background-color:blue;">
                <div class="container  text-center">

            <h1 class="display-4">Robotics Event</h1>
            <p class="lead">An Interaction with Robotics</p>
            <hr class="my-4">
            <p>The participants will be exposed to problem-solving activities, infrastructure of Robotics and future of
                Robotics.</p>
            <p class="lead">

            </p>
        </div>
    </div>

    <div class="container">
         
            <div class="jumbotron jumbotron-fluid" style="background-color:aqua;">
                <div class="container  text-center">

        <div class="row">
            <div class="col-12">

                <h1>Congragulations!You're in.</h1>
                <p class="lead">We hope you have fun and learn more about robotics. Thank You and Have a great day.

                </p>
            <a href="/home/" class="btn btn-primary btn-lg active" role="button" aria-pressed="true">Home</a>
    </div>

                <!-- Optional JavaScript -->
                <!-- jQuery first, then Popper.js, then Bootstrap JS -->
                <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
                    integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
                    crossorigin="anonymous"></script>
                <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
                    integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
                    crossorigin="anonymous"></script>
                <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
                    integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
                    crossorigin="anonymous"></script>
</body>

</html>


### failed.html

<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
             <div class="container">
            <div class="jumbotron jumbotron-fluid" style="background-color:blue;">
                <div class="container  text-center">

            <h1 class="display-4">Robotics Event</h1>
            <p class="lead">An Interaction with Robotics</p>
            <hr class="my-4">
            <p>The participants will be exposed to problem-solving activities, infrastructure of Robotics and future of
                Robotics.</p>
            <p class="lead">

            </p>
        </div>
    </div>

    <div class="container">
        <div class="row">
            <div class="col-12">

                <h1>Sorry!</h1>
                <p class="lead">Try again next time.Have a good day.

                </p>
    <a href="/home/" class="btn btn-primary btn-lg active" role="button" aria-pressed="true">Home</a>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>


### participants.html

<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
             
            <div class="jumbotron jumbotron-fluid" style="background-color:blue;">
                <div class="container  text-center">

            <h1 class="display-4">Robotics Event</h1>
            <p class="lead">An Interaction with Robotics</p>
            <hr class="my-4">
            <p>The participants will be exposed to problem-solving activities, infrastructure of Robotics and future of
                Robotics.</p>
            <p class="lead">
                
            </p>
        </div>
    </div>
    <div class="container">
         <div class="container">
            <div class="jumbotron jumbotron-fluid" style="background-color:aqua;">
                <div class="container  text-center">

        <div class="row">
            <div class="col-12">
                <h1>Congragulations!</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-12">
                <table class="table">
                    <thead>
                        <tr>
                            <th scope="col">NAME</th>
                            <th scope="col">EMAIL</th>
                            <th scope="col">PHONE</th>
                            <th scope="col">INSTITUTION</th>
                        </tr>
                    </thead>
                    <tbody>

                        <tr>
                            <td>Kamal</td>
                            <td>raja@gmail.com</td>
                            <td>1564820000</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Sandhya</td>
                            <td>sandhya@gmail.com</td>
                            <td>23424200000</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Akshay</td>
                            <td>akshay@gmail.com</td>
                            <td>1234567890</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Sasi Reddy</td>
                            <td>reddy@gmail.com</td>
                            <td>2342200350</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Ajay</td>
                            <td>ajay@gmail.com</td>
                            <td>1599517530</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Sierra</td>
                            <td>sierra@gmail.com</td>
                            <td>7533572580</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Vishal</td>
                            <td>vishal@gmail.com</td>
                            <td>1477413690</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Sandy</td>
                            <td>sandy@gmail.com</td>
                            <td>3699632580</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Linda</td>
                            <td>linda@gmail,com</td>
                            <td>3216549870</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Tia</td>
                            <td>tia@gmail.com</td>
                            <td>7894561230</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Ziya</td>
                            <td>ziya@gmail.com</td>
                            <td>1234567890</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Willson</td>
                            <td>will@gmail.com</td>
                            <td>4561237890</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Karl</td>
                            <td>karl@gmail.com</td>
                            <td>7891234560</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Shalini</td>
                            <td>shalini@gmail.com</td>
                            <td>1473692580</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>Anu</td>
                            <td>anu@gmail.com</td>
                            <td>2583691470</td>
                            <td>Saveetha</td>
                        </tr>


                    </tbody>
                </table>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <a href="/home/" class="btn btn-primary btn-lg" role="button">Home</a>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>


## OUTPUT:
![output](./static/img/output1.png)

![output](./static/img/output2.png)

![output](./static/img/output3.png)

![output](./static/img/output4.png)


## RESULT:
 Thus, a UX design is created and a web application is developed for event registration is the url http://sanjnapriya.student.saveetha.in:8000/home/.