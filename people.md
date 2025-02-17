---
layout: default
title:
description:
---

{% assign organizers = site.data.people | where:'role', 'organizer' | sort: "nick" %}

{% assign presenters2023sep = site.data.people | where_exp: "person", "person.role contains 'presenter-2023-09'" | sort: "nick" %}
{% assign panelists2023sep = site.data.people | where_exp: "person", "person.role contains 'panelist-2023-09'" | sort: "nick" %}
{% assign presenters2023nov = site.data.people | where_exp: "person", "person.role contains 'presenter-2023-11'" | sort: "nick" %}
{% assign panelists2023nov = site.data.people | where_exp: "person", "person.role contains 'panelist-2023-11'" | sort: "nick" %}
{% assign presenters2024feb = site.data.people | where_exp: "person", "person.role contains 'presenter-2024-02'" | sort: "nick" %}
{% assign panelists2024feb = site.data.people | where_exp: "person", "person.role contains 'panelist-2024-02'" | sort: "nick" %}
{% assign presenters2024apr = site.data.people | where_exp: "person", "person.role contains 'presenter-2024-04'" | sort: "nick" %}
{% assign panelists2024apr = site.data.people | where_exp: "person", "person.role contains 'panelist-2024-04'" | sort: "nick" %}
{% assign presenters2024sep = site.data.people | where_exp: "person", "person.role contains 'presenter-2024-09'" | sort: "nick" %}
{% assign panelists2024sep = site.data.people | where_exp: "person", "person.role contains 'panelist-2024-09'" | sort: "nick" %}
{% assign presenters2024dec = site.data.people | where_exp: "person", "person.role contains 'presenter-2024-12'" | sort: "nick" %}
{% assign panelists2024dec = site.data.people | where_exp: "person", "person.role contains 'panelist-2024-12'" | sort: "nick" %}
{% assign presenters2025feb = site.data.people | where_exp: "person", "person.role contains 'presenter-2025-02'" | sort: "nick" %}
{% assign panelists2025feb = site.data.people | where_exp: "person", "person.role contains 'panelist-2025-02'" | sort: "nick" %}

# Organizers
---
{% for person in organizers %}

  {% include person.html %}

{% endfor %}

# February 2025 Seminar
---

## Presenters

{% for person in presenters2025feb %}

  {% include person.html %}

{% endfor %}

<!-- ## Panelists

{% for person in panelists2025feb %}

  {% include person.html %}

{% endfor %} -->

# December 2024 Seminar
---

## Presenters

{% for person in presenters2024dec %}

  {% include person.html %}

{% endfor %}

<!-- ## Panelists

{% for person in panelists2024dec %}

  {% include person.html %}

{% endfor %} -->

# September 2024 Seminar
---

## Presenters

{% for person in presenters2024sep %}

  {% include person.html %}

{% endfor %}

<!-- ## Panelists

{% for person in panelists2024sep %}

  {% include person.html %}

{% endfor %} -->

# April 2024 Seminar
---

## Presenters

{% for person in presenters2024apr %}

  {% include person.html %}

{% endfor %}

<!-- ## Panelists

{% for person in panelists2024apr %}

  {% include person.html %}

{% endfor %} -->

# February 2024 Seminar
---

## Presenters

{% for person in presenters2024feb %}

  {% include person.html %}

{% endfor %}

<!-- ## Panelists

{% for person in panelists2024feb %}

  {% include person.html %}

{% endfor %} -->
# November 2023 Seminar
---

## Presenters

{% for person in presenters2023nov %}

  {% include person.html %}

{% endfor %}

<!-- ## Panelists

{% for person in panelists2023nov %}

  {% include person.html %}

{% endfor %} -->

# September 2023 Seminar
---

## Presenters

{% for person in presenters2023sep %}

  {% include person.html %}

{% endfor %}

<!-- ## Panelists

{% for person in panelists2023sep %}

  {% include person.html %}

{% endfor %} -->
