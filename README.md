# Hero Animation

**Essential classes:**
- Hero
- Inkwell
- Navigator
- Route

Standard:
- MaterialPageRoute
- CupertinoPageRoute
- PageRouteBuilder

**Standard hero animation code:**
* hero_animation
* basic_hero_animation


**Jika error :**
> no directionality widget found. scaffold widgets require a directionality widget ancestor.

**Solusi:**
```
void main() {
  runApp(MaterialApp(
    home: MyApp(),
  ));
}
```

Tambahin **MaterialApp** di Root nya.

---

<br>


# Radial hero animations

A radial transformation animates a circular shape into a square shape.
MaterialRectCenter­Arc­Tween defines the tween animation.

Pro tip: The radial hero animation involves intersecting a round shape with a square shape. This can be hard to see, even when slowing the animation with timeDilation, so you might consider enabling the debugPaintSizeEnabled flag during development.

The hero wraps the RadialExpansion widget.
The example defines the tweening interpolation using MaterialRectCenterArcTween.