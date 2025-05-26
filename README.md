<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Interactive Page</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1 id="main-title">Welcome to My Page</h1>
  </header>

  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <main>
    <section>
      <p id="description">Click the button to change this text and style.</p>
      <button id="action-btn">Do Something</button>
    </section>

  
  </main>

  <footer>
    <p>&copy; 2025 My Website</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>

              This is my Js
document.getElementById("action-btn").addEventListener("click", function () {
  const desc = document.getElementById("description");
  desc.textContent = "The text has changed!";
  desc.style.color = "blue";
  desc.style.fontWeight = "bold";

  const container = document.getElementById("dynamic-container");
  
  if (!document.getElementById("new-element")) {
    // Create and add new element
    const newPara = document.createElement("p");
    newPara.id = "new-element";
    newPara.textContent = "This element was added dynamically!";
    container.appendChild(newPara);
  } else {
    // Remove the element
    container.removeChild(document.getElementById("new-element"));
  }
});

     This is my css
     
     body {
  font-family: Arial, sans-serif;
  margin: 20px;
  line-height: 1.6;
}

header, nav, main, footer {
  margin-bottom: 20px;
}

button {
  padding: 10px 15px;
  font-size: 16px;
}


      
