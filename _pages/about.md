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

Hi there! I’m Elle, a PhD student at the **University of Edinburgh**. My goal is to develop intelligent robots that **empower people** and solve complex real-world problems.

My research lies at the intersection of **reinforcement learning** and robotic control, with a focus on **contact-rich manipulation**. My work leverages **tactile sensing** and **self-supervision** to help agents derive richer latent representations of their physical world. Currently, I am looking into longstanding challenges of RL for whole-body humanoid manipulation. 

I am fortunate to be supervised by a great interdisciplinary team: [Prof. Sethu Vijayakumar](https://web.inf.ed.ac.uk/slmc) (UoE), [Associate Prof. Oisin Mac Aodha](https://homepages.inf.ed.ac.uk/omacaod/) (UoE),  [Associate Prof. Rika Antonova](https://contactrika.github.io/) (University of Cambridge), and [Dr. David Abel](https://david-abel.github.io/) (UoE, DeepMind).

Before my doctorate, I researched robotic autonomy at **NASA Jet Propulsion Laboratory (JPL)** and assistive grasping at the **DLR Institute for Mechatronics and Robotics**. I also helped create [EVA](https://youtu.be/nMkcBbofDY0), a novel mobile humanoid. My journey began at the **University of Sydney**, where I graduated with First Class Honours in Mechatronic (Space) Engineering and Advanced Physics.

Along the way, I've understook internships with **Max Planck Institute of Astronomy**, **Cochlear**, **Australian National University**, and **Saber Astronautics**.

On a personal note, I enjoy tea, jazz music, cinema, and meeting people from around the world. Feel free to get in touch 💌

<style>
.profile .more-info { text-align: center; }
.robot-carousel swiper-slide { display: flex; flex-direction: column; justify-content: center; align-items: center; padding-bottom: 2.5rem; }
.robot-carousel img { max-height: 400px; object-fit: contain; }
.robot-carousel .slide-caption {
  margin-top: 0.75rem;
  padding: 0.6rem 1rem;
  background: var(--global-card-bg-color);
  border-radius: 0.5rem;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12);
  font-size: 1rem;
  color: var(--global-text-color);
  text-align: center;
  max-width: 100%;
}
</style>
<swiper-container slides-per-view="1" loop="true" pagination="true" navigation="true" class="robot-carousel mt-3">
  <swiper-slide>
    <img src="{{ 'assets/img/airec_lifting.jpg' | relative_url }}" alt="AIREC" class="img-fluid rounded z-depth-1" loading="eager">
    <div class="slide-caption">Meet AIREC (AI Robot for Embrace and Care). This robot was developed under the Japanese Moonshot Program. In this photo, AIREC had just picked me up from the chair! </div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/valkyrie2.png' | relative_url }}" alt="Valkyrie" class="img-fluid rounded z-depth-1" loading="eager">
    <div class="slide-caption">NASA's Valkyrie, built in 2015. She was on lease to researchers at Uni of Edinburgh for 10 years.</div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/edan2.jpeg' | relative_url }}" alt="EDAN" class="img-fluid rounded z-depth-1" loading="lazy">
    <div class="slide-caption">DLR's EDAN. This is robotic wheelchair + arm designed to help people with motor impairments carry out everyday tasks. </div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/eva.png' | relative_url }}" alt="EVA" class="img-fluid rounded z-depth-1" loading="eager">
    <div class="slide-caption">SLMC's EVA. This is a hybrid mobile humanoid platform we made  by integrating a Nextage robot (Kawada) with an omnidirectional base.</div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/justin.jpeg' | relative_url }}" alt="Justin" class="img-fluid rounded z-depth-1" loading="lazy">
    <div class="slide-caption">Meet "Rollin' Justin". DLR (German Aerospace Center) make their own robots from scratch, so each robot is a one-of-kind.</div>
  </swiper-slide>
  <swiper-slide>
    <img src="{{ 'assets/img/mars.jpg' | relative_url }}" alt="Perseverance & Ingenuity" class="img-fluid rounded z-depth-1" loading="lazy">
    <div class="slide-caption">NASA's Perseverance & Ingenuity (just models, since they are on Mars! Each rover does have a twin though, that is used for debugging.)</div>
  </swiper-slide>
</swiper-container>

<!-- <script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=G3JqO2IkDumQbXPCgL1ii_R51Ml__n42MQd4Bkg71XQ&cl=ffffff&w=a"></script> -->