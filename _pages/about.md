---
layout: about
title: about
permalink: /
subtitle:

images:
  slider: true

profile:
  align: right
  image: nasa_website.jpeg
  image_circular: false # crops the image to make it circular
  more_info: >
    <strong style="color: black;">elle.miller@ed.ac.uk</strong>

news: true # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

Hi there! I’m Elle, a **third year PhD student** at the University of Edinburgh.

I’m interested in generalisable methods for improving the performance of robotic reinforcement learning agents in contact-rich manipulation, with a focus on tactile sensing. I'm planning on applying my research to a wide range of scenarios, from dexterous manipulation to humanoid physical assistance in healthcare.

I am fortunate to have an awesome PhD supervision team: [Prof. Sethu Vijayakumar](https://web.inf.ed.ac.uk/slmc) (UoE), [Associate Prof. Oisin Mac Aodha](https://homepages.inf.ed.ac.uk/omacaod/) (UoE), [Dr. David Abel](https://david-abel.github.io/) (UoE, DeepMind), and [Associate Prof. Rika Antonova](https://contactrika.github.io/) (University of Cambridge).

Prior to my doctorate I worked for **NASA Jet Propulsion Laboratory (JPL)** and the **DLR Institute for Mechatronics and Robotics**. At NASA I researched semantic perception for robotic autonomy in hazardous environments, while at DLR I worked improving user agency in grasping on the  inspiring assistive robotics system [EDAN](https://www.dlr.de/rm/en/desktopdefault.aspx/tabid-11670). Along the way I also helped create a mobile humanoid robot called [EVA](https://youtu.be/nMkcBbofDY0).

I graduated with First Class Honours in a BEng (Mechatronic (Space)) & BSc (Advanced Physics) from the **University of Sydney** in 2023. As an undergraduate, I undertook several internships in parallel with my studies, working with the **Max Planck Institute of Astronomy**, **University of Cambridge**, **Cochlear**, **Australian National University**, and **Saber Astronautics**.


On a personal note, I enjoy playing and making music, film photography, lindy hop, cinema, and living in different cities. Feel free to get in touch 💌

<style>
.robot-carousel swiper-slide { display: flex; flex-direction: column; justify-content: center; align-items: center; }
.robot-carousel img { max-height: 400px; object-fit: contain; }
.robot-carousel .slide-caption { margin-top: 0.5rem; font-size: 0.9rem; color: var(--global-text-color-light); text-align: center; }
</style>
<swiper-container slides-per-view="1" loop="true" pagination="true" navigation="true" class="robot-carousel mt-3">
  <swiper-slide>
    <img src="{{ 'assets/img/airec_lifting.jpg' | relative_url }}" alt="AIREC" class="img-fluid rounded z-depth-1" loading="eager">
    <div class="slide-caption">Meet AIREC (AI Robot for Embrace and Care). This robot was developed under the Japanese Moonshot Program. In this photo, AIREC had just picked me up from the chair! </div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/valkyrie2.png' | relative_url }}" alt="Valkyrie" class="img-fluid rounded z-depth-1" loading="eager">
    <div class="slide-caption">NASA Valkyrie</div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/edan2.jpeg' | relative_url }}" alt="EDAN" class="img-fluid rounded z-depth-1" loading="lazy">
    <div class="slide-caption">DLR EDAN</div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/eva.png' | relative_url }}" alt="EVA" class="img-fluid rounded z-depth-1" loading="eager">
    <div class="slide-caption">SLMC EVA</div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/justin.jpeg' | relative_url }}" alt="Justin" class="img-fluid rounded z-depth-1" loading="lazy">
    <div class="slide-caption">DLR Justin</div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/mars.jpg' | relative_url }}" alt="Perseverance & Ingenuity" class="img-fluid rounded z-depth-1" loading="lazy">
    <div class="slide-caption">NASA Perseverance & Ingenuity</div>
  </swiper-slide>
</swiper-container>

<!-- <script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=G3JqO2IkDumQbXPCgL1ii_R51Ml__n42MQd4Bkg71XQ&cl=ffffff&w=a"></script> -->