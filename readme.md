# Foliage-Shadow-Imposter

### Youtube Vid: 
https://www.youtube.com/watch?v=tmJ_R4uT0-w&ab_channel=Wanli

### Paper: 
https://www.spiedigitallibrary.org/conference-proceedings-of-spie/12784/127842E/Unreal-engine-nanite-foliage-shadow-imposter/10.1117/12.2692451.short#_=_
<br />

#### There was no good Nanite Shadow Imposter demonstration on the Internet while l wrote this paper. 
#### So, l thought, why didn’t l make one?  ####


<br />
<br />

<p align="center">
  <img src="https://raw.githubusercontent.com/One1ee/MyGarage/main/usethis.png"/>
</p>

---

<br />

The idea is to increase performance by replacing dynamic shadow-casting foliage with shadow imposters and non-shadow casting foliage, disabling expensive World Position Offset shadow on selected foliage and replace it with a static shadow imposter of the current mesh.

- ![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) `uncached virtual shadow map with dynamic shadow`

![uncached virtual shadow map with shadow imposter](https://raw.githubusercontent.com/One1ee/MyGarage/main/delemete1.png)

<br />

- ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) `cached virtual shadow map with shadow imposter`

![cached virtual shadow map with shadow imposter](https://raw.githubusercontent.com/One1ee/MyGarage/main/deleteme2.png)

<br />
<br />
DisplayMap2 is built with WPO foliage with dynamic shadow; DisplayMap3 is built with WPO foliage with static shadow imposter.<br />
Try run through the forests, the density gets higher the further you go. <br />
Simple weather change, time change, and Landscape replacement functions are also implemented(see below👇).

#### Have Fun!
<br />

---
#### key mapping:
```java
//movement
W, A, S, D: move

//swap maps
Z: Go to DisplaMap2(dynamic shadow map)
X: Go to DisplayMap3(shadow imposter map)

//scalability
C, V, B, N, M: set scalability, c being low(lowest), m being cinematic(highest)

//time change
R: change time, adding 6 hours in 1 second
T: change time, adding 6 hours in 20 second
Y: move forward by 30 mins
U: move backward by 30 mins

// landscape replacement
L: swap realistic Landscape with a simple one
K: swap simple Landscape with a realistic Landscape

// weather rotation
1, 2, 3, 4: change weather (clear skies, cloudy, rainy, snowy)

Esc: quit game
```

<br />

