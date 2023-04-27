# Foliage-Shadow-Imposter

### Youtube Vid: https://www.youtube.com/watch?v=tmJ_R4uT0-w&ab_channel=Wanli

<br />

There was no good Nanite Shadow Imposter demonstration on Internet while l wrote this paper. So, l thought, why didn’t l make one? 

<br />

The idea is to increase performance by replacing dynamic shadow-casting foliage with shadow imposters and non-shadow casting foliage and disabling expensive World Position Offset shadow on selected foliage and replace it with a static shadow imposter of the current mesh.

- ![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) `uncached virtual shadow map with dynamic shadow`

<br />

![uncached virtual shadow map with shadow imposter](https://github.com/One1ee/MyGarage/blob/main/delemete1.png)

<br />

- ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) `cached virtual shadow map with shadow imposter`
![cached virtual shadow map with shadow imposter](https://github.com/One1ee/MyGarage/blob/main/deleteme2.png)

<br />
<br />
DisplayMap2 would be WPO foliage with dynamic shadow, and DisplayMap3 would be WPO foliage with static shadow imposter.
Try run through the forests till the end, the density gets higher the further you go. Simple weather and time change functions are also implemented.

Have Fun!



key mapping:
```java
W, A, S, D: move

Z: Go to DisplaMap2(dynamic shadow map)
X: Go to DisplayMap3(shadow imposter map)

C, V, B, N, M: set scalability, c being low(lowest), m being cinematic(highest)

R: change time, adding 6 hours in 1 second
T: change time, adding 6 hours in 20 second
Y: move forward by 30 mins
U: move backward by 30 mins

L: swap realistic Landscape with a simple one
K: swap simple Landscape with a realistic Landscape

1, 2, 3, 4: change weather (clear skies, cloudy, rainy, snowy)

Esc: quit game
```




<p align="center">
  <img src="https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=75212877,1031858063&fm=26&gp=0.jpg" width="400" height="640">
</p>

//colors
- ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) `#f03c15`
- ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) `#c5f015`
- ![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) `#1589F0`

```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```

//break
<br>
