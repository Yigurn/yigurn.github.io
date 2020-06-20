---
layout: post
title: "Drum Controller"
date: 2020-04-12
categories: ['Programming']
tags: drums music game
image: http://placehold.it/900x300
subtitle: New game idea
---
<p>Whenever I have seen drum simulators, they seem to fall into one of two catagories:</p>
<ol>
  <li>A VR setup where you actually move as if you are at a drum kit.</li>
  <li>A top-down view of a drum kit, where you click on individual drums with your fingers/mouse.</li>
</ol>
<p>After playing my brothers new twin-stick game <a href="https://thenewtropic.itch.io/extreme-social-distancing">Extreme Social Distancing</a>, I was sitting at my drum kit and realized the idea could be used to make a challenging drum simulator where you have to move the sticks around as well as focus on playing in time. The goal is, to have a game where you can control the hands and feet in order to play percussion instruments, having beats or songs to play along to, similar to Guitar Hero.</p>

<p>I began creating a simple concept game to test how practical/challenging it is.</p>

<img width="600" height="400" src="https://via.placeholder.com/600x400.gif?text=Gif+of+0.0.3" alt="" />

<p>It turns out controlling the sticks was even harder than I imagined, so I began work on some new input method.</p>

<p>First was the grid method, each drum found it's closest neighbour in each of the four cardinal directions which the stick could travel between. The other method I implemented was of a circular style, where the drums were all put in a ring and the stick would travel to the drum closest to the angle given. Whilst the second method does work, it is something you have to get used to.</p>
