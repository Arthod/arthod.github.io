---
layout: page
title: IHTC 2024
description: Part of the team that ranked 2nd in the Integrated Healthcare Timetabling Competition 2024.
img: assets/img/projects/ihtc2024_certificate.webp
importance: 1
category: former
related_publications: false
---

The [Integrated Healthcare Timetabling Competition 2024](https://ihtc2024.github.io/) (IHTC 2024) [[1]](#1) was an international optimization competition that challenged participants to develop algorithms for solving the Integrated Healthcare Timetabling Problem (IHTP). The IHTP combines several NP-hard healthcare scheduling problems into a single integrated problem, which includes patient scheduling, nurse rostering, and operating theatre scheduling.

As part of a team of two, Prof. [Marco Chiarandini](https://imada.sdu.dk/u/marco) and I, we ranked 2nd place overall and 1st place in the open-source category among a total of 32 participating teams from around the world. Our solution was a multi-neighborhood, lexicographic local search algorithm consisting of two phases: a simulated annealing phase followed by an iterated local search phase. The solver is available on [GitHub](https://github.com/Arthod/ihtc2024-imada-submission).

The implementation is written in C++ and was largely based on the [ROAR-NET API specification](https://github.com/roar-net/roar-net-api-spec), with various modifications focused on performance. The work was featured in a [ROAR-NET news article](https://roar-net.eu/news/ihtc-2024-best-oss-prize/), and we presented it at [EURO 2025 in Leeds](https://www.euro-online.org/conf/euro34/treat_abstract?paperid=2774) as well as at the [ROAR-NET Third General Meeting in Zagreb](https://roar-net.eu/events/third-general-meeting/).

Final paper is currently awaiting publication in a special issue of *Operations Research, Data Analytics and Logistics* (ORDAL) dedicated to the competition.


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