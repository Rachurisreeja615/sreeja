# sreeja
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fun Fact Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        #fun-fact {
            margin: 20px;
            font-size: 1.5em;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
        }
    </style>
</head>
<body>

<h1>Fun Fact Generator</h1>
<div id="fun-fact">Click the button to see a fun fact!</div>
<button onclick="showFunFact()">Get Fun Fact</button>

<script>
    function showFunFact() {
        const facts = [
            "Honey never spoils. Archaeologists have found pots of honey in ancient Egyptian tombs that are over 3,000 years old and still perfectly edible.",
            "A day on Venus is longer than a year on Venus. It takes Venus longer to rotate once on its axis (243 Earth days) than it does to complete one orbit of the Sun (225 Earth days).",
            "Bananas are berries, but strawberries aren't. Botanically speaking, a berry is a fruit produced from the ovary of a single flower with seeds embedded in the flesh.",
            "There are more stars in the universe than grains of sand on all the Earth's beaches. Scientists estimate there are about 100 billion galaxies, each containing millions or billions of stars.",
            "Octopuses have three hearts. Two pump blood to the gills, while the third pumps it to the rest of the body."
        ];
        const randomFact = facts[Math.floor(Math.random() * facts.length)];
        document.getElementById("fun-fact").innerText = randomFact;
    }
</script>

</body>
</html>
