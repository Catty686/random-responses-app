# random-responses-app
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Response App</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Random Response App</h1>
    <button id="responseButton">Get Random Response</button>
    <p id="response"></p>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    text-align: center;
    margin-top: 50px;
}

button {
    padding: 10px 20px;
    font-size: 16px;
}

p {
    font-size: 20px;
    margin-top: 20px;
}
const responses = [
 "Yes",
        "No",
        "Maybe",
        "It is certain",
        "Outlook not so good",
        "Ask again later",
        "Better not tell you now",
        "Cannot predict now",
        "Concentrate and ask again",
        "Don't count on it",
        "Very likely",
        "Not looking good",
        "Definitely yes",
        "Absolutely not",
        "The stars say no",
        "Signs point to yes",
        "It is decidedly so",
        "My sources say no",
        "You may rely on it",
        "Reply hazy, try again",
        "As I see it, yes",
        "Most likely",
        "My reply is no",
        "Without a doubt",
        "Very doubtful",
        "It is not certain",
        "Certainly not",
        "Absolutely",
        "Not in a million years",
        "The outlook is good",
        "Chances are high",
        "Highly unlikely",
        "In your dreams",
        "The answer is hiding from you"
];

document.getElementById('responseButton').addEventListener('click', () => {
    const randomResponse = responses[Math.floor(Math.random() * responses.length)];
    document.getElementById('response').textContent = randomResponse;
});

