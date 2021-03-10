---
layout: kz-page
permalink: "/travel/"
subheadline:
title: "Exploring the world"
teaser:
header: no
widgets:
- url:
  image: tirana.jpg
  title: ﻿1. Albania
  cols: 3

- url:
  image: vienna.jpg
  title: 2. Austria
  cols: 3

- url:
  image: sarajevo.jpg
  title: 3. Bosnia and Herzogovina
  cols: 3

- url:
  image: canada.jpg
  title: 4. Canada
  cols: 3

- url:
  image: colombia.jpg
  title: 5. Colombia
  cols: 3

- url:
  image: croatia.jpg
  title: 6. Croatia
  cols: 3

- url:
  image: denmark.jpg
  title: 7. Denmark
  cols: 3

- url:
  image: egypt.jpg
  title: 8. Egypt
  cols: 3

- url:
  image: finland.jpg
  title: 9. Finland
  cols: 3

- url:
  image: france.jpg
  title: 10. France
  cols: 3

- url:
  image: georgia.jpg
  title: 11. Georgia
  cols: 3

- url:
  image: germany.jpg
  title: 12. Germany
  cols: 3

- url:
  image: greece.jpg
  title: 13. Greece
  cols: 3

- url:
  image: budapest.jpg
  title: 14. Hungary
  cols: 3

- url:
  image: japan.jpg
  title: 15. Japan
  cols: 3

- url:
  image: india.jpg
  title: 16. India
  cols: 3

- url:
  image: italy.jpg
  title: 17. Italy
  cols: 3

- url:
  image: ireland.jpg
  title: 18. Ireland
  cols: 3

- url:
  image: riga.jpg
  title: 19. Latvia
  cols: 3

- url:
  image: lithuania.jpg
  title: 20. Lithuania
  cols: 3

- url:
  image: malaysia.jpg
  title: ﻿21. Malaysia
  cols: 3

- url:
  image: malta.jpg
  title: 22. Malta
  cols: 3

- url: /travel/mexico/
  image: mexico.jpg
  title: <a href="/travel/mexico/" target="_self">23. Mexico</a>
  cols: 3

- url:
  image: montenegro.jpg
  title: 24. Montenegro
  cols: 3

- url:
  image: morocco.jpg
  title: 25. Morocco
  cols: 3

- url:
  image: netherlands.jpg
  title: 26. Netherlands
  cols: 3

- url:
  image: north_macedonia.jpg
  title: 27. North Macedonia
  cols: 3

- url:
  image: norway.jpg
  title: 28. Norway
  cols: 3

- url:
  image: oman.jpg
  title: 29. Oman
  cols: 3

- url:
  image: panama.jpg
  title: 30. Panama
  cols: 3

- url:
  image: warsaw.jpg
  title: 31. Poland
  cols: 3

- url:
  image: portugal.jpg
  title: 32. Portugal
  cols: 3

- url:
  image: russia.jpg
  title: 33. Russia
  cols: 3

- url:
  image: singapore.jpg
  title: 34. Singapore
  cols: 3

- url:
  image: bratislava.jpg
  title: 35. Slovakia
  cols: 3

- url: /travel/spain/
  image: spain.jpg
  title: <a href="/travel/spain/" target="_self">36. Spain</a>
  cols: 3

- url:
  image: sweden.jpg
  title: 37. Sweden
  cols: 3

- url:
  image: switzerland.jpg
  title: 38. Switzerland
  cols: 3

- url:
  image: uk.jpg
  title: 39. United Kingdom
  cols: 3

- url:
  image: usa.jpg
  title: 40. USA
  cols: 3

---

<div class="row t20">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 4 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
