async function searchRecipe() {
  const query = document.getElementById("foodInput").value.trim();
  const resultsDiv = document.getElementById("results");
  resultsDiv.innerHTML = "<p>Searching...</p>";

  if (!query) {
    resultsDiv.innerHTML = "<p>Please enter a food item.</p>";
    return;
  }

  try {
    // Fetch meals by ingredient
    const res = await fetch(https://www.themealdb.com/api/json/v1/1/filter.php?i=${query});
    const data = await res.json();

    if (!data.meals) {
      resultsDiv.innerHTML = "<p>No recipes found for that ingredient.</p>";
      return;
    }

    resultsDiv.innerHTML = "";

    // For each meal, fetch full details
    for (let meal of data.meals.slice(0, 5)) { // Limit to 5 recipes
      const detailRes = await fetch(https://www.themealdb.com/api/json/v1/1/lookup.php?i=${meal.idMeal});
      const detailData = await detailRes.json();
      const mealDetails = detailData.meals[0];

      const recipeDiv = document.createElement("div");
      recipeDiv.className = "recipe";
      recipeDiv.innerHTML = `
        <img src="${mealDetails.strMealThumb}" alt="${mealDetails.strMeal}">
        <h2>${mealDetails.strMeal}</h2>
        <p><strong>Category:</strong> ${mealDetails.strCategory}</p>
        <p><strong>Area:</strong> ${mealDetails.strArea}</p>
        <h3>Instructions:</h3>
        <p>${mealDetails.strInstructions}</p>
        <a href="${mealDetails.strYoutube}" target="_blank">▶ Watch Video</a>
      `;

      resultsDiv.appendChild(recipeDiv);
    }

  } catch (error) {
    resultsDiv.innerHTML = "<p>Error fetching recipes. Try again later.</p>";
  }
}
