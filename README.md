# 🐴 Hero Eliza: Jungle Adventure

An interactive educational game for young children that combines learning with fun adventure gameplay.

## 🎮 Game Overview

Hero Eliza is a browser-based game where a child becomes a hero riding a horse through the jungle, defeating enemies with correct answers to questions and collecting coins along the way.

## ✨ Features

- **Two Question Types:**
  - **Counting Questions**: Child sees emojis and counts them to select the correct number
  - **Reading Questions**: Parent reads a question aloud, child taps the correct emoji answer

- **Text-to-Speech**: All questions are spoken aloud in Spanish for interactive learning
- **Engaging Gameplay**: 
  - Hero gallops across the jungle defeating enemies
  - Collect coins for each correct answer
  - Defeat 7 enemies to win the game
  - Celebration animation with confetti on victory

- **Beautiful UI**:
  - Jungle themed background with trees
  - Adorable hero character on horseback
  - Animated enemies (lions and robots)
  - Carrot bucket reward at the finish line

## 🎯 How to Play

1. Open `jungle-adventure.html` in a web browser
2. Child sees the first question with emojis and answer options
3. For **counting questions**: Count the emojis displayed and tap the correct number
4. For **reading questions**: Listen to the parent read the question aloud, then tap the correct emoji answer
5. Correct answers = Hero gallops forward and defeats an enemy, earns a coin
6. Wrong answers = Hero shakes, try again
7. Defeat all 7 enemies and reach the carrot bucket to win!

## 🛠️ Customizing Questions

Edit the `ALL_QUESTIONS` array in `jungle-adventure.html` to add or modify questions:

### Counting Question Format:
```javascript
{ 
  type: "count", 
  emojis: "🐒🐒🐒",           // Emojis to count
  a: ["2", "3", "4"],          // Answer options
  ok: 1                         // Index of correct answer (0, 1, or 2)
}
```

### Reading Question Format:
```javascript
{ 
  type: "read", 
  text: "¿Cuál tiene trompa?",  // Question text (spoken aloud)
  a: ["🐒", "🐘", "🦜"],       // Emoji options
  ok: 1                         // Index of correct answer
}
```

## 📱 Device Compatibility

- Works on desktop and tablet browsers
- Requires JavaScript enabled
- Uses Web Speech API for text-to-speech (standard browsers)
- Responsive design adapts to different screen sizes

## 🌍 Language

Currently set to Spanish (`es-ES`). To change language settings, modify the `speakQuestion()` function:
- Change `utterance.lang = 'es-ES'` to your desired language code

## 🎨 Game Elements

- **Game Size**: 900px × 580px
- **World Area**: 63% (sky, jungle, road)
- **Question Panel**: 37% (questions and answer buttons)
- **Enemies**: 7 total (alternating lions and robots)
- **Questions per Game**: 7 (randomly selected from available questions)

## 💡 Tips

- Add more questions to the `ALL_QUESTIONS` array for variety
- Adjust speech rate/pitch in `speakQuestion()` for different preferences
- Modify emoji choices for different themes
- Customize colors in CSS for different jungle themes

## 🚀 Getting Started

1. Clone or download the repository
2. Open `jungle-adventure.html` in any modern web browser
3. Click "Jugar otra vez!" (Play Again!) to start a new game

Enjoy playing! 🎉
