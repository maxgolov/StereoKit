---
layout: default
title: Vec3.PerpendicularRight
description: Exactly the same as Vec3.Cross, but has some naming memnonics for getting the order right when trying to find a perpendicular vector using the cross product. This'll also make it more obvious to read if that's what you're actually going for when crossing vectors!  If you consider a forward vector and an up vector, then the direction to the right is pretty trivial to imagine in relation to those vectors!
---
# [Vec3]({{site.url}}/Pages/Reference/Vec3.html).PerpendicularRight

<div class='signature' markdown='1'>
static [Vec3]({{site.url}}/Pages/Reference/Vec3.html) PerpendicularRight([Vec3]({{site.url}}/Pages/Reference/Vec3.html) forward, [Vec3]({{site.url}}/Pages/Reference/Vec3.html) up)
</div>

|  |  |
|--|--|
|[Vec3]({{site.url}}/Pages/Reference/Vec3.html) forward|What way are you facing?|
|[Vec3]({{site.url}}/Pages/Reference/Vec3.html) up|What direction is up?|
|RETURNS: [Vec3]({{site.url}}/Pages/Reference/Vec3.html)|Your direction to the right! Result is -not- a unit vector, even if both 'forward' and 'up' are unit vectors.|

Exactly the same as Vec3.Cross, but has some naming
memnonics for getting the order right when trying to find a
perpendicular vector using the cross product. This'll also make
it more obvious to read if that's what you're actually going for
when crossing vectors!

If you consider a forward vector and an up vector, then the
direction to the right is pretty trivial to imagine in relation
to those vectors!



