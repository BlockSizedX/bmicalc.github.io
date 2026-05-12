# Simple BMI Calculator

### Project Overview
This project is a streamlined, high-performance Body Mass Index (BMI) Calculator. It was developed to provide a lightweight alternative to resource-heavy health applications. By utilizing vanilla HTML5, CSS3, and modern JavaScript, the application ensures maximum compatibility across all web browsers while maintaining a minimal footprint.

The core objective was to demonstrate that essential utility tools do not require complex frameworks like React or Vue to be effective, accessible, and responsive.

### Functional Features
The application is designed with a focus on precision and user feedback.

*   **Real-Time Data Processing:** The JavaScript engine calculates the BMI immediately upon user input, providing a seamless experience without page reloads.
*   **Dynamic Health Classification:** The tool does more than provide a raw number. It compares the result against the World Health Organization (WHO) standards to categorize the user into Underweight, Normal Weight, Overweight, or Obese classes.
*   **Accessibility and UI Design:** The interface was built with a mobile-first approach. The layout adapts to various screen sizes, ensuring that the input fields and result displays remain legible on small mobile devices and large desktop monitors alike.

### Technical Implementation and Learning Objectives
Building this tool allowed for a deep dive into several fundamental web development concepts:

*   **Mathematical Logic in Programming:** Implementing the BMI formula required careful handling of data types to ensure that string inputs from the DOM are correctly converted to floating-point numbers for calculation.
*   **Event Handling:** The application uses event listeners to trigger calculations, demonstrating an understanding of how to capture user actions efficiently.
*   **CSS Architecture:** I utilized a combination of Flexbox and CSS variables to create a theme that is easy to modify and maintain. The styling ensures that the visual hierarchy directs the user's attention to the result area.

### Project Structure and Installation
The repository is organized into a flat structure for simplicity:
*   `index.html`: Contains the semantic structure and the input forms.
*   `style.css`: Contains all layout rules and responsive media queries.
*   `script.js`: Contains the calculation logic and DOM manipulation code.

To run this project locally:
1.  Clone the repository using `git clone https://github.com`.
2.  Navigate to the project directory.
3.  Open `index.html` in your browser. No local server or build step is required.

### Detailed Calculation Logic
The script converts the height from centimeters to meters before applying the standard formula. The result is then rounded to two decimal places to ensure a clean presentation.

```javascript
// Internal calculation logic
function calculateBMI(weight, height) {
    const heightInMeters = height / 100;
    const result = weight / (heightInMeters * heightInMeters);
    return result.toFixed(2);
}
```

### Future Roadmap
While the current version is fully functional, I plan to implement the following features in upcoming updates:
*   **Unit Toggle:** A switch to allow users to choose between Metric (kg/cm) and Imperial (lbs/inches) systems.
*   **Local Storage:** An optional feature to save previous results locally so users can track their progress over time.
*   **Data Visualization:** A simple visual scale or gauge to show where the user's BMI falls within the health categories.

### Troubleshooting
If the calculator does not appear to be working, ensure that:
1.  JavaScript is enabled in your browser settings.
2.  Both height and weight fields contain positive numerical values.
3.  You are using a modern browser (Chrome, Firefox, Safari, or Edge).

### Contribution and License
Feedback is highly encouraged. If you have suggestions for improving the code efficiency or the user interface, please feel free to fork this repository and submit a pull request. 

For major changes, please open an issue first to discuss what you would like to change.

**Repository Link:** [https://github.com](https://github.com)

---
*Disclaimer: This tool is intended for educational and general informational purposes. BMI is a general indicator and does not account for muscle mass, bone density, or overall body composition. Consult a healthcare provider for a comprehensive health assessment.*
