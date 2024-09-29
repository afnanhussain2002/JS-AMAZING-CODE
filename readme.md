
```markdown
# Utility Functions and Snippets

This project provides various utility JavaScript snippets for common tasks in web development, such as handling URLs, validating emails, detecting mobile browsers, and more. Below is a summary of the key functions and utilities included.

## Features

### 1. Operating System Detection
Logs the platform of the user's operating system.
```javascript
console.log(navigator.platform);
```

### 2. Prevent Page Refresh with `void(0)`
An anchor tag example to prevent page refresh when clicked.
```html
<a href="JavaScript:void(0);" onclick="alert('Well done!')">Click Me!</a>
```

### 3. Redirect to a New Page
Redirects the user to a new page.
```javascript
function redirect() {
    window.location.href = "newPage.html";
}
```

### 4. Get the Current URL
Retrieve the full URL of the current page.
```javascript
console.log("location.href", window.location.href);
console.log("document.URL", document.URL);
```

### 5. Email Validation
Validates an email address using a regular expression.
```javascript
function validateEmailUnicode(email) {
    var re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return re.test(String(email).toLowerCase());
}
```

### 6. Mobile Browser Detection (with Regex)
Detects whether the user is on a mobile browser.
```javascript
window.mobilecheck = function () {
    // Mobile check logic
};
```

### 7. Mobile Browser Detection (without Regex)
An alternative method to detect mobile browsers without using regex.
```javascript
function detectmob() {
    if (navigator.userAgent.match(/Android/i) || ...) {
        return true;
    }
    return false;
}
```

### 8. Detect Disabled JavaScript
Alerts the user when JavaScript is disabled.
```html
<noscript>
    <a href="next_page.html?noJS=true">JavaScript is disabled on the page. Enable it asap!</a>
</noscript>
```

### 9. Get Timezone Offset
Logs the user's timezone offset from UTC.
```javascript
var offset = new Date().getTimezoneOffset();
console.log(offset);
```

### 10. Change Cursor to Wait
Changes the cursor to a wait symbol while an operation is in progress.
```javascript
function myFunction() {
    window.document.body.style.cursor = "wait";
}
```

### 11. Get Checkbox Status
Checks whether a checkbox is selected.
```javascript
console.log(document.getElementById('checkboxname').checked);
```

### 12. Styled Console Messages
Logs messages to the console with custom styles.
```javascript
console.log("%cStyled Text", "color: purple; font-size: x-large; background: white");
```

### 13. Disable Right-Click on Page
Prevents the right-click context menu from appearing on the page.
```html
<body oncontextmenu="return false;"></body>
```

### 14. Capture Browser Back Button
Logs an event when the user clicks the browser's back button.
```javascript
window.addEventListener('beforeunload', () => {
    console.log('Clicked browser back button');
});
```

### 15. Group and Nest Console Output
Groups related console messages for better readability.
```javascript
console.group("User Details");
// nested console logs
console.groupEnd();
```

## Getting Started

To use these snippets, simply include the corresponding functions in your project or modify them as needed. These utilities are useful for enhancing user interaction, debugging, and handling web page behavior efficiently.

## License

This project is licensed under the MIT License.
```

This `README.md` provides a brief overview of the functionality included in your code and instructions for usage. Let me know if you'd like any changes!