---
layout: default
---

<link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.10.21/css/jquery.dataTables.min.css" />
<script src="https://code.jquery.com/jquery-3.5.1.js"></script>
<script src="https://cdn.datatables.net/1.10.21/js/jquery.dataTables.min.js"></script>

# SPRING 2026

## Class Information

| Item                   |
| ---------------------- | ---------------------------------------------------- |
| Schedule               | Tuesdays 6:00 - 7:00 PM Eastern                      |
| Location               | Zoom. Details on Carmen                              |
| Professor              | Brad Coy / coy DOT 48 AT osu DOT edu                 |
| Professor Office Hours | Thursdays 6:00 - 7:00 PM Eastern. Details on Carmen. |
| TA                     | Not applicable                                       |
| TA Office Hours        | Not applicable                                       |

## Description:

This class aims to introduce ways to mine and analyze data for people who are in data related fields but are not necessarily computer scientists or data scientists. This webpage will serve as a source of content for the course, including homework and project files.
It is highly encouraged that you simply fork this entire repo and then periodically sync updates. This will provide you the easiest access to all the updated code at once. For more information on this process, you can see the documentation [here](https://docs.github.com/en/get-started/quickstart/fork-a-repo).

## Github Repository Details

If you would like to make a correction or a fix (either to this page or the associated jupyter notebooks/data) please submit a pull request. I'll review and merge and then hopefully, everyone taking this class benefits!

The direct link to the actual repository is here: [https://github.com/bcoy48/osu-gradtda-5622-sp25](https://github.com/bcoy48/osu-gradtda-5622-sp25).

## Grading Plan:

1. Homework x5: 30%
2. Case Studies x4: 40%
3. Final Project: 20%
4. Participation: 10%

There might be tentative bonus points assigned for harder math or cs problems. Max would be at most 2-3% per problem.

## Homeworks

<table class="display" border=1 frame=sides rules=all>
  {% for row in site.data.Homeworks %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ 	pair[1] }}
    {% endtablerow %}

{% endfor %}

</table>

## Case Studies

<table class="display" border=1 frame=sides rules=all>
  {% for row in site.data.Casestudies %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ 	pair[1] }}
    {% endtablerow %}

{% endfor %}

</table>

## Synchronous Class Notebooks

<table class="display" border=1 frame=sides rules=all>
  {% for row in site.data.SyncClass %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ 	pair[1] }}
    {% endtablerow %}

{% endfor %}

</table>

## Final

<table class="display" border=1 frame=sides rules=all>
  {% for row in site.data.Final %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ 	pair[1] }}
    {% endtablerow %}

{% endfor %}

</table>

#### Site created by Greg Ryslik (gryslik) for Spring 2024 term. Adapted by Brad Coy (bcoy48) for Spring 2025, 2026 terms.

{{ page.last_modified_at }}
