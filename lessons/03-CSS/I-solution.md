# Solution: Building a Simple Recipe Webpage

Let`s create a stunning recipe for Omelette :)

### **index.html**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="icon" type="image/x-icon" href="assets/images/favicon-32x32.png">
  <title>Simple Omelette Recipe</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<div class="container">
  <div class="image-container">
    <img src="assets/images/image-omelette.jpeg" alt="Omelette Image">
  </div>
  <div class="content">
    <h1>Simple Omelette Recipe</h1>
    <p class="description">An easy and quick dish, perfect for any meal. This classic omelette combines beaten eggs
      cooked
      to perfection, optionally filled with your choice of cheese, vegetables, or meats.</p>

    <div class="prep-time">
      <h3>Preparation time</h3>
      <ul>
        <li><strong>Total:</strong> Approximately 10 minutes</li>
        <li><strong>Preparation:</strong> 5 minutes</li>
        <li><strong>Cooking:</strong> 5 minutes</li>
      </ul>
    </div>

    <h2>Ingredients</h2>
    <ul class="ingredients">
      <li>2-3 large eggs</li>
      <li>Salt, to taste</li>
      <li>Pepper, to taste</li>
      <li>1 tablespoon of butter or oil</li>
      <li>Optional fillings: cheese, diced vegetables, cooked meats, herbs</li>
    </ul>

    <hr />

    <h2>Instructions</h2>
    <ol class="instructions">
      <li><strong>Beat the eggs:</strong> In a bowl, beat the eggs with a pinch of salt and pepper until they are
        well
        mixed. You can add a tablespoon of water or milk for a fluffier texture.
      </li>
      <li><strong>Heat the pan:</strong> Place a non-stick frying pan over medium heat and add butter or oil.</li>
      <li><strong>Cook the omelette:</strong> Once the butter is melted and bubbling, pour in the eggs. Tilt the
        pan
        to
        ensure the eggs evenly coat the surface.
      </li>
      <li><strong>Add fillings (optional):</strong> When the eggs begin to set at the edges but are still slightly
        runny
        in the middle, sprinkle your chosen fillings over one half of the omelette.
      </li>
      <li><strong>Fold and serve:</strong> As the omelette continues to cook, carefully lift one edge and fold it
        over
        the
        fillings. Let it cook for another minute, then slide it onto a plate.
      </li>
      <li><strong>Enjoy:</strong> Serve hot, with additional salt and pepper if needed.</li>
    </ol>
    <hr />
    <h2>Nutrition</h2>
    <p class="nutrition">The table below shows nutritional values per serving without the additional fillings.</p>
    <table class="nutrition-table">
      <tr>
        <th>Calories</th>
        <td>277kcal</td>
      </tr>
      <tr>
        <th>Carbs</th>
        <td>0g</td>
      </tr>
      <tr>
        <th>Protein</th>
        <td>20g</td>
      </tr>
      <tr>
        <th>Fat</th>
        <td>22g</td>
      </tr>
    </table>
  </div>
</div>

</body>
</html>
```

### **styles.css**

```css
@font-face {
    font-family: YoungSerif;
    src: url(assets/fonts/young-serif/YoungSerif-Regular.ttf);
    font-weight: 400;
}

@font-face {
    font-family: Outfit;
    src: url(assets/fonts/outfit/static/Outfit-Regular.ttf);
    font-weight: 400;
}

@font-face {
    font-family: Outfit;
    src: url(assets/fonts/outfit/static/Outfit-SemiBold.ttf);
    font-weight: 600;
}


body {
    font-family: 'Outfit', sans-serif;
    font-weight: 400;
    background-color: #f9f3ef;
    color: #4a4a4a;
    margin: 0;
    padding: 20px;
}

h1, h2 {
    font-family: 'YoungSerif', sans-serif;
    font-weight: 400;
}

.container {
    max-width: 700px;
    margin: 0 auto;
    background-color: white;
    border-radius: 24px;
}

.image-container {
    padding: 48px 48px 0 48px;
}

.content {
    padding: 0 48px 48px 48px;
}

.image-container img {
    width: 100%;
    height: auto;
    border-radius: 24px;
}

h1 {
    font-size: 32px;
    color: #333;
    margin-top: 20px;
    text-align: left;
}

.description {
    font-size: 16px;
    text-align: left;
    color: #666;
    margin-bottom: 20px;
}

.prep-time {
    background-color: #fbeff3;
    padding: 15px;
    border-radius: 8px;
    margin-bottom: 20px;
}

.prep-time h3 {
    font-family: 'Outfit', sans-serif;
    font-weight: 600;
    margin: 0 0 10px 20px;
    font-size: 18px;
    color: #7B284FFF
}


.prep-time li {
    margin-bottom: 10px;
    padding: 0 20px;
}

.prep-time li::marker {
    color: #7B284FFF
}

h2 {
    font-size: 24px;
    color: #b45f06;
    margin-bottom: 10px;
}

.ingredients li,
.instructions li {
    margin-bottom: 10px;
    line-height: 1.5;
    padding: 0 20px;
}

.instructions li {
    position: relative;
    padding-left: 25px;
}

.instructions li::marker, .ingredients li::marker {
    color: #854632FF;
    font-weight: bold;
}

hr {
    background-color: #ddd;
    height: 1px;
    border: 0;
    margin: 40px 0;
}

.nutrition {
    color: #666;
    margin-bottom: 10px;
}

.nutrition-table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 10px;
}

.nutrition-table th,
.nutrition-table td {
    padding: 10px;
    text-align: left;
    border-bottom: 1px solid #ddd;
}

.nutrition-table th {
    color: #666;
    font-weight: 400;
}

.nutrition-table td {
    color: #b45f06;
    font-weight: 600;
}

@media (max-width: 375px) {
    .image-container {
        padding: 0;
    }

    .image-container img {
        border-radius: 0;
    }

    .content {
        padding: 0 24px 24px 24px;
    }

    h1 {
        font-size: 24px;
    }

    .prep-time li {
        padding: 0 10px;
    }

    .ingredients,
    .instructions {
        padding: 0 20px
    }

    .ingredients li,
    .instructions li {
        padding: 0 10px;
    }
}
```

> 💡 [Here](https://github.com/amirmvahed/front-end-for-back-end-engineers-tasks/tree/main/recipe) you can see the source
> code 
