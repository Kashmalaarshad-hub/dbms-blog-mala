---
layout: page
title: Technical Portfolio
permalink: /blog/
---

<div style="font-family: 'Segoe UI', Arial, sans-serif; color: #333; max-width: 850px; margin: auto;">

    <div style="text-align: center; padding: 20px; border-bottom: 2px solid #eee; margin-bottom: 30px;">
        <h1 style="color: #2c3e50; margin: 0;">Academic Lab Portfolio</h1>
        <p style="color: #7f8c8d; margin-top: 10px;">Documentation of DBMS and Programming Fundamentals</p>
    </div>

    <div style="background: #fff; border: 1px solid #e1e4e8; border-left: 5px solid #0366d6; padding: 20px; border-radius: 6px; margin-bottom: 25px;">
        <h3 style="color: #0366d6; margin-top: 0;">Database Management Systems (DBMS)</h3>
        <p style="font-size: 0.95em;">Focusing on Relational Modeling, SQL query optimization, and database normalization techniques.</p>
        <div style="font-size: 0.85em; color: #586069; font-weight: bold;">
            Skills: MySQL | ER Diagrams | SQL Queries
        </div>
    </div>

    <div style="background: #fff; border: 1px solid #e1e4e8; border-left: 5px solid #f66a0a; padding: 20px; border-radius: 6px; margin-bottom: 40px;">
        <h3 style="color: #f66a0a; margin-top: 0;">Programming Fundamentals (PF)</h3>
        <p style="font-size: 0.95em;">Core logic building using C++, including control structures, functions, and memory management.</p>
        <div style="font-size: 0.85em; color: #586069; font-weight: bold;">
            Skills: C++ Logic | Iterative Structures | Data Types
        </div>
    </div>

    <h3 style="color: #2c3e50; border-bottom: 1px solid #eee; padding-bottom: 10px;">Recent Lab Entries</h3>
    {% for post in site.posts %}
    <div style="padding: 15px 0; border-bottom: 1px solid #f6f8fa;">
        <h4 style="margin: 0;"><a href="{{ post.url | relative_url }}" style="color: #0366d6; text-decoration: none;">{{ post.title }}</a></h4>
        <p style="font-size: 0.9em; color: #586069; margin: 5px 0;">{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
        <small style="color: #959da5;">Date: {{ post.date | date_to_string }}</small>
    </div>
    {% endfor %}

</div>
