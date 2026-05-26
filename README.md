# America First Studies Quiz

**Interactive civics and U.S. history assessment platform** with no question repetition across rounds.

[![Forest Green Theme](https://img.shields.io/badge/theme-Forest%20Green-166534)]()
[![Questions](https://img.shields.io/badge/questions-12%20%2B%20expandable-brightgreen)]()
[![Levels](https://img.shields.io/badge/levels-3%20difficulty%20tiers-blue)]()

## 🎯 Features

- **3 Difficulty Levels**: Beginner (5Q), Intermediate (8Q), Advanced (10Q)
- **No Question Repetition**: Questions marked as used, won't repeat until pool reset
- **Professional Forest Green Theme**: Consistent branding throughout
- **Instant Feedback**: Explanations for each question after submission
- **Score Tracking**: Real-time score display and performance analysis
- **Responsive Design**: Works seamlessly on mobile, tablet, and desktop
- **LocalStorage Persistence**: Your progress is saved automatically
- **Keyboard Support**: Press Enter to submit answers or move to next question
- **Question Pool Management**: View status and reset pool as needed

## 🚀 Quick Start

1. **Open the app**: Open `index.html` in any modern web browser
2. **Select a level**: Choose from Beginner, Intermediate, or Advanced
3. **Answer questions**: Select an option and click "Check Answer"
4. **View explanation**: Read the explanation before moving to the next question
5. **See results**: View your score and performance metrics at the end

## 📚 Question Bank

Currently includes **12 high-quality civics questions** covering:

- Declaration of Independence
- Bill of Rights & Constitutional Amendments
- Supreme Court Landmarks (Brown v. Board, etc.)
- Progressive Era history
- Founding principles and the Federalist Papers
- Presidential history and civic figures

**Expandable**: Add more questions by editing the `questions` array in the script.

## 🎮 How It Works

### Difficulty Levels

| Level | Questions | Focus |
|-------|-----------|-------|
| **1 - Beginner** | 5 | Foundational concepts, Constitution basics, key figures |
| **2 - Intermediate** | 8 | Amendments, Progressive Era, Supreme Court, Federalist principles |
| **3 - Advanced** | 10 | Constitutional structure analysis, civil rights, historical context |

### Question Tracking

- Each question is assigned a unique ID
- When you complete a round, those questions are marked as "used"
- Used questions won't appear in new rounds (avoiding repetition)
- **Reset Pool**: Click "Reset Question Pool" to clear all used questions and start fresh

## 💾 Data Storage

Your progress is saved in browser localStorage:
- `afs_usedQuestionIds`: Tracks which questions you've answered

Clearing browser data will reset this. To manually reset, use the "Reset Question Pool" button.

## 🎨 Theme Customization

The app uses a **Forest Green theme** (`#166534`) with supporting colors:

```css
--forest-green: #166534;      /* Primary brand color */
--forest-dark: #14532d;       /* Hover state */
--forest-light: #dcfce7;      /* Success state */
--green-100: #f0fdf4;         /* Light background */
```

Edit the CSS variables in `<style>` to customize colors.

## 🔧 Expanding the Question Bank

### Add a New Question

```javascript
{
    id: 13,  // Must be unique
    question: "Your question text here?",
    options: ["Option A", "Option B", "Option C", "Option D"],
    correctIndex: 0,  // 0-3, which option is correct
    explanation: "Detailed explanation of the correct answer.",
    difficulty: 2  // 1 for Level 1, 2 for Levels 2+
}
```

Add this object to the `questions` array in the `<script>` section.

## 📱 Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🏆 Performance Tiers

- **85%+**: Outstanding – Strong command of material
- **70-84%**: Solid – Continue reviewing for mastery
- **Below 70%**: Review explanations and try another round

## 📖 Educational Use

This platform is designed for:
- Civic education review
- History assessment
- Test preparation
- Self-paced learning

## 🔐 Privacy

No data is sent to external servers. All progress is stored locally in your browser.

## 📝 License

Built for educational use. Freely distributable for learning purposes.

---

**Built with**: HTML5, Tailwind CSS, Font Awesome, Vanilla JavaScript  
**Theme**: Forest Green (#166534)  
**All questions randomized with no repetition across rounds**
