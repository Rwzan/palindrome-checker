
# Palindrome Checker 🔄

A simple, clean, and interactive web application built with HTML, CSS, and vanilla JavaScript that checks whether a given word or phrase is a palindrome (reads the same backward as forward).

## 🚀 Features

*   **Real-time Validation:** Instantly checks if the input text is a palindrome upon clicking the button.
*   **Case & Space Insensitive:** Automatically handles uppercase letters and spaces (e.g., "Nurses run" will correctly be identified as a palindrome).
*   **Dynamic UI Updates:** Displays a clear feedback message showing the original text and its reversed version.
*   **Clean Design:** Centered layout with a modern color palette (Burgundy & Gold).

## 🛠️ Technologies Used

*   **HTML5:** For the structure and semantic markup.
*   **CSS3:** For styling, layout centering, and responsiveness.
*   **JavaScript (ES6):** For the logical check and DOM manipulation.

## 📁 Project Structure

The entire project is self-contained within a single file for simplicity:
*   `index.html` - Contains the UI layout, styling rules, and JavaScript logic.

## 💻 How to Run the Project

1. **Clone the repository:**
```bash
   git clone [https://github.com/Rwzan/palindrome-checker.git](https://github.com/Rwzan/palindrome-checker.git)

```

2. **Navigate to the project folder:**

```bash
   cd palindrome-checker

```

3. **Open the file:**
Simply double-click the `index.html` file to open it in any modern web browser.

## 🧠 How It Works (Code Overview)

The core logic cleans the user input by converting it to lowercase and removing spaces using Regular Expressions (RegEx). It then compares the cleaned string with its reversed version:

```javascript
function checkPilandrome(myText) {
  let cleaned = myText.toLowerCase().replace(/\s/g, "");
  let reversed = cleaned.split('').reverse().join("");
  return { isPalindrome: cleaned === reversed, reversed: reversed };
}

```

## 📝 License

This project is open-source.
