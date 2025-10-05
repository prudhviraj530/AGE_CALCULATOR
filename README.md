# AGE_CALCULATOR

Here is a **step-by-step guide** explaining how you created your **Age Calculator** project. This can help others (or yourself later) understand how you built it and how they could recreate it too:

---

## ✅ Project Title:

**Age Calculator using HTML, CSS, and JavaScript**

---

## 🔧 Tools Used:

* **HTML** – For structuring the web page
* **CSS** – For styling the page to make it look nice
* **JavaScript** – For calculating the age dynamically

---

## 🧭 Step-by-Step Process:

### 1. **Create the Basic HTML Structure**

Start with a simple HTML template:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  ...
</head>
<body>
  ...
</body>
</html>
```

* `<!DOCTYPE html>` tells the browser that this is an HTML5 document.
* The `<html>` element wraps everything on the page.
* Inside the `<head>`, you include metadata and a `<title>` for the page.
* The `<body>` holds all visible content on the screen.

---

### 2. **Design the Layout in the `<body>`**

Inside the `<body>`, you created a container that includes:

* A **title** (`<h2>`)
* A **label and input field** for selecting date of birth (`<input type="date">`)
* A **button** to trigger the age calculation
* A **div** to display the result

```html
<div class="container">
  <h2>Age Calculator</h2>
  <label for="dob">Enter your Date of Birth:</label>
  <input type="date" id="dob">
  <button onclick="calculateAge()">Calculate Age</button>
  <div class="result" id="result"></div>
</div>
```

---

### 3. **Add Styling with CSS**

Inside the `<style>` tag in the `<head>`, you added custom CSS to:

* Center the content using **Flexbox**
* Style the container, buttons, inputs, and results
* Add colors and spacing for better visual appearance

Example:

```css
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
.container {
  background: #fff;
  padding: 30px;
  border-radius: 12px;
}
```

This makes your UI look clean and modern.

---

### 4. **Add JavaScript to Calculate the Age**

At the bottom of the HTML, you added a `<script>` tag containing the logic:

```javascript
function calculateAge() {
  let dob = document.getElementById("dob").value;
  ...
}
```

### 🔍 How the Calculation Works:

1. Get the selected date of birth.
2. Create a `Date` object from the input.
3. Get today’s date using `new Date()`.
4. Subtract birth year from current year.
5. Adjust **months** and **days** if the birthday hasn’t happened yet this year.
6. Display the result using `innerHTML`.

You also added:

* A **warning message** if the date is not selected.
* **Color styling** to the result (green for years, blue for months, red for days).

---

### 5. **Test the Project**

After writing the code:

* Open the HTML file in a web browser.
* Try selecting different birth dates.
* Check if the age is calculated correctly.
* Test for edge cases (e.g., today’s date, leap years, etc.)

---

## ✅ Final Output:

* A beautiful form where users enter their birth date.
* One click shows their **age in years, months, and days**.

---


