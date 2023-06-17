---
layout: post
title:  "Older Game"
summary: "Associate Technical Designer"
date:   2022-09-07 15:39:40
preview: /assets/images/postpreview.png
---

<!-- ![Picture 1](Portfolio/assets/fullsize.png) -->
![m'lady](https://i.imgur.com/v8IVDka.jpg)
Put down info here, either in bullets or paragraphs.

This site was built using [github pages](https://pages.github.com/).

```cs
 public void Hit(Weapon weapon)
    {
        var canReflect = isAngleCorrect(weapon.BladeDirection);
        weapon.IsReflect = canReflect && durability > 0;
        SparkParticles.Play();

        if (canReflect)
        {
            durability--;
            if (durability <= 0)
            {
                ArmoredLimb.enabled = true;
                Destroy(this);
            }
        }
    }
```