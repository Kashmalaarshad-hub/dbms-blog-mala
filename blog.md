---
layout: page
title: Technical Portfolio & Lab Logs
permalink: /blog/
---

<div style="font-family: 'Segoe UI', Tahoma, sans-serif; color: #333; max-width: 900px; margin: auto; line-height: 1.6;">

    <div style="background: #ffffff; border: 1px solid #dee2e6; border-top: 5px solid #2c3e50; padding: 30px; border-radius: 4px; margin-bottom: 40px; box-shadow: 0 2px 4px rgba(0,0,0,0.05);">
        <h2 style="margin-top: 0; color: #2c3e50; letter-spacing: 0.5px;">Semester Overview</h2>
        <p style="color: #555;">This digital portfolio documents my technical growth and laboratory work during the current semester at <strong>UET Faisalabad</strong>. The content focuses on database architecture, programming logic, and practical data implementation.</p>
        
        <div style="display: flex; gap: 20px; margin-top: 25px; font-size: 0.85em; text-transform: uppercase; font-weight: bold; color: #666;">
            <div style="flex: 1; border-left: 3px solid #0056b3; padding-left: 10px;">Primary Focus: DBMS</div>
            <div style="flex: 1; border-left: 3px solid #d9534f; padding-left: 10px;">Secondary Focus: PF</div>
            <div style="flex: 1; border-left: 3px solid #5cb85c; padding-left: 10px;">Status: In Progress</div>
        </div>
    </div>

    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 25px; margin-bottom: 50px;">
        <div style="border: 1px solid #e1e4e8; padding: 25px; border-radius: 8px; background: #fafbfc;">
            <h3 style="color: #0366d6; margin-top: 0; border-bottom: 1px solid #eee; padding-bottom: 10px;">Database Systems</h3>
            <p style="font-size: 0.9em; color: #444;">Implementation of relational schemas, SQL optimization, and WAMP server connectivity.</p>
            <ul style="font-size: 0.85em; padding-left: 20px; color: #555;">
                <li>Relational Modeling & ERDs</li>
                <li>Database Normalization (1NF - 3NF)</li>
                <li>Structured Query Language (SQL)</li>
            </ul>
        </div>
        
        <div style="border: 1px solid #e1e4e8; padding: 25px; border-radius: 8px; background: #fafbfc;">
            <h3 style="color: #d73a49; margin-top: 0; border-bottom: 1px solid #eee; padding-bottom: 10px;">Programming Logic</h3>
            <p style="font-size: 0.9em; color: #444;">Logical problem-solving using C++ with emphasis on memory management and structured code.</p>
            <ul style="font-size: 0.85em; padding-left: 20px; color: #555;">
                <li>Control Structures & Loops</li>
                <li>Modular Programming (Functions)</li>
                <li>Array Manipulation & Logic</li>
            </ul>
        </div>
    </div>

    <h2 style="border-bottom: 2px solid #2c3e50; padding-bottom: 10px; color: #2c3e50; font-size: 1.5em;">Detailed Lab Entries</h2>
    
    <div style="margin-top: 20px;">
        {% for post in site.posts %}
        <div style="padding: 25px 0; border-bottom: 1px solid #f0f0f0;">
            <h3 style="margin: 0; font-size: 1.25em;">
                <a href="{{ post.url | relative_url }}" style="color: #0366d6; text-decoration: none;">{{ post.title }}</a>
            </h3>
            <div style="margin: 10px 0; font-size: 0.8em; color: #888; font-weight: 600;">
                DATE: {{ post.date | date: "%B %d, %Y" }} | CATEGORY: {{ post.categories | join: ' / ' | upcase }}
            </div>
            <p style="font-size: 0.95em; color: #555; margin-top: 10px; line-height: 1.7;">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
            <a href="{{ post.url | relative_url }}" style="font-size: 0.85em; color: #0366d6; font-weight: bold; text-decoration: underline;">VIEW FULL REPORT</a>
        </div>
        {% endfor %}
    </div>

    <div style="margin-top:
