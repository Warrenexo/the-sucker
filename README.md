the-sucker
==========

A js13kGames competition entry. A zombie survival. No guns. Brain only.

Fun hack: Turn those red pixels into something a little slimier. Fork the repository and make the following change to this line:

app.blood.forEach(function (elem)
{
-  ctx.fillStyle = 'rgb(' + (128 + Math.floor(Math.random() * 128)) + ', 0, 0)';
+  ctx.fillStyle = 'rgb(0,' + (128 + Math.floor(Math.random() * 128)) + ', 0)';
   ctx.fillRect(app.round(elem.x), app.round(elem.y), elem.w, elem.h);
});
