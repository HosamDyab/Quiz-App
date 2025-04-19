# 🚀 Internet Technology Quiz

<div align="center">

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-100%25-brightgreen?style=for-the-badge)
![Accessibility](https://img.shields.io/badge/Accessibility-WCAG_2.1-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)


</div>

A modern, interactive Internet Technology quiz application with a beautiful neomorphic UI design. Features multiple question types, theme switching, detailed review section, and a sleek animation system. Built with pure frontend technologies for outstanding performance.



## ✨ Key Features

<div align="center">
<table>
  <tr>
    <td align="center" width="33%">
      <img src="https://cdn-icons-png.flaticon.com/512/3500/3500833.png" width="48" height="48" alt="Multiple Question Types"/><br/>
      <b>Multiple Question Types</b>
    </td>
    <td align="center" width="33%">
      <img src="https://cdn-icons-png.flaticon.com/512/2972/2972531.png" width="48" height="48" alt="Interactive"/><br/>
      <b>Neomorphic UI</b>
    </td>
    <td align="center" width="33%">
      <img src="https://cdn-icons-png.flaticon.com/512/1243/1243560.png" width="48" height="48" alt="Timer"/><br/>
      <b>Quiz Timer</b>
    </td>
  </tr>
  <tr>
    <td align="center" width="33%">
      <img src="https://cdn-icons-png.flaticon.com/512/6357/6357050.png" width="48" height="48" alt="Dark Mode"/><br/>
      <b>Dark/Light Themes</b>
    </td>
    <td align="center" width="33%">
      <img src="https://cdn-icons-png.flaticon.com/512/5352/5352645.png" width="48" height="48" alt="Analytics"/><br/>
      <b>Detailed Review</b>
    </td>
    <td align="center" width="33%">
      <img src="https://cdn-icons-png.flaticon.com/512/747/747086.png" width="48" height="48" alt="Animation"/><br/>
      <b>Rich Animations</b>
    </td>
  </tr>
</table>
</div>


## 📱 Responsive Design

The application is fully responsive and works beautifully on all devices:

- **Desktop**: Full-featured experience with optimized layouts
- **Tablet**: Adjusted UI for comfortable touch interaction
- **Mobile**: Streamlined interface for on-the-go learning

## 🎮 Quiz Features

- **20 Internet Technology Questions**: Covering HTTP, DNS, networking, web development and more
- **Multiple Question Types**: MCQ, True/False, and Text Input questions
- **15-Minute Timer**: Challenge yourself to complete all questions in time
- **Score Tracking**: See how well you performed
- **Detailed Review**: Compare your answers with correct ones, with explanations
- **Navigation**: Go back to previous questions to change answers
- **Visual Feedback**: Clear color-coding (green for correct, red for incorrect)

## 🎨 UI/UX Highlights

### Neomorphic Design System
- Soft, realistic shadows that create a 3D effect
- Custom elevation system for interactive elements
- Consistent design language throughout the application

### Color Themes
- **Light theme**: Clean, bright interface for daytime use
- **Dark theme**: Eye-friendly dark mode for night time
- **System preference detection**: Automatically matches your device settings

### Animation System
- Smooth transitions between quiz states
- Micro-interactions for enhanced feedback
- Performance-optimized animations using CSS techniques

## 💻 Technical Implementation

### Vanilla JavaScript Architecture
```javascript
/**
 * Shows the review screen with a list of questions and user's answers
 * Visually indicates if answers are correct or incorrect
 */
function showReviewScreen() {
    // Create review item for each question
    questions.forEach((question, index) => {
        // Get user's answer
        const userAnswerText = getUserAnswerText(question);
        
        // Create visual feedback based on correctness
        const userAnswerObj = userAnswers[index];
        if (userAnswerObj && userAnswerObj.correct) {
            userAnswer.classList.add('correct'); // Green styling
        } else if (userAnswerText !== "Not answered") {
            userAnswer.classList.add('wrong'); // Red styling
        }
        
        // Display correct answer for comparison
        const correctAnswer = document.createElement('div');
        correctAnswer.classList.add('review-answer', 'correct-answer');
        correctAnswer.textContent = getCorrectAnswerText(question);
    });
}
```

### CSS Variables & Design Tokens
```css
:root {
    /* Color Palette */
    --primary: #7000FF;
    --primary-dark: #5B00CC;
    --primary-light: #9B4DFF;
    --primary-rgb: 112, 0, 255;
    --secondary: #FF2D55;
    --accent: #00F7FF;
    --accent-secondary: #0096FF;
    
    /* Neomorphic Shadow System */
    --soft-shadow-light: rgba(166, 177, 199, 0.5);
    --hard-shadow-light: rgba(255, 255, 255, 0.8);
    --soft-shadow-dark: rgba(0, 0, 0, 0.3);
    --hard-shadow-dark: rgba(40, 45, 60, 0.5);
    
    /* Dynamic Theme Variables */
    --background: var(--bg-light);
    --text: var(--text-light);
    --shadow-soft: var(--soft-shadow-light);
    --shadow-hard: var(--hard-shadow-light);
}
```

## ⚡ Performance Optimizations

- **Efficient DOM Manipulation**: Minimized reflows and repaints
- **Event Delegation**: Optimized event handling
- **CSS Animation**: Hardware-accelerated animations with transforms
- **Lazy Initialization**: Components load only when needed
- **Debounced Events**: Prevents performance bottlenecks during interaction

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/HosamDyab/Quiz-App.git

# Navigate to the project
cd Quiz-App

# No build tools or dependencies required!
# Simply open index.html in your browser
```

### Running Locally
1. Double-click on `index.html` or open it with your browser
2. No server needed - works directly from the filesystem
3. No external dependencies - everything included!

## 📁 Project Structure

```
Quiz-App/
├── index.html          # Main entry point
├── script.js           # Quiz application logic
├── styles.css          # Styling and animations
├── README.md           # Documentation
```

## 🧪 Browser Compatibility

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)
- ✅ Mobile browsers

## 🛠️ Future Enhancements

- [ ] User accounts and progress tracking
- [ ] Additional question categories
- [ ] Difficulty level settings
- [ ] Offline support with PWA implementation
- [ ] Multi-language support
- [ ] Social sharing of results

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👏 Acknowledgements

- [Font Awesome](https://fontawesome.com/) for the icons
- [Google Fonts](https://fonts.google.com/) for typography
- All contributors and reviewers

---

<div align="center">
Made with ❤️ by <a href="https://github.com/HosamDyab">Hosam Dyab</a>
<br><br>
<a href="https://github.com/HosamDyab"><img src="https://img.shields.io/github/followers/HosamDyab?label=Follow&style=social" alt="GitHub"></a>
</div>
