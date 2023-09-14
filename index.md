---
layout: home
title: Home
nav_order: 1
nav_exclude: false
permalink: index.html
seo:
  type: Course
  name: Data 8 Spring 2024
---

# Data 8: Foundations of Data Science

{: .mb-2 }
Inclusion Bridge, College Advantage 2024
{: .mb-2 .fs-6 .text-grey-dk-000 }

[Lecture Zoom Link](https://us06web.zoom.us/my/ttogun?pwd=bGsxeU1uN0F0ZHVTQ1NBTWVWNUNEdz09){: .btn .btn-blue}

## Let us start your Data Science Journey together

**Acknowledgements**

This course is adopted from Data 8, “The Foundations of Data Science” course taught to first-year students at UC Berkeley.
All materials for the course, including the textbook and assignments, are available for free online under a Creative Commons license.
Textbook: [Computational and Inferential Thinking: The Foundations of Data Science](http://inferentialthinking.com/) is a free online textbook that includes interactive Jupyter notebooks and public data sets for all examples.
Course Materials: The Embedded Demo, Lab and Homework Notebooks as well as linked references all come from publicly available materials used in the course during the [Spring 2020 semester at UC Berkeley](http://www.data8.org/sp20/) as well as materials used in the self-paced [Data 8X course on EdX](https://github.com/data-8/materials-x19).

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}

{% assign mods = site.modules | where: 'class', 'CollegeAdvantage' %}
{% for module in mods %}
{{ module }}
{% endfor %}

<
<br />

<button class="js-toggle-dark-mode dm-btn btn">Toggle Dark Mode</button>

<script src="assets/darkmode.js"></script>
<script>
  const toggleDarkMode = document.querySelector('.js-toggle-dark-mode');

  jtd.addEvent(toggleDarkMode, 'click', function(){
    if (jtd.getTheme() === 'custom_dark') {
      jtd.setTheme('light');
      localStorage.setItem("darkMode", 0);
      toggleDarkMode.innerHTML = "Toggle Dark Mode";
      toggleDarkMode.classList.add('dm-btn');
        toggleDarkMode.classList.remove('dm-dark-btn');
    } else {
      jtd.setTheme('custom_dark');
      localStorage.setItem("darkMode", 1);
      toggleDarkMode.innerHTML = "Return to the Light";
      toggleDarkMode.classList.add('dm-dark-btn');
      toggleDarkMode.classList.remove('dm-btn');
    }
  });

    window.addEventListener("DOMContentLoaded", (event) => {
      onLoad();
  });
</script>
