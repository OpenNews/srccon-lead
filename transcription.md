---
layout: layout
section: remote
permalink: /transcription/
---

# Transcription

SRCCON:LEAD is an intentionally small event, but we also care about getting these conversations into the wider world. The most important way this happens is when attendees return home and put their new skills and approaches to work, but we also document extensively.

Our captioner will provide live transcription of each talk and several of the sessions at SRCCON:LEAD. Links to the transcripts will remain below.

<div>
    <h3>Tuesday</h3>
    <table>{% assign tuesday = site.data.schedule | where:"day","Tuesday" %}
{% for session in tuesday %}
        {% if session.transcription != "" %}<tr><td>{{ session.time }}</td><td><a href="{{ session.transcription }}">{{ session.title }}</a></td></tr>{% endif %}
{% endfor %}
    </table>
</div>

<div>
    <h3>Wednesday</h3>
    <table>{% assign wednesday = site.data.schedule | where:"day","Wednesday" %}
{% for session in wednesday %}
        {% if session.transcription != "" %}<tr><td>{{ session.time }}</td><td><a href="{{ session.transcription }}">{{ session.title }}</a></td></tr>{% endif %}
{% endfor %}
    </table>
</div>
