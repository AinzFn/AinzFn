<div align="center">
  <div class="wave-container">
    <h1 class="poem-text">
      蒲公英，随风飘，何时方知归何处？<br>
      终结时，沙漠中，恋此花者一人足。<br>
      于是此生无憾。
    </h1>
  </div>
</div>

<style>
.wave-container {
  position: relative;
  background: linear-gradient(45deg, #00ff87, #60efff, #00ff87, #60efff);
  background-size: 400% 400%;
  animation: gradient-wave 4s ease infinite, fadeIn 2s;
  padding: 40px 20px;
  border-radius: 15px;
  overflow: hidden;
}

.wave-container::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: repeating-linear-gradient(
    60deg,
    transparent,
    transparent 10px,
    rgba(255, 255, 255, 0.1) 10px,
    rgba(255, 255, 255, 0.1) 20px
  );
  animation: wave-move 3s linear infinite;
}

.poem-text {
  position: relative;
  color: #004d00;
  font-family: "KaiTi", "楷体", "STKaiti", serif;
  font-weight: bold;
  font-size: 1.8em;
  line-height: 1.8;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
  z-index: 1;
  margin: 0;
}

@keyframes gradient-wave {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

@keyframes wave-move {
  0% {
    transform: translate(0, 0) rotate(0deg);
  }
  100% {
    transform: translate(50px, 50px) rotate(360deg);
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(-20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

---

# Original Content

<!-- Original content starts here -->
