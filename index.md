---
title: 연습 지침
permalink: index.html
layout: home
---

# 연습

이 페이지에는 [Microsoft Learn](https://learn.microsoft.com)의 Microsoft 기술 콘텐츠와 관련된 연습이 나열되어 있습니다.

<!-- You can edit the paragraph above to provide a more specific description and links to content on Learn.

Include the following note if an Azure subscription is required (or add something similar for any other requirements, such as a Microsoft 365 account).

> **Note**: To complete these exercises, you will need a [Microsoft Azure subscription](https://azure.microsoft.com/free) in which you have sufficient permissions to create and configure the required resources.

If a more complex setup is required, create a separate markdown file with setup instructions at \Instructions\Labs\00-setup.md - being sure to include "lab.title"" metadata at the top so it shows up the list below
-->

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %} {% for activity in labs  %}
- [{{ activity.lab.title }}]({{ site.github.url }}{{ activity.url }}) {% endfor %}

