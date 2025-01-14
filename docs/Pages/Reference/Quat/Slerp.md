---
layout: default
title: Quat.Slerp
description: Spherical Linear intERPolation. Interpolates between two quaternions! Both Quats should be normalized/unit quaternions, or you may get unexpected results.
---
# [Quat]({{site.url}}/Pages/Reference/Quat.html).Slerp

<div class='signature' markdown='1'>
static [Quat]({{site.url}}/Pages/Reference/Quat.html) Slerp([Quat]({{site.url}}/Pages/Reference/Quat.html) a, [Quat]({{site.url}}/Pages/Reference/Quat.html) b, float slerp)
</div>

|  |  |
|--|--|
|[Quat]({{site.url}}/Pages/Reference/Quat.html) a|Start quaternion, should be normalized/unit              length.|
|[Quat]({{site.url}}/Pages/Reference/Quat.html) b|End quaternion, should be normalized/unit length.|
|float slerp|The interpolation amount! This'll be a if 0,              and b if 1. Unclamped.|
|RETURNS: [Quat]({{site.url}}/Pages/Reference/Quat.html)|A blend between the two quaternions!|

Spherical Linear intERPolation. Interpolates between two
quaternions! Both Quats should be normalized/unit quaternions, or
you may get unexpected results.



