---
layout: about
title: About
permalink: /
subtitle: Mcgill University .M.Eng (Thesis). BBME 24' | B.Eng Bioengineering and Biotechnology 22'
nav_order: 1
profile:
  align: right
  image: chenda_pic.jpg
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
Hello! I'm Ishita Hiremath, `a second-year M.Eng Thesis student in Biology and Biomedical Engineering at McGill University, advised by Prof. [Caroline Wagner](https://www.mcgill.ca/bbme/caroline-wagner). I will be strating my Ph.D under Prof. Wagner at the [] (BGH Lab) [https://bgh.lab.mcgill.ca/] this fall 2024. Previously, I graduated with a B.Eng. in Bioengineering and Biotechnology from Birla Institute of Technology, Mesra India.

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

<h2 style="margin-top: 50px;">About my academics.</h2>

The field of computer science is vast and ever-evolving. Within this expansive domain, it is hard to constrain yourself into a specific area of interest. I am a firm believer in the power of interdisciplinary research and the importance of a broad skillset. I am passionate about the intersection of machine learning, computer vision, LLMs, and robotics. I am also very interested in the application of machine learning in the field of Biology, Medicine, and Economics.

**Research Interests**:
- AI for Science
- LLM, LMMs
- Reinforcement Learning
- Robotics


At UCLA, I've been privileged to collaborate with three prominent research teams:

**Research Groups**:
- UCLA Prof Vwani Roychowdhury's Group
- UCLA Prof Bolei Zhou'S Group
- UCLA's Center for Neurobehavioral Genetics.
- UCLA Structures-Computer Interaction Lab.


For more information about me, connections, or just a friendly chat, all contact and social media details are available below.





