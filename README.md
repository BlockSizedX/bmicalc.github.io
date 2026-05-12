# Simple BMI Calculator

This is a straightforward, no-nonsense BMI Calculator built using just the basics: HTML, CSS, and JavaScript. I avoided heavy frameworks and fancy libraries to keep the code clean, fast, and easy to understand for anyone looking to see how the math translates into a functional web tool.

### What it does

The application takes a user's height and weight and provides their Body Mass Index (BMI) along with a clear health classification. It is designed to be a quick reference point for weight-to-height proportions.

*   **Fast Calculations:** Results are generated instantly via client-side JavaScript.
*   **Health Categories:** The tool interprets the numerical result, categorizing it into Underweight, Normal, Overweight, or Obese based on standard health scales.
*   **Clean Interface:** The design is focused on utility. I kept the UI minimal to ensure that the user experience is intuitive and free of distractions.

### Why I built this

The goal was to create a tool that is actually useful for daily health tracking without the "bloat" found in modern health apps. On a technical level, this project served as a great exercise in:

*   **Logic Implementation:** Handling the mathematical formula and rounding data correctly.
*   **DOM Manipulation:** Learning how to capture user input and update the page content dynamically without a refresh.
*   **Responsive Design:** Ensuring the layout remains functional and readable on everything from a desktop monitor to a smartphone.

### How to use

1.  Download or clone the repository to your local machine.
2.  Open the `index.html` file in your preferred web browser.
3.  Enter your height in centimeters (cm).
4.  Enter your weight in kilograms (kg).
5.  Click the calculate button to see your result and health category.

### Technical Details

The calculator uses the standard metric formula: weight (kg) divided by height (m) squared. 

```javascript
// Example logic used in the app
const heightInMeters = height / 100;
const bmi = (weight / (heightInMeters * heightInMeters)).toFixed(2);
```

### Contributions

If you are interested in seeing how the math works or want to add your own styling, feel free to fork the repository. I am open to suggestions, whether it is adding support for imperial units (lbs/inches) or improving the CSS layout.

**Check out the repository here:** [https://github.com](https://github.com)

If you find a bug or have an idea for a new feature, feel free to open an issue or submit a pull request.



