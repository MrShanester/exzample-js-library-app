<template>
  <div>
    <h1></h1>
  </div>
</template>

<script>
import Two from "two.js";

var two = new Two({
  fullscreen: true,
  autostart: true,
}).appendTo(document.body);
var rect = two.makeRectangle(two.width / 2, two.height / 2, 50, 50);
two.bind("update", function () {
  rect.rotation += 0.1;
});

console.log("Importing this square using their docs took me nearly an hour and a half.");
</script>
