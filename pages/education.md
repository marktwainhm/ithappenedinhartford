---
title: It Happened Here in Your Town
layout: about
permalink: /education.html
---

Education Program Page! 

Cupcake ipsum dolor sit amet liquorice brownie chocolate bar. Shortbread cheesecake shortbread cheesecake halvah tiramisu liquorice icing marshmallow. Tart danish cake soufflé topping. Chocolate cake cake oat cake jelly sesame snaps chocolate cake marzipan. Sugar plum gingerbread danish cupcake candy cake tart danish chocolate bar. Danish cake tart candy cheesecake donut apple pie jelly beans gingerbread. Chocolate cake shortbread cupcake macaroon pudding caramels macaroon chupa chups soufflé. Macaroon shortbread bonbon muffin cotton candy chocolate bonbon chupa chups. Liquorice dragée danish cheesecake sweet biscuit cheesecake. Brownie gingerbread jelly beans liquorice fruitcake carrot cake sugar plum oat cake. Oat cake pudding biscuit sesame snaps cookie gingerbread. Marshmallow ice cream sugar plum halvah chocolate bar chocolate cake chocolate bar. Cookie cupcake gingerbread bonbon cookie cookie. Cookie jujubes cupcake gingerbread cookie.

What else should be on this page?

## Essays
{% for town in site.towns %}
- 	[{{ town.title }}]({{ town.permalink }}) by {{ town.author }}
{% endfor %}