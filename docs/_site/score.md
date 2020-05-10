# Eklavya Task Score Board

{% assign sorted = site.data.scoreboard | sort: "Score" | reverse %}

| Rank | Team Name         | Assignment 1 | Assignment 2 | Assignment 3 | Assignment 4 | Score |
|:----:|-------------------|:------------:|:------------:|:------------:|:------------:|:-----:|{% for team in sorted %}
| {{ forloop.index }} |{{ team.TeamName }} | {{ team.Assignment1 }} | {{ team.Assignment2 }}  | {{ team.Assignment3 }}  | {{ team.Assignment4 }}  | {{ team.Score }}  |{% endfor %}

[Go back](index.md)

