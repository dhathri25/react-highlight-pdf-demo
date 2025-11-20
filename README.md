# Maersk Report Highlighter – ReactJS Assignment
This project is a ReactJS web application created for the assignment where the task is to display a PDF on one side of the screen and the analysis text on the other side. The main objective of the assignment is that when the user clicks on reference number [3] in the analysis text, a specific sentence inside the PDF should get highlighted in yellow. The sentence is: “Gain on sale of non-current assets, etc”.

The idea behind the project is to show how interaction on one part of the UI can affect content in another part—in this case, clicking a reference and automatically jumping to or highlighting a line in a PDF. Since PDFs are not straightforward to edit or highlight directly, I used a React-based PDF viewer to simulate the highlight when the reference is clicked.

## 🚀 Features

- 📄 **PDF Viewer** using `react-pdf`
- ✨ **Highlight specific text** inside the PDF on click
- 📝 Right-side analysis panel with clickable references
- 🔗 Smooth communication between components
- 🎯 Meets the assignment requirement:
  - On clicking **[3]**, highlight the line *"Gain on sale of non-current assets, etc"* in the PDF.

---

The screen layout is simple and clear. On the left side, the PDF file is shown using a PDF viewer component. On the right side, the analysis text is displayed. The analysis text contains three references ([1], [2], [3]), and when the user clicks on [3], I trigger a function that sends a highlight signal to the PDF viewer. The viewer then finds the matching text inside the PDF and highlights it in yellow. This completes the main functionality required in the assignment.

To run this project on your system:
1. First install all dependencies by running: npm install
2. Then start the application using: npm start
3. The project will run on http://localhost:3000 by default.

If you want to replace the PDF with the real Maersk Q2 2025 Interim Report, you can simply put the PDF file inside the public folder and rename it to sample.pdf. The application will automatically load whatever PDF file is placed with that name.

The project is built using ReactJS because that was the requirement mentioned. It uses functional components and hooks to manage the highlight state. The PDF rendering is done with the react-pdf library, which allows the PDF to be shown inside the browser. When the highlight trigger is activated, the viewer searches for the phrase inside the rendered text layer and highlights it visually.

For deployment, you can upload this React project to GitHub and then deploy it using Vercel. Vercel automatically detects React projects and sets everything up for you. After deployment, you will get a live link that you can submit in the Excel sheet as required.

Overall, this project demonstrates the required behavior: 
- Left side shows the PDF
- Right side shows the analysis text
- Clicking reference [3] triggers the highlight
- The correct sentence inside the PDF gets highlighted
- The project is built fully in ReactJS as instructed.

This completes the assignment successfully.

