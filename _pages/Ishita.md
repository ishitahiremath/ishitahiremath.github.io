---
layout: about
title: Home
permalink: /
subtitle: Mcgill University .M.Eng (Thesis) BBME 24' | B.Eng Bioengineering and Biotechnology 22'
nav_order: 1
profile:
  align: right
  image: Ishita_Img.jpg
  image_circular: false # crops the image to make it circular
  address: >
    <p>Montreal, QC, H3W 2P9</p>
    <p>Phone: 438-939-4250</p>
    <p>Email: <a href="mailto:ishita.hiremath@mail.mcgill.ca">ishita.hiremath@mail.mcgill.ca</a></p>

news: true  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
years: [2022]
---
<h2 style="margin-top: 50px;">Hey There!</h2>
Hello! I'm Ishita Hiremath, a second-year M.Eng Thesis student in Biology and Biomedical Engineering at McGill University, currently working under the mentorship of Prof. [Caroline Wagner](https://www.mcgill.ca/bbme/caroline-wagner),[BGH Lab](https://bgh.lab.mcgill.ca/). My Master’s research has been a thrilling exploration of virus-like particles in mucus, where I've developed models to simulate their transport using principles of viscoelasticity and binding interactions. I am particularly excited about trying to integrate machine learning with my models to enhance their accuracy and applicability — an approach quite distinct from my primary field—into my studies. 

This fall 2024, I will begin my Ph.D. at the [BGH Lab](https://bgh.lab.mcgill.ca/), where I plan to delve deeper into the fascinating world of mucus biology using microfluidic chips. Prof. Wagner's willingness to cross traditional disciplinary boundaries inspires me, as it resonates with my belief in the power of interdisciplinary approaches and robust collaboration for groundbreaking research.

Currently, I am diving into the techniques of culturing induced pluripotent stem cells (iPSCs) and exploring how these skills can enhance my research capabilities, thanks to Dr. Luv Srivastav. 

Presenting my research at major conferences in Canada—delivering oral presentations — has been among the highlights of my academic career so far, reinforcing my passion for science communication. As an avid debater and orator, these experiences have not only enhanced my presentation skills but have also deepened my enjoyment of the scientific dialogue.

As I look toward my Ph.D., I am eager to explore innovative technologies such as organ-on-chip and advanced microfluidics, aiming to use machine learning as tools, if need be, to pioneer solutions redefining our approach to biomedical challenges.

<!---🔍 **Actively Seeking Opportunities**:
- **Summer Internship** as a Research Scientist, Machine Learning Engineer, or Quant Researcher in the US. 
<!---
I need to re-write this section

If you believe there's a potential fit, please [contact me](mailto:ishita.hiremath@mail.mcgill.ca). I'm eager to explore new challenges and collaborations.-->

<div class="news" style="width: 65%;">
  <h2 style="margin-top: 50px;">News</h2>
  {% if site.news != blank -%} 
  {%- assign news_size = site.news | size -%}
  <div class="table-responsive" {% if site.news_scrollable and news_size > 5 %}style="max-height: 20vw"{% endif %}>
    <table class="table table-sm table-borderless">
    {%- assign news = site.news | reverse -%}
    {% if site.news_limit %}
    {% assign news_limit = site.news_limit %}
    {% else %}
    {% assign news_limit = news_size %}
    {% endif %}
    {% for item in news limit: news_limit %} 
      <tr>
        <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
        <td>
          {% if item.inline -%} 
            {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
          {%- else -%} 
            <a class="news-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
          {%- endif %} 
        </td>
      </tr>
    {%- endfor %} 
    </table>
  </div>
{%- else -%} 
  <p>No news so far...</p>
{%- endif %} 
</div>


<h2 style="margin-top: 50px;">My Vision in Biological Engineering</h2>  
As a PhD student deeply engaged in bioengineering research, I am continually inspired by the vast possibilities that emerge at the intersection of biology and engineering. My academic journey has spanned pharmacology, bioinformatics, and biomaterials, revealing the transformative potential of applying engineering principles not only within healthcare but also across other critical sectors such as energy, environmental sustainability, and beyond.   
Biomaterials hold a special place in my research and intellectual curiosity. These materials are not just pivotal in advancing medical science; they also present unique opportunities to tackle some of the most pressing societal challenges. By harnessing the inherent capabilities of biological systems, biomaterials can offer sustainable solutions that extend far beyond the conventional boundaries of medicine.   
Looking ahead, I am driven by a vision to lead and innovate in the field of biological engineering. My goal is to catalyze the transition of biological concepts into real-world applications that enhance not just healthcare but also sectors like energy and environmental sustainability. As I advance in my career, I am committed to being at the forefront of this exciting field, shaping its future and contributing to a more sustainable and healthier world.  

<h2 style="margin-top: 50px;">Publication</h2>  
<!-- _pages/publications.md -->
<div class="publications">
  {%- for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {% bibliography -f papers -q @*[year={{y}}]* %}
  {% endfor %}
</div>
<h2 style="margin-top: 50px;">Past Research Experience</h2>  

**Research Groups**:
- [Biofluids and ​Global Health Lab](https://bgh.lab.mcgill.ca/), McGill University
- [Sintim Research Group](https://sites.google.com/site/sintimgrouphomepage/), Purdue University
- Bio-Nanotechnology Lab, Indian Academy of Sciences
- [Calmettes Lab](https://ccalmettes.profs.inrs.ca/), Université INRS – Laval
- [Cancer Pharmacology Lab](https://discovery.nus.edu.sg/1847-gautam-sethi), National University of Singapore(NUS)
- [Structural Biology and Protein Engineering Lab](https://www.iitr.ac.in/mculaboratory/index.html), IIT Roorkee

**Research Interests**:
- Biomaterials
- Cellular Biology
- Simulations
- Epigenetics and Pharmacology

For more information about me, connections, or just a friendly chat, all contact and social media details are available below.






