.heart {
  width: 40px;
  height: 40px;
  position: relative;
  margin: 50px auto;
}

.heart:before,
.heart:after {
  content: "";
  position: absolute;
  left: 20px;
  top: 0;
  width: 20px;
  height: 30px;
  border-radius: 20px 20px 0;
  transform: rotate(45deg);
  transform-origin: 0 100%;
}

.heart:after {
  left: 0;
  transform: rotate(-45deg);
  transform-origin: 100% 100%;
}

@keyframes beat {
  0% {
    transform: scale(1);
  }
  14% {
    transform: scale(1.3);
  }
  28% {
    transform: scale(1);
  }
}

.heart.beat {
  animation: beat 1s infinite linear;
}
