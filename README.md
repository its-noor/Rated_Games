# Rated_Games

Standalone repository for the **Q4 Interactive Visualization** project using **D3.js**.

This project creates an interactive visualization showing board game rating distributions and the most popular games for each rating.

---

## Contents

- `Q4.html` — Main visualization file  
- `average-rating.csv` — Dataset containing board game ratings  
- `lib/d3.v5.min.js` — D3 visualization library  
- `lib/d3-dsv.min.js` — CSV parsing library  
- `index.html` — Entry page for the project  

---

## Project Description

This project builds an **interactive frequency polygon line chart** using D3.js.  
The visualization displays the **count of board games by rating for each year from 2015–2019**.

### Interactive Feature

When hovering over a circle on the line chart:

- A **horizontal bar chart appears**
- It shows the **Top 5 most rated board games**
- The data corresponds to the **selected year and rating**

The length of each bar represents the **number of users who rated the game**.

---

## Dataset

The dataset used:

```
average-rating.csv
```

Columns include:

- `name` — board game name  
- `year` — year published  
- `average_rating` — average rating score  
- `users_rated` — number of users who rated the game  

Ratings are grouped using:

```
Math.floor(average_rating)
```

---

## Running the Project Locally

Because browsers block local CSV loading, run a local server.

Start the server with:

```powershell
python -m http.server 8000
```

Then open the project in your browser:

```
http://localhost:8000/Q4/Q4.html
```

Google Chrome is recommended.

---

## Technologies Used

- D3.js v5
- HTML
- CSS
- JavaScript
