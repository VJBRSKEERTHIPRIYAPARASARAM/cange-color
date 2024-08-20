# cange-color
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Assignment 3</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .container {
            width: 300px;
            height: 200px;
            background-color: lightblue;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 20px auto;
            transition: background-color 0.3s ease;
        }
        .btn-toggle {
            position: relative;
            display: inline-block;
            padding: 10px 20px;
            background-color: gray;
            color: white;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        input[type="checkbox"] {
            display: none;
        }
        input[type="checkbox"]:checked ~ .container {
            background-color: coral;
        }
        input[type="checkbox"]:checked ~ .btn-toggle {
            background-color: black;
            color: white;
        }
        input[type="checkbox"]:checked ~ .container span {
            color: white;
        }
    </style>
</head>
<body>

<input type="checkbox" id="toggle">
<label for="toggle" class="btn-toggle">Press Me</label>

<div class="container">
    <span>This is a container</span>
</div>

</body>
</html>
