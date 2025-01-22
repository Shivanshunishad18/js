// script.js

// Function to display an alert when the paragraph is clicked
function handleParagraphClick() {
  alert("You clicked on the paragraph!");
}

// Function to change the color of the text inside the paragraph
function changeTextColor() {
  const paragraph = document.querySelector("p");
  paragraph.style.color = "#28a745"; // Green color
}

// Adding event listeners after the DOM is fully loaded
document.addEventListener("DOMContentLoaded", () => {
  // Select the paragraph
  const paragraph = document.querySelector("p");

  // Add a click event to the paragraph
  paragraph.addEventListener("click", handleParagraphClick);

  // Change the text color after 2 seconds
  setTimeout(changeTextColor, 2000);
});
