<!DOCTYPE html>
<html>
<head>
<style>
.blink {
  animation: blinker 1s linear infinite;
}

@keyframes blinker {
  50% {
    opacity: 0;
  }
}
</style>
</head>
<body>

<p id="blinkText" class="blink">Texto piscante</p>

<script>
let colors = ['#f03c15', '#c5f015', '#1589F0'];
let i = 0;
setInterval(() => {
  document.getElementById('blinkText').style.color = colors[i];
  i = (i + 1) % colors.length;
}, 1000);
</script>

</body>
</html>
