---
layout: page
title: Staff
description: A listing of all the officer team
nav_order: 4
---

# **Staff**

<!-- ## Instructors

<div class="role flex">
{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}
</div> -->

## Executive Team

{% assign head_teaching_assistants = site.staffers | where: 'role', '20-hour Lead uGSI (UCS2)' %}
{% assign num_head_teaching_assistants = head_teaching_assistants | size %}
{% if num_head_teaching_assistants != 0 %}

<div class="role flex">
{% for staffer in head_teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
</div>

<!-- ## Teaching Assistants

{% assign teaching_assistants = site.staffers | where: 'role', 'uGSI (UCS2)' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}


<div class="role flex">
{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
</div>

## Tutors
{% assign tutors = site.staffers | where: 'role', 'Tutor (UCS1)' %}
{% assign num_tutors = tutors | size %}
{% if num_tutors != 0 %}

<div class="role flex">
{% for staffer in tutors %}
{{ staffer }}
{% endfor %}
{% endif %}
</div> -->