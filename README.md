<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Wewe Sass Research</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <header>
      <h1>Wewe Sass Research</h1>
      <button id="toggleLang">Kreyòl</button>
    </header>

    <div class="search-bar">
      <input type="text" id="searchInput" placeholder="Search for anything..." />
      <button onclick="handleSearch()">Search</button>
    </div>

    <div id="results" class="results"></div>

    <footer>
      <p><strong>Piblisite:</strong> Dekouvri mond lan ak Wewe Sass!</p>
    </footer>
  </div>

  <script src="script.js"></script>
</body>
</html>body {
  margin: 0;
  font-family: sans-serif;
  background: #f9f9f9;
  color: #222;
}

.container {
  max-width: 600px;
  margin: auto;
  padding: 20px;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

h1 {
  color: #0d6efd;
  font-size: 1.8rem;
}

.search-bar {
  display: flex;
  gap: 10px;
  margin-bottom: 20px;
}

input[type="text"] {
  flex: 1;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-size: 16px;
}

button {
  padding: 10px 16px;
  background: #0d6efd;
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

button:hover {
  background: #0b5ed7;
}

.results {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.result-card {
  background: white;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 1px 4px rgba(0,0,0,0.1);
}

.result-card a {
  color: #0d6efd;
  text-decoration: underline;
  display: block;
  margin-top: 5px;
}

footer {
  margin-top: 40px;
  font-size: 14px;
  text-align: center;
  color: gray;
}const searchInput = document.getElementById("searchInput");
const resultsDiv = document.getElementById("results");
const langBtn = document.getElementById("toggleLang");

let currentLang = "en";

function handleSearch() {
  const query = searchInput.value.trim();
  resultsDiv.innerHTML = "";

  if (query === "") return;

  // Fè ti rezilta fiktiv pou demo a
  const fakeResults = [
    {
      title: currentLang === "en" ? "Video: What is the Sun?" : "Videyo: Ki sa ki Solèy la?",
      url: "https://youtube.com/watch?v=solèy",
    },
    {
      title: currentLang === "en" ? "Image: Galaxy" : "Imaj: Galaksi",
      url: "https://bing.com/images/galaxy",
    },
    {
      title: currentLang === "en" ? "Wikipedia: Universe" : "Wikipedya: Linivè",
      url: "https://wikipedia.org/wiki/Universe",
    },
  ];

  fakeResults.forEach((item) => {
    const card = document.createElement("div");
    card.className = "result-card";
    card.innerHTML = `
      <strong>${item.title}</strong>
      <a href="${item.url}" target="_blank">${item.url}</a>
    `;
    resultsDiv.appendChild(card);
  });
}

// Bouton pou chanje lang
langBtn.addEventListener("click", () => {
  currentLang = currentLang === "en" ? "ht" : "en";
  searchInput.placeholder = currentLang === "en" ? "Search for anything..." : "Rechèch nenpòt bagay...";
  langBtn.textContent = currentLang === "en" ? "Kreyòl" : "English";
});<div class="gcse-search"></div><head>
  <meta charset="UTF-8" />
  <title>Wewe Sass Research</title>
  <script async src="https://cse.google.com/cse.js?cx=b331104695f1a470f"></script>
</head>
<body>
  <h1>Welcome to Wewe Sass Research</h1>
  <input type="text" id="searchInput" placeholder="Rechèch..." />
  <button onclick="startSearch()">Rechèch</button>

  <!-- Rezilta Google CSE -->
  <div class="gcse-search"></div>
</body><script async src="https://cse.google.com/cse.js?cx=b331104695f1a470f"></script><body>
  <h1>Welcome to Wewe Sass Research</h1>
  
  <input type="text" id="searchInput" placeholder="Rechèch...">
  <button onclick="startSearch()">Rechèch</button>

  <!-- Moun ap wè rezilta rechèch yo la -->
  <div class="gcse-search"></div>
</body><body>
  <h1>Welcome to Wewe Sass Research</h1>
  
  <input type="text" id="searchInput" placeholder="Rechèch...">
  <button onclick="startSearch()">Rechèch</button>

  <!-- Moun ap wè rezilta rechèch yo la -->
  <div class="gcse-search"></div>
</body><!-- CSE Script -->
<script async src="https://cse.google.com/cse.js?cx=b331104695f1a470f"></script>
<div class="gcse-search"></div><div class="help">
    <h3>❓ Bezwen Èd?</h3>
    <button class="button" onclick="alert('Tanpri dekri pwoblèm ou a pou AI asistans lan ka ede.')">Klike pou èd</button>
</div><div class="help">
    <h3>❓ Bezwen Èd?</h3>
    <button class="button" onclick="alert('Tanpri dekri pwoblèm ou a pou AI asistans lan ka ede.')">Klike pou èd</button>
  </div>

  <!-- Google Custom Search -->
  <div class="product">
    <h3>🔎 Rechèch sou entènèt (CSE)</h3>
    <script async src="https://cse.google.com/cse.js?cx=b331104695f1a470f"></script>
    <div class="gcse-search"></div>
  </div>


