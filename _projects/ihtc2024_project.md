---
layout: page
title: IHTC 2024
description: Part of the team that ranked 2nd in the Integrated Healthcare Timetabling Competition 2024.
img: assets/img/projects/ihtc2024_certificate.webp
importance: 2
category: former
related_publications: false
---

The [Integrated Healthcare Timetabling Competition 2024](https://ihtc2024.github.io/) (IHTC 2024) [[1]](#1) was an international competition that challenged participants to develop algorithms for solving a complex integrated healthcare timetabling problem. The competition introduced the problem Integrated Healthcare Timetabling Problem (IHTP), which integrates several NP-hard subproblems found in healthcare scheduling, including patient scheduling, nurse rostering and operating theatre scheduling.

As part of a team of two, [Prof. Marco Chiarandini](https://imada.sdu.dk/u/marco) and I, we ranked 2nd in the competition and 1st in the open-source category out of a total of 32 teams across the world. Our solution was a multi-neighborhood, lexicographic local search algorithm that consisted of two phases: a simulated annealing phase followed by an iterated local search phase. The solver is available in our [GitHub repository](https://github.com/Arthod/ihtc2024-imada-submission).

The algorithm was implemented in C++ and was largely structured around the [ROAR-NET API specification](https://github.com/roar-net/roar-net-api-spec), with various modifications focused on performance. Because of this, our result was featured in a [news article from the ROAR-NET](https://roar-net.eu/news/ihtc-2024-best-oss-prize/).

## References
<a id="1">[1]</a> 
Sara Ceschia, Roberto Maria Rosati, Andrea Schaerf, Pieter Smet, Greet Vanden Berghe, Eugenia Zanazzo (2025),
The Integrated Healthcare Timetabling competition 2024,
Operations Research, Data Analytics and Logistics, Volume 45.
[https://doi.org/10.1016/j.ordal.2025.200481](https://doi.org/10.1016/j.ordal.2025.200481).

## Images

Group photos are taken from the [IHTC 2024 homepage](https://ihtc2024.github.io/).

<p align="center">
  <img src="../../assets/img/projects/ihtc2024_participants.jpg" alt="IHTC 2024 Participants" style="max-width: 70%; height: auto;"/>
</p>
<p align="center">
  <img src="../../assets/img/projects/ihtc2024_top5.jpg" alt="IHTC 2024 Top 5 Teams" style="max-width: 70%; height: auto;"/>
</p>
<p align="center">
  <img src="../../assets/img/projects/ihtc2024_certificate.webp" alt="IHTC 2024 Certificate of Achievement" style="max-width: 70%; height: auto;"/>
</p>