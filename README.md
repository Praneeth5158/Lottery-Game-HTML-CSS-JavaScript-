# Lottery-Game-HTML-CSS-JavaScript-

📌 Overview
The Lottery Game is a fun and interactive web-based mini-game built using HTML, CSS, and JavaScript.
When the user clicks the Pick a Number button, the game:

Highlights random lottery boxes for animation

Plays a ticking sound

Finally selects a winning box

Displays the prize associated with that number

Plays a winning sound

All 50 lottery boxes are generated dynamically using JavaScript, making the project clean and scalable.

🚀 Features
🎲 Random number selection

🎁 50 unique gifts

🔊 Sound effects (tap + win)

✨ Animated box highlighting

🎨 Responsive and clean UI

⚡ Fully dynamic DOM creation

🛠️ Technologies Used
HTML5 – Structure

CSS3 – Styling & layout

JavaScript – Game logic, DOM manipulation, randomization

🎵 Audio files (tap.wav, win.wav)

📂 Project Structure
/Lottery-Game
│── index.html
│── styles.css
│── script.js
│── tap.wav
│── win.wav
📘 How It Works
✔️ Box Creation
All 50 boxes are generated dynamically using this code:

gifts.forEach(function(value,i){
    let boxelement = `<div class="Box" id=${i+1}>${i+1}. ${value}<div>`;
    lotterySheetContainer.insertAdjacentHTML("beforeend", boxelement);
});
✔️ Random Highlight Animation
setInterval() highlights a new random box every second:

const randomBox = Math.floor(Math.random()*50)+1;
✔️ Final Winner Selection
After 5 cycles:

let floornum = Math.floor((Math.random()*50)+1);
✔️ Sound Effects
tick.play();
win.play();
▶️ How to Run
Download all project files

Keep them in the same folder (HTML, CSS, JS, WAV files)

Open index.html in any web browser

Click Pick a Number

Enjoy the animation and your surprise gift! 🎁

🎯 Future Improvements
Add difficulty levels

Add animation speed controls

Make the UI mobile-friendly

Store last won gift using localStorage

📜 License
This project is free to use for learning and personal projects.

