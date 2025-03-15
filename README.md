# javascript-html
html::
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript Styling</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <div id="content">
        <img id="logo" src="logo-white.png" alt="Logo">
        <h2 id="heading">HTML</h2>
        <p id="paragraph">A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.</p>
    </div>

    <button onclick="applyStyles()">Click to Apply Styles</button>

    <script src="script.js"></script>
</body>
</html>
___________
.styled {
    background-color: lightblue;
    padding: 20px;
    border-radius: 10px;
}

.styled p {
    color: darkred;
    font-size: 18px;
    font-weight: bold;
}

__________
function applyStyles() {
    let div = document.getElementById("content");
    let heading = document.getElementById("heading");

    div.classList.add("styled"); 
    heading.textContent = "Updated Heading!";
}


