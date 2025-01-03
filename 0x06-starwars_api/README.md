# 🌌 Star Wars API Explorer

Welcome to **Star Wars API Explorer**, where we boldly go where many fans have gone before—exploring galaxies far, far away with code! 🚀✨ This project leverages the power of the [SWAPI](https://swapi.dev) to fetch and display information about Star Wars films and their characters.

---

## 📜 Project Overview

This project is part of the **ALX Software Engineering program** and focuses on consuming APIs in Node.js. Specifically, it:
- Retrieves a Star Wars film by ID.
- Lists the characters from that film in their correct appearance order.
- Uses recursion to ensure data flows as smoothly as the Millennium Falcon in hyperspace.

---

## 🛠 Features

- **Galactic Data Retrieval**: Fetch any Star Wars movie details by ID.
- **Exact Character Order**: Ensure the character list is presented in the order they appeared in the movie.
- **Simple API Requests**: Built using the `request` module for easy HTTP requests.

---

## 🚀 How to Get Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/starwars_api_explorer.git
cd starwars_api_explorer
```

### 2️⃣ Install Dependencies
Ensure you have Node.js installed, then install the required package:
```bash
npm install
```

### 3️⃣ Run the Script
The script expects one argument: the ID of the Star Wars film you want to fetch. Run it like this:
```bash
./0-starwars_characters.js <film_id>
```

For example:
```bash
./0-starwars_characters.js 3
```

> **Note**: Film IDs correspond to movies in release order. For instance:
> - `1`: *A New Hope*
> - `2`: *The Empire Strikes Back*
> - `3`: *Return of the Jedi*

---

## 📂 File Structure

```plaintext
.
├── 0-starwars_characters.js  # The main script
├── package.json              # Project metadata and dependencies
├── package-lock.json         # Dependency tree lock file
└── README.md                 # This document (obviously)
```

---

## 🤓 How It Works (in Galactic Terms)

1. **Film ID Input**: Enter the film ID, and the script will hit the SWAPI to fetch film details.
2. **Character Parade**: It will extract all character URLs from the API response.
3. **Recursive Awesomeness**: Using a recursive function, the script fetches and displays each character’s name in their exact appearance order. (*Trust the Force, it works!*)

---

## 🤖 Requirements

- **Node.js**: A JavaScript runtime.
- **Internet Connection**: This isn't the 1980s; we need access to SWAPI.
- **Request Module**: Installed via `npm`.

---

## 🛡 Known Issues

- **Slow Characters**: Recursion ensures proper order but might slow things down slightly when fetching a large number of characters.
- **Film ID Confusion**: Make sure you use valid film IDs (`1–6`).

---

## 🧑‍💻 Author

Code crafted with Jedi-level care by Judith (https://github.com/Jud-et).

> **Disclaimer**: No droids, Ewoks, or Wookiees were harmed during this project.

---

## 🧩 Fun Fact

Did you know SWAPI refers to **Star Wars API**, not a new type of lightsaber? You're welcome. 🛠✨

---

May the **code** be with you. Always. ✨
