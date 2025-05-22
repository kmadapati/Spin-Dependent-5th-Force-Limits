---
layout: default
title: Conferences
---

# Conferences

Stay updated with upcoming and past conferences:

## Upcoming Conferences

{% for conference in site.data.conferences %}
{% if conference.status == 'upcoming' %}
### {{ conference.title }}

**Date:** {{ conference.date }}

**Location:** {{ conference.location }}

**Link:** [{{ conference.link_text }}]({{ conference.link }})

---

{% endif %}
{% endfor %}

## Past Conferences

{% for conference in site.data.conferences %}
{% if conference.status == 'past' %}
### {{ conference.title }}

**Date:** {{ conference.date }}

**Location:** {{ conference.location }}

**Link:** [{{ conference.link_text }}]({{ conference.link }})

---

{% endif %}
{% endfor %}
