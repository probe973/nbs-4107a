/* style.css - FINAL CLEANED AND CONSOLIDATED VERSION */

/* --- General Body and Typography Styles --- */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
    text-rendering: optimizeLegibility;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

h1, h2, h3, h4, h5, h6 {
    color: #2c3e50;
    margin-top: 1.5em;
    margin-bottom: 0.8em;
    line-height: 1.2;
}

/* --- Header and Footer Styles --- */
header {
    background-color: #34495e;
    color: #ffffff;
    padding: 1.5rem 0;
    text-align: center;
    box-shadow: 0 3px 6px rgba(0,0,0,0.15);
}

header h1 {
    color: #ffffff;
    margin: 0;
    font-size: 2.5em;
}

header p {
    color: #e0e0e0;
    margin: 0.5em 0 0;
    font-size: 1.1em;
}

footer {
    text-align: center;
    padding: 25px;
    margin-top: 40px;
    background-color: #34495e;
    color: #e0e0e0;
    font-size: 0.9em;
    box-shadow: 0 -3px 6px rgba(0,0,0,0.1);
}

footer a {
    color: #5dade2;
    text-decoration: none;
}

footer a:hover,
footer a:focus {
    text-decoration: underline;
    color: #85c1e9;
}

/* --- Navigation Bar Styles --- */
nav {
    background-color: #2c3e50;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    padding: 0.5rem 0;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

nav ul li a {
    display: block;
    color: #ecf0f1;
    text-align: center;
    padding: 12px 20px;
    text-decoration: none;
    transition: background-color 0.3s ease, color 0.3s ease;
    font-size: 1.0em;
    font-weight: 500;
}

nav ul li a:hover,
nav ul li a:focus {
    background-color: #3498db;
    color: #ffffff;
    outline: none;
}

nav ul li a.active {
    background-color: #3498db;
    color: #ffffff;
    font-weight: bold;
    cursor: default;
}

/* --- Main Content and Layout Styles --- */
main {
    max-width: 960px;
    margin: 25px auto;
    padding: 25px 30px;
    background-color: #ffffff;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    border-radius: 8px;
    line-height: 1.7;
}

/* --- Colored Section Box Styles --- */
.explanation, .instructions, .output {
    padding: 1.8em;
    border-radius: 7px;
    margin-bottom: 20px;
}

.explanation {
    background-color: #fff8e1;
    color: #5d4037;
}

.instructions {
    background-color: #e3f2fd;
    color: #1976d2;
}

.output {
    background-color: #e8f5e9;
    color: #2e7d32;
    font-family: 'Courier New', Courier, monospace;
    white-space: pre-wrap;
    word-wrap: break-word;
}

/* Fix for large gap above titles in colored boxes */
.explanation h1:first-child, .instructions h1:first-child, .output h1:first-child,
.explanation h2:first-child, .instructions h2:first-child, .output h2:first-child {
    margin-top: 0;
}

/* --- Code Snippet Styles --- */
code {
    background-color: #f0f0f0;
    padding: 0.2em 0.4em;
    border-radius: 3px;
    font-family: 'Courier New', Courier, monospace;
    color: #c7254e;
    word-wrap: break-word;
}

pre {
    background-color: #f8f8f8;
    padding: 1.2em;
    border-radius: 5px;
    overflow-x: auto;
    border: 1px solid #e0e0e0;
}

/* --- General Element Styles (Images, Accessibility) --- */
img {
    max-width: 100%;
    height: auto;
    display: block;
    margin: 1.5em auto;
    border: 1px solid #ddd;
    border-radius: 4px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}

a:focus:not(.btn), button:focus:not(.btn), input:focus, select:focus, textarea:focus {
    outline: 3px solid #f39c12;
    outline-offset: 2px;
}

.MathJax_Display {
    overflow-x: auto;
    margin: 1em 0;
}

/* --- Topic Card Menu Styles --- */
.card-menu {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 25px;
    margin-top: 3em;
}

.card {
    background-color: #ffffff;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 25px;
    text-decoration: none;
    color: #333;
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    border-color: #3498db;
}

.card-content {
    display: flex;
    align-items: center;
    gap: 20px;
}

.card-icon {
    flex-shrink: 0;
}

.card-icon svg {
    width: 48px;
    height: 48px;
    stroke: #34495e;
}

.card-text h3 {
    margin: 0 0 5px 0;
    font-size: 1.3em;
    color: #2c3e50;
}

.card-text p {
    margin: 0;
    font-size: 0.95em;
    color: #666;
    line-height: 1.5;
}

/* --- Interactive Question Styles --- */
.question-container {
    background-color: #f5f7f9;
    border-left: 5px solid #607d8b;
    padding: 1.8em 2em;
    margin-top: 2.5em;
    margin-bottom: 2.5em;
    border-radius: 0 8px 8px 0;
}

.question-container h3 {
    margin-top: 0;
}

.btn {
    display: inline-block;
    background-color: #28a745;
    color: white;
    padding: 12px 24px;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    font-size: 1.05em;
    font-weight: 600;
    letter-spacing: 0.5px;
    margin-top: 15px;
    transition: background-color 0.2s ease, transform 0.2s ease, box-shadow 0.2s ease;
    text-decoration: none;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.btn:hover {
    background-color: #218838;
    transform: translateY(-2px);
    box-shadow: 0 5px 10px rgba(0,0,0,0.15);
}

.btn-primary {
    background-color: #007bff;
}

.btn-primary:hover {
    background-color: #0056b3;
}

.mcq-options {
    margin-top: 1.5em;
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.mcq-options label {
    display: block;
    background-color: #ffffff;
    padding: 15px;
    border: 1px solid #ddd;
    border-radius: 6px;
    cursor: pointer;
    transition: border-color 0.2s ease, box-shadow 0.2s ease;
}

.mcq-options label:hover {
    border-color: #3498db;
    box-shadow: 0 2px 5px rgba(0,0,0,0.08);
}

.mcq-options input[type="radio"] {
    margin-right: 12px;
    transform: scale(1.2);
}

.numerical-answer-container {
    margin-top: 1.5em;
    display: flex;
    align-items: center;
    gap: 15px;
    flex-wrap: wrap;
}

input[type="number"] {
    max-width: 200px;
    font-size: 1.1em;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

.feedback {
    margin-top: 1em;
    padding: 10px 15px;
    border-radius: 5px;
    font-weight: bold;
}

.feedback-correct {
    background-color: #e8f5e9;
    color: #2e7d32;
    border: 1px solid #c8e6c9;
}

.feedback-incorrect {
    background-color: #fbe9e7;
    color: #c62828;
    border: 1px solid #ffccbc;
}

.solution-toggle-button {
    margin-top: 1.5em;
}

.solution-content {
    background-color: #fff8e1;
    border: 1px solid #ffecb3;
    padding: 1.5em;
    margin-top: 1em;
    border-radius: 7px;
    display: none;
    line-height: 1.6;
}

.solution-content.visible {
    display: block;
}
