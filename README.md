# MWAD-EXP_04-Simple-caluculator
## Date:22-10-2025

## AIM
To  develop a Simple Calculator using React.js with clean and responsive design, ensuring a smooth user experience across different screen sizes.

## ALGORITHM
### STEP 1
Create a React App.

### STEP 2
Open a terminal and run:
  <ul><li>npx create-react-app simple-calculator</li>
  <li>cd simple-calculator</li>
  <li>npm start</li></ul>

### STEP 3
Inside the src/ folder, create a new file Calculator.js and define the basic structure.

### STEP 4
Plan the UI: Display screen, number buttons (0-9), operators (+, -, *, /), clear (C), and equal (=).

### STEP 5
Create a new file Calculator.css in src/ and add the styling.

### STEP 6
Open src/App.js and modify it.

### STEP 7
Start the development server.
  npm start

### STEP 8
Open http://localhost:3000/ in the browser.

### STEP 9
Test the calculator by entering numbers and operations.

### STEP 10
Fix styling issues and refine content placement.

### STEP 11
Deploy the website.

### STEP 12
Upload to GitHub Pages for free hosting.

## PROGRAM
```
calc.html

<html >
<head>

    <title>Simple Calculator</title>
    <style>
        #calc {
            text-align: center;
            margin: auto;
            width: 240px;
        }
        .button {
            margin-left: 550px;
            margin-right: 550px;
            padding: 30px;
            background-color:rgb(155, 187, 150);
            color: rgb(168, 104, 104);
            border:5px solid rgb(67, 72, 82)
        }

        .button input[type="button"] {
            background-color:coral;
            height: 50px;
            width: 50px;
            margin: 0 2px;
            border: 3px solid burlywood;
        }
    </style>
</head>

<body style="background-color: black;">
        <h1 align="center" style="color: aliceblue;">SARANYA CALCULATOR</h1>
        <h1 align="center" style="color: blanchedalmond">REGISTER NUMBER:212223040188</h1> </h1>
        <div class="button">
            <center>
            
            <input type="text" id="t1" style="width:270px; height:30px;"><br><br>
            <input type="button" onkeydown="op(event)" onclick="f('7')" value="7">
            <input type="button" onkeydown="op(event)" onclick="f('8')" value="8">
            <input type="button" onkeydown="op(event)" onclick="f('9')" value="9">
            <input type="button" onkeydown="op(event)" onclick="f('+')" value="+">
            <input type="button" onkeydown="op(event)" value="C"  onclick="clr()"><br><br>

            <input type="button" onkeydown="op(event)" onclick="f('4')" value="4">
            <input type="button" onkeydown="op(event)" onclick="f('5')" value="5">
            <input type="button" onkeydown="op(event)" onclick="f('6')" value="6">
            <input type="button" onkeydown="op(event)" onclick="f('*')" value="x">
            <input type="button" onkeydown="op(event)" onclick="f('^0.5')" value="&radic;"><br><br>
    
            <input type="button" onkeydown="op(event)" onclick="f('1')" value="1">
            <input type="button" onkeydown="op(event)" onclick="f('2')" value="2">
            <input type="button" onkeydown="op(event)" onclick="f('3')" value="3">
            <input type="button" onkeydown="op(event)" onclick="f('-')" value="-">
            <input type="button" onkeydown="op(event)" onclick="f('/')" value="%"><br><br>
        
            <input type="button" onkeydown="op(event)" onclick="f('0')" value="0">
            <input type="button" onkeydown="op(event)" onclick="f('.')"
                value=".">
            
            <input type="button" onkeydown="op(event)" onclick="f('+')" value="+">
            <input type="button" onclick="solve()" value="=" style="color: blue; width:110px;font-weight:bolder;">
        </center>
        </div>
</body>
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjs/9.4.4/math.js"></script>

<script>
    function f(val) {
        document.getElementById('t1').value += val;
    }

    function clr() {
        document.getElementById('t1').value = "";
    }

    function op(event) {
        if (event.key == '7' || event.key == '8' || event.key == '9' || event.key == '+' || event.key == '+/-' || event.key == '4' ||
            event.key == '5' || event.key == '6' || event.key == '*' || event.key == '^0.5' || event.key == '1' ||
            event.key == '2' || event.key == '3' || event.key == '-' || event.key == '/' || event.key == '0' || event.key == '.') {
            document.getElementById('t1').value += event.key;
        }
    }

    var cal = document.getElementById('calc');
    cal.onkeyup = function (event) {
        if (event.keyCode == 13) {
            console.log("Enter");
            solve();
        }
    }

    function solve() {
        let x = document.getElementById('t1').value;
        let y = math.evaluate(x); // Assuming you have included the math.js library
        document.getElementById('t1').value = y;
    }
</script>

</html>
```

## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ab0149ee-c383-4b59-8140-464377646317" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6cf304d7-eb80-4c29-87d2-cdd065b5a1de" />

## RESULT
The program for developing a simple calculator in React.js is executed successfully.
