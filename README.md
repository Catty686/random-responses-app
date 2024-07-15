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
    "Ask again later",
    "Definitely",
    "I don't think so"
];

document.getElementById('responseButton').addEventListener('click', () => {
    const randomResponse = responses[Math.floor(Math.random() * responses.length)];
    document.getElementById('response').textContent = randomResponse;
});
