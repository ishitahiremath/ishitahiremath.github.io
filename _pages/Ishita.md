---
layout: about
title: Ishita
permalink: /
subtitle: Mcgill University .M.Eng (Thesis) BBME 24' | B.Eng Bioengineering and Biotechnology 22'
nav_order: 1
profile:
  align: right
  image: WhatsApp Image 2024-04-24 at 14.19.57_a02291d5.jpg
  image_circular: False # crops the image to make it circular
  address: >
    <p>Montreal, QC, H3W 2P9</p>
    <p>Phone: 438-939-4250</p>
    <p>Email: ishita.hiremath@mail.mcgill.ca</p>

news: true  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---
<h2 style="margin-top: 50px;">About me</h2>
Hello! I'm Ishita Hiremath, `a second-year M.Eng Thesis student in Biology and Biomedical Engineering at McGill University, advised by Prof. [Caroline Wagner](https://www.mcgill.ca/bbme/caroline-wagner). I will be strating my Ph.D under Prof. Wagner at the [BGH Lab](https://bgh.lab.mcgill.ca/) this fall 2024. Previously, I graduated with a B.Eng. in Bioengineering and Biotechnology from Birla Institute of Technology, Mesra India.

<!---🔍 **Actively Seeking Opportunities**:
- **Summer Internship** as a Research Scientist, Machine Learning Engineer, or Quant Researcher in the US. 
<!---
I need to re-write this section

If you believe there's a potential fit, please [contact me](mailto:ishita.hiremath@mail.mcgill.ca). I'm eager to explore new challenges and collaborations.-->

<div class="news">
  <h2 style="margin-top: 50px;">News</h2>
  {% if site.news != blank -%} 
  {%- assign news_size = site.news | size -%}
  <div class="table-responsive" {% if site.news_scrollable and news_size > 3 %}style="max-height: 10vw"{% endif %}>
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

**Expansive Research Interests**:
- Biomaterials
- Cellular Biology
- Simulations
- Epigenetics and Pharmacology

**Research Groups**:
- Biofluids and ​Global Health Lab, McGill University
- Sintim Research Group, Purdue University
- Bio-Nanotechnology Lab, Indian Academy of Sciences
- Calmettes Lab, Université INRS – Laval
- Carncer Pharmacology Lab, National University of Singapore(NUS)
- Structural Biology and Protein Engineering Lab, IIT Roorkee


For more information about me, connections, or just a friendly chat, all contact and social media details are available below.






