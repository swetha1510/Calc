# Ex.08 Design of a Standard Calculator
## Date:26.10.23

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Calculator</title>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width" />
    <style>
        body {
            background-color: #424242;
            font-family: Tahoma;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            width: 100vw;
        }

        #container {
            width: 200px;
            padding: 8px 8px 20px 8px;
            margin: 20px auto;
            background-color: #ABABAB;
            border-radius: 4px;
            border: 2px solid #C1C1C1;
            box-shadow: -3px 3px 7px rgba(0, 0, 0, 0.6), inset -100px 0px 100px rgba(255, 255, 255, 0.5);
        }

        #display {
            display: block;
            margin: 15px auto;
            height: 42px;
            width: 227px;
            padding: 0 10px;
            border-radius: 4px;
            border: 2px solid #C1C1C1;
            background-color: #FFF;
            box-shadow: inset 0px 0px 10px #030303, inset 0px -20px 1px rgba(150, 150, 150, 0.2);
            font-size: 28px;
            color: #666;
            text-align: right;
            font-weight: 400;
        }

        .button {
            display: inline-block;
            margin: 2px;
            width: 42px;
            height: 42px;
            font-size: 16px;
            font-weight: bold;
            border-radius: 4px;
        }

        .mathButtons {
            margin: 2px 2px 6px 2px;
            color: #FFF;
            text-shadow: -1px -1px 0px #44006F;
            background-color: #434343;
            border: 2px solid #C1C1C1;
            box-shadow: 0px 0px 2px #030303, inset 0px -20px 1px #2E2E2E;
        }

        .digits {
            color: #181818;
            text-shadow: 1px 1px 0px #FFF;
            background-color: #EBEBEB;
            border: 2px solid #FFF;
            box-shadow: 0px 0px 2px #030303, inset 0px -20px 1px #DCDCDC;
        }

        .digits:hover,
        .mathButtons:hover,
        #clearButton:hover {
            background-color: #FFBA75;
            box-shadow: 0px 0px 2px #FFBA75, inset 0px -20px 1px #FF8000;
            border: 2px solid #FFF;
        }

        #clearButton {
            color: #FFF;
            text-shadow: -1px -1px 0px #44006F;
            background-color: #D20000;
            border: 2px solid #FF8484;
            box-shadow: 0px 0px 2px #030303, inset 0px -20px 1px #B00000;
        }

        .equalsButton {
            background-color: #4CAF50; /* Green color */
        }

        .equalsButton:hover {
            background-color: #66BB6A; /* Lighter green on hover */
            box-shadow: 0px 0px 2px #66BB6A, inset 0px -20px 1px #4CAF50;
            border: 2px solid #FFF;
        }
    </style>
</head>
<body>
    <div class="container">
        <fieldset id="container">
            <form name="calculator">
                <input id="display" type="text" name="display" readonly>
                <input class="button digits" type="button" value="7" onclick="calculator.display.value += '7'">
                <input class="button digits" type="button" value="8" onclick="calculator.display.value += '8'">
                <input class="button digits" type="button" value="9" onclick="calculator.display.value += '9'">
                <input class="button mathButtons" type="button" value="+" onclick="calculator.display.value += ' + '">
                <input class="button mathButtons" type="button" value="(" onclick="calculator.display.value += ' ('"><br>
                <input class="button digits" type="button" value="4" onclick="calculator.display.value += '4'">
                <input class="button digits" type="button" value="5" onclick="calculator.display.value += '5'">
                <input class="button digits" type="button" value="6" onclick="calculator.display.value += '6'">
                <input class="button mathButtons" type="button" value="-" onclick="calculator.display.value += ' - '">
                <input class="button mathButtons" type="button" value=")" onclick="calculator.display.value += ' )'"><br>
                <input class="button digits" type="button" value="1" onclick="calculator.display.value += '1'">
                <input class="button digits" type="button" value="2" onclick="calculator.display.value += '2'">
                <input class="button digits" type="button" value="3" onclick="calculator.display.value += '3'">
                <input class="button mathButtons" type="button" value="x" onclick="calculator.display.value += ' * '">
                <input class="button mathButtons" type="button" value="^" onclick="calculator.display.value += ' ** '"><br>
                <input id="clearButton" class="button" type="button" value="C" onclick="calculator.display.value = ''">
                <input class="button digits" type="button" value="0" onclick="calculator.display.value += '0'">
                <input class="button mathButtons equalsButton" type="button" value="=" onclick="calculator.display.value = eval(calculator.display.value)">
                <input class="button mathButtons" type="button" value="/" onclick="calculator.display.value += ' / '">
                <input class="button mathButtons" type="button" value="%" onclick="calculator.display.value += ' % '">
            </form>
        </fieldset>
    </div>
</body>
</html>
```

## OUTPUT:

![Screenshot 2023-11-15 181822](https://github.com/swetha1510/Calc/assets/120623583/b064ee1e-8f04-4a90-841f-d2b06f51ba0e)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
