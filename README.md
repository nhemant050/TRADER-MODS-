# TRADER-MODS-

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Hacker Theme Login</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Share+Tech+Mono&display=swap');

  /* Background with falling code effect */
  body {
    margin: 0;
    height: 100vh;
    background: black;
    overflow: hidden;
    font-family: 'Share Tech Mono', monospace;
    color: #00ff00;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  /* Falling code lines */
  .code-rain {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 0;
  }

  .code-rain span {
    position: absolute;
    top: -100px;
    color: #00ff00;
    font-size: 14px;
    user-select: none;
    animation-name: fall;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
  }

  @keyframes fall {
    0% {
      top: -100px;
      opacity: 1;
    }
    100% {
      top: 110vh;
      opacity: 0;
    }
  }

  /* Login container */
  .login-container {
    position: relative;
    background: rgba(0, 0, 0, 0.85);
    border: 2px solid #00ff00;
    padding: 40px 50px;
    border-radius: 12px;
    box-shadow: 0 0 20px #00ff00;
    width: 320px;
    z-index: 1;
  }

  .login-container h1 {
    text-align: center;
    margin-bottom: 30px;
    font-weight: 700;
    font-size: 2rem;
    letter-spacing: 3px;
    text-shadow: 0 0 8px #00ff00;
  }

  label {
    display: block;
    margin-bottom: 8px;
    font-size: 0.9rem;
    letter-spacing: 1.5px;
  }

  input[type="text"],
  input[type="password"] {
    width: 100%;
    padding: 12px 15px;
    margin-bottom: 25px;
    background: black;
    border: 1.5px solid #00ff00;
    border-radius: 6px;
    color: #00ff00;
    font-size: 1rem;
    font-family: 'Share Tech Mono', monospace;
    outline: none;
    transition: box-shadow 0.3s ease;
  }

  input[type="text"]:focus,
  input[type="password"]:focus {
    box-shadow: 0 0 10px #00ff00;
    border-color: #00ff00;
  }

  /* Login button with key icon */
  .login-btn {
    position: relative;
    width: 100%;
    padding: 14px 0;
    background: transparent;
    border: 2px solid #00ff00;
    border-radius: 8px;
    color: #00ff00;
    font-size: 1.1rem;
    font-weight: 700;
    cursor: pointer;
    font-family: 'Share Tech Mono', monospace;
    overflow: hidden;
    transition: background 0.3s ease, color 0.3s ease;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
  }

  .login-btn:hover {
    background: #00ff00;
    color: black;
    box-shadow: 0 0 15px #00ff00;
  }

  /* Key icon */
  .key-icon {
    width: 20px;
    height: 20px;
    stroke: currentColor;
    stroke-width: 2;
    fill: none;
    animation: pulse 2s infinite;
    transition: transform 0.3s ease;
  }

  .login-btn:hover .key-icon {
    animation: pulse-fast 0.6s infinite;
    transform: scale(1.2);
  }

  @keyframes pulse {
    0%, 100% {
      stroke-opacity: 1;
      filter: drop-shadow(0 0 3px #00ff00);
    }
    50% {
      stroke-opacity: 0.5;
      filter: drop-shadow(0 0 10px #00ff00);
    }
  }

  @keyframes pulse-fast {
    0%, 100% {
      stroke-opacity: 1;
      filter: drop-shadow(0 0 6px #00ff00);
    }
    50% {
      stroke-opacity: 0.3;
      filter: drop-shadow(0 0 20px #00ff00);
    }
  }
</style>
</head>
<body>

<div class="code-rain" aria-hidden="true"></div>

<div class="login-container" role="main" aria-label="Login form">
  <h1>ACCESS</h1>
  <form id="loginForm" autocomplete="off">
    <label for="username">8234022</label>
    <input type="text" id="username" name="username" required autocomplete="username" spellcheck="false" />
    <label for="password">8234022</label>

<input type="password" id="password" name="password" required autocomplete="current-password" />
    <button type="submit" class="login-btn" aria-label="Login">
      <svg class="key-icon" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
        <circle cx="7" cy="12" r="3"></circle>
        <path d="M10 12h7v2h-3v2h-2v-2h-2v-2z"></path>
      </svg>
      LOGIN
    </button>
  </form>
</div>

<script>
  // Generate falling code rain effect
  const codeRain = document.querySelector('.code-rain');
  const letters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*()';

  function createCodeSpan() {
    const span = document.createElement('span');
    span.textContent = letters.charAt(Math.floor(Math.random() * letters.length));
    span.style.left = Math.random() * 100 + 'vw';
    span.style.animationDuration = (5 + Math.random() * 10) + 's';
    span.style.fontSize = (12 + Math.random() * 14) + 'px';
    span.style.opacity = Math.random();
    return span;
  }

  for (let i = 0; i < 150; i++) {
    codeRain.appendChild(createCodeSpan());
  }

  // Simple login form demo
  const form = document.getElementById('loginForm');
  form.addEventListener('submit', e => {
    e.preventDefault();
    alert(Welcome, ${form.username.value}!);
  });
</script>

</body>
</html>
