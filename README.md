<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Project</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@700;800;900&display=swap');

body {
  background: radial-gradient(circle at 20% 20%, #0d1117 0%, #000 100%);
  color: white;
  font-family: 'Inter', sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  overflow: hidden;
}

h1 {
  font-size: 4rem;
  font-weight: 900;
  letter-spacing: -2px;
  text-transform: uppercase;
  background: linear-gradient(90deg, #00eaff, #007bff, #5e00ff, #00eaff);
  background-size: 300% 300%;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: gradientShift 6s ease-in-out infinite, fadeIn 2s ease-out forwards;
  position: relative;
  user-select: none;
}

h1::after {
  content: '';
  position: absolute;
  top: 0;
  left: -10%;
  width: 120%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
  transform: skewX(-20deg);
  animation: shimmer 4s infinite linear;
}

.badges {
  display: flex;
  gap: 0.5rem;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 1rem;
  opacity: 0;
  animation: fadeInUp 1.5s ease-out 0.8s forwards;
}

.badges a img, .badges img {
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 255, 255, 0.3);
  transition: all 0.3s ease;
  animation: floatBadge 4s ease-in-out infinite;
}

.badges img:hover {
  transform: scale(1.1) rotate(1deg);
  box-shadow: 0 0 20px rgba(0, 255, 255, 0.7);
  filter: brightness(1.3);
}

@keyframes gradientShift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

@keyframes shimmer {
  0% { left: -20%; }
  100% { left: 120%; }
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(30px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes floatBadge {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-6px); }
}

.glow {
  position: absolute;
  width: 300px;
  height: 300px;
  background: radial-gradient(circle, rgba(0,255,255,0.3) 0%, transparent 70%);
  filter: blur(100px);
  animation: moveGlow 10s ease-in-out infinite alternate;
}

@keyframes moveGlow {
  0% { transform: translate(-150px, -100px); }
  100% { transform: translate(150px, 100px); }
}
</style>
</head>
<body>

<div class="glow"></div>

<h1>PROJECT</h1>

<div class="badges">
  <img src="https://img.shields.io/badge/build-passing-00e676?style=for-the-badge&labelColor=1c1c1c&logo=github&logoColor=white" alt="Build Status"/>
  <img src="https://img.shields.io/badge/lang-C++-00599C?style=for-the-badge&labelColor=1c1c1c&logo=c%2B%2B&logoColor=white" alt="Language"/>
  <img src="https://img.shields.io/badge/game-TF2-f39c12?style=for-the-badge&labelColor=1c1c1c&logo=steam&logoColor=white" alt="Game"/>
  <a href="https://www.unknowncheats.me/forum/team-fortress-2-a/436430-seowned-featured-cheat.html" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/origin-SEOwned-0078ff?style=for-the-badge&labelColor=1c1c1c&logo=github&logoColor=white" alt="Origin"/>
  </a>
</div>

</body>
</html>
