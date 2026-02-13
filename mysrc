const yesBtn = document.getElementById("yesBtn");
const noBtn = document.getElementById("noBtn");
const card = document.getElementById("card");
const music = document.getElementById("bgMusic");

// No button politely escapes 😌
noBtn.addEventListener("mouseover", () => {
  const x = Math.random() * 180 - 90;
  const y = Math.random() * 180 - 90;
  noBtn.style.transform = `translate(${x}px, ${y}px)`;
});

// Floating hearts
function createHeart() {
  const heart = document.createElement("div");
  heart.className = "heart";
  heart.innerHTML = "💗";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.fontSize = Math.random() * 10 + 16 + "px";
  document.body.appendChild(heart);

  setTimeout(() => heart.remove(), 7000);
}

// Sparkle effect
function createSparkle() {
  const sparkle = document.createElement("div");
  sparkle.className = "sparkle";
  sparkle.innerHTML = "✨";
  sparkle.style.left = Math.random() * 100 + "vw";
  sparkle.style.top = Math.random() * 100 + "vh";
  document.body.appendChild(sparkle);

  setTimeout(() => sparkle.remove(), 3000);
}

// YES click
yesBtn.addEventListener("click", () => {
  music.volume = 0.4; // gentle volume
  music.play();

  setInterval(createHeart, 400);
  setInterval(createSparkle, 800);

  card.innerHTML = `
    <h2>🌸💖</h2>
    <h3>Yay! You said YES 💕</h3>
    <p>
      My dearest Taimoor,<br><br>
      From your wife — with pure love.<br><br>
      You are my comfort, my calm,
      and my forever Valentine.<br><br>
      Loving you is easy,
      choosing you is natural,
      staying with you is home.<br><br>
      <strong>I love you endlessly 💗</strong>
    </p>
  `;
});
