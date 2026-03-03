---
title: "CMU 17-332/732 05-332/632: Introduction to Accessibility and Assistive Technology"
hide:
  - navigation
---

# CMU 17-332/732 05-332/632: Introduction to Accessibility and Assistive Technology

## This Week

<div id="this-week">

{%- set this_week = extra.this_week -%}

<div class="card"> 
    <div class="header">
        Lectures & Readings
    </div>
    <div class="content">
        {% if this_week.lectures %}
            {% for lecture in this_week.lectures %}
                <div class="lecture-name">
                    {{ lecture.name }}
                </div>
                <div class="lecture-date">
                    <span class="material-symbols-outlined">calendar_month</span> 
                    {{ lecture.date }}
                </div>

                {% if lecture.link != "" %}
                <a class="label label-gold" href="{{lecture.link}}" target="_blank">
                    <span class="material-symbols-outlined">slideshow</span>
                    Slides
                </a>
                {% endif %}

                {% if lecture.readings %}
                    {% for reading in lecture.readings %}
                        {% if reading.name != "" %}
                            <a class="label label-blue" href="{{reading.link}}" target="_blank">
                            <span class="material-symbols-outlined">link</span>
                            {{reading.name}}
                            </a><br/>
                        {% endif %}
                    {% endfor %}
                {% endif %}
                {% if not loop.last %}
                <hr/>
                {% endif %}
            {% endfor %}
        {% else %}
            None!
        {% endif %}
    </div>

</div>

<div class="card"> 
 
    <div class="header">
        Office Hours
    </div>
    <div class="content">
        Andrew's office hours are held in his office TCS 441.<p>
        See <a href="#class-calendar">class calendar</a> below for exact times!
    </div>

</div>

<div class="card"> 
    <div class="header">
        Projects
    </div>
    <div class="content">
        {% if this_week.projects %}
            {% for project in this_week.projects %}
                <div class="homework-name">
                    {{ project.name }}
                </div>

                <div class="homework-date">
                    <span class="material-symbols-outlined">calendar_month</span>
                    Released {{ project.date }}
                </div>

                {% if project.deadline != "" %}
                <div class="homework-date">
                    <span class="material-symbols-outlined">calendar_month</span>
                    Due {{ project.deadline }}
                </div>
                {% endif %}

                {% if project.link != "" %}
                <a class="label label-red" href="{{project.link}}">
                    <span class="material-symbols-outlined">description</span>Handout
                </a>
                {% endif %}
                {% if not loop.last %}
                <hr/>
                {% endif %}
            {% endfor %}
        {% else %}
            None!
        {% endif %}
    </div>

</div>

</div>

## Class Calendar

<!--<iframe src="https://calendar.google.com/calendar/embed?src=c_816535019d2afe0315ddce666512c1cb44767b09c171338c109e46cb2afde65d%40group.calendar.google.com&ctz=America%2FNew_York" style="border: 0" width="1000" height="600" frameborder="0" scrolling="no"></iframe>-->

## Weekly Schedule

<div id="schedule" markdown>

<!-- Loading in schedule from schedule.yaml -->

{%- set schedule = extra.schedule -%}

{% if schedule %}
{% set ns = namespace(recitation_days_left=0, homework_days_left=0) %}

<table>
    <thead>
        <th><b>Date</b></th>
        <th><b>Lecture</b></th>
        <th><b>Readings</b></th>
        <th><b>Project Deadline</b></th>
    </thead>
    <tbody>
        {% for schedule_day in schedule %}
        <tr>
            <td><span class="schedule-day">{{schedule_day.date}}</span></td>

            <td><span class="schedule-lecture">
                {% if schedule_day.lecture.name != "" and schedule_day.lecture.link != "" %}
                    <a class="label label-gold" href="{{schedule_day.lecture.link}}" target="_blank">
                        {{schedule_day.lecture.name}}
                    </a>
                {% elif schedule_day.lecture.name != "" %}
                    <b>{{schedule_day.lecture.name}}</b>
                {% endif %}
            </span></td>

            <td><span class="schedule-reading">
                {% if schedule_day.readings != "" %}
                    {% for reading in schedule_day.readings %}
                        {% if reading.name != "" %}
                            <a class="label label-blue" href="{{reading.link}}" target="_blank">
                            {{reading.name}}
                            </a><br/>
                        {% endif %}
                    {% endfor %}
                {% endif %}
            </span></td>

            {% if schedule_day.homework.name != "" %}
                <td rowspan="{{schedule_day.homework.numDays}}"><span class="schedule-homework">
                    <b>{{schedule_day.homework.name}}</b>
                    <br/>
                    {{schedule_day.homework.deadline}}
                    <br/>

                    {% if schedule_day.homework.link != "" %}
                    <a class="label label-red" href="{{schedule_day.homework.link}}">
                        <span class="material-symbols-outlined">description</span>Handout
                    </a>
                    {% endif %}
                </span></td>
                {% set ns.homework_days_left = schedule_day.homework.numDays - 1 %}
            {% else %}
                {% if ns.homework_days_left > 0 %}
                    {% set ns.homework_days_left = ns.homework_days_left - 1 %}
                {% else %}
                    <td><span class="schedule-homework"></span></td>
                {% endif %}
            {% endif %}
        </tr>
        {% endfor %}
    </tbody>

</table>

{% else %}
Coming Soon!
{% endif %}

</div>

## Staff

### Instructors

<div id="course-instructors">
{%- set instructors = extra.staff | selectattr("role", "==", "Instructor") | list -%}
{% for instructor in instructors %}
<div class="staffer card"> 
    <div class="container">
        <img class="staffer-image" src="/assets/images/{{instructor.photo}}" alt="">
        <div>
            <h3 class="staffer-name"> 
                {{instructor.name}}
            </h3>
            <div class="staffer-links">
                <a href="mailto:{{instructor.email}}"><span class="material-symbols-outlined">
                    mail
                </span></a>
                {% if instructor.website %}
                <a href="{{instructor.website}}" target="_blank"><span class="material-symbols-outlined">
                    public
                </span></a>
                {% endif %}
            </div>
        </div>
    </div>
</div>
{% endfor %}

</div>

{%- set assistants = extra.staff | selectattr("role", "==", "Teaching Assistant") | list -%}
{%- set num_teaching_assistants = assistants | count -%}

{% if num_teaching_assistants > 0 %}

### Teaching Assistants

<div id="course-assistants">

{% for assistant in assistants %}

<div class="staffer card"> 
    <div class="container">
        <img class="staffer-image" src="/assets/images/{{assistant.photo}}" alt="">
        <div>
            <h3 class="staffer-name"> 
                {{assistant.name}}
            </h3>
            <div class="staffer-links">
                <a href="mailto:{{assistant.email}}"><span class="material-symbols-outlined">
                    mail
                </span></a>
                {% if assistant.website %}
                <a href="{{assistant.website}}" target="_blank"><span class="material-symbols-outlined">
                    public
                </span></a>
                {% endif %}
            </div>
        </div>
    </div>
</div>
{% endfor %}

</div>
{% endif %}
