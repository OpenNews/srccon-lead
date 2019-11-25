---
layout: layout
section: sessions
photocredit: Erik Westra
photocredit_url: http://www.westraco.com/
permalink: /sessions/
title: SRCCON:LEAD 2019 — Sessions
---

## Sessions at SRCCON:LEAD

Sessions at SRCCON:LEAD are [collaborative and hands-on](/program), a chance to draw on the experiences of every attendee and work together on plans to change the power dynamics in journalism. Our schedule will explore what journalism leadership could and _should_ look like, and help us teach each other skills we can use to be part of that change.

Here are the sessions we've confirmed for SRCCON:LEAD so far. This list and these descriptions may evolve between now and our conference on November 19 & 20 in Philadelphia. Huge thanks to all who submitted proposals, and to the [community reviewers](#community-review) who helped us during the review process.

<div class="session-proposal-list">{% comment %}The one-line if statement below is ugly but prevents massive whitespace in the template{% endcomment %}
{% for proposal in site.data.sessions %}
    {% if proposal.facilitator.size > 0 and proposal.facilitator_twitter.size > 0 %}{% capture facilitator_name %}<a href="https://twitter.com/{{ proposal.facilitator_twitter }}">{{ proposal.facilitator }}</a>{% endcapture %}{% elsif proposal.facilitator.size > 0 %}{% capture facilitator_name %}{{ proposal.facilitator }}{% endcapture %}{% else %}{% assign facilitator_name = false %}{% endif %}{% if proposal.cofacilitator.size > 0 and proposal.cofacilitator_twitter.size > 0 %}{% capture cofacilitator_name %}<a href="https://twitter.com/{{ proposal.cofacilitator_twitter }}">{{ proposal.cofacilitator }}</a>{% endcapture %}{% elsif proposal.cofacilitator.size > 0 %}{% capture cofacilitator_name %}{{ proposal.cofacilitator }}{% endcapture %}{% else %}{% assign cofacilitator_name = false %}{% endif %}{% if proposal.cofacilitator_two.size > 0 and proposal.cofacilitator_two_twitter.size > 0 %}{% capture cofacilitator_two_name %}<a href="https://twitter.com/{{ proposal.cofacilitator_two_twitter }}">{{ proposal.cofacilitator_two }}</a>{% endcapture %}{% elsif proposal.cofacilitator_two.size > 0 %}{% capture cofacilitator_two_name %}{{ proposal.cofacilitator_two }}{% endcapture %}{% else %}{% assign cofacilitator_two_name = false %}{% endif %}{% if proposal.cofacilitator_three.size > 0 and proposal.cofacilitator_three_twitter.size > 0 %}{% capture cofacilitator_three_name %}<a href="https://twitter.com/{{ proposal.cofacilitator_three_twitter }}">{{ proposal.cofacilitator_three }}</a>{% endcapture %}{% elsif proposal.cofacilitator_three.size > 0 %}{% capture cofacilitator_three_name %}{{ proposal.cofacilitator_three }}{% endcapture %}{% else %}{% assign cofacilitator_three_name = false %}{% endif %}
    <div class="session-proposal" id="{{ proposal.id }}">
        <h2 class="session-title"><a href="#{{ proposal.id }}">{{ proposal.title }}</a></h2>
        {% if facilitator_name %}<p class="facilitator">Facilitated by {{ facilitator_name }}{% if cofacilitator_name %} &amp; {{ cofacilitator_name }}{% endif %}{% if cofacilitator_two_name %} &amp; {{ cofacilitator_two_name }}{% endif %}{% if cofacilitator_three_name %} &amp; {{ cofacilitator_three_name }}{% endif %}</p>{% endif %}
        <p class="session-description">{{ proposal.description | markdownify }}</p>
    </div>
{% endfor %}
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script src="/media/js/listfilter.min.js"></script>
<script>
var filter = ListFilter({
    listContainer: '.session-proposal-list',
    filterItemClass: '.session-proposal'
});
</script>

<span id="community-review"></span>

## Community reviewers

We'd also like to thank the people who helped us think through themes and programming for SRCCON:LEAD and select this amazing slate of sessions!

* Erin Mansfield
* Angilee Shah