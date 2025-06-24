---
layout: project
title: Fundraiser Portfolio Scorecard - UW Advancement
subtitle: "Turning siloed data into actionable insights for fundraising strategy"
---
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

**Executive Summary.**
The Fundraiser Portfolio Scorecard Report is a Tableau dashboard and related documentation developed for the University of Washington's University Advancement team, a strategic fundraising unit that generated $668.7 million in FY 2023/24. Our project's core objective was to provide ~197 fundraisers with a centralized, visual tool for efficient and strategic portfolio monitoring. <br/>
**Problem & Solution**: Fundraisers previously lacked a unified tool, leading to difficulties in tracking engagement, prioritizing outreach, and meeting performance goals. Our solution is an interactive Tableau dashboard that centralizes key portfolio insights, offers actionable data, supports pipeline management, and provides real-time visibility.
**Approach & Deliverables**: Our capstone team employed a user-centered design and agile analytics approach. This involved user research, wireframing, data warehouse exploration, SQL view creation, and dashboard prototyping. The key deliverable is the Tableau dashboard which consolidates metrics like contact history, qualification status, and giving activity, applying business logic to identify portfolio gaps and trends.
<br/>
**Impact & Benefits**: This solution is projected to save approximately 500 staff-hours weekly, replace disparate reports, highlight high-priority prospects, and suggest "Next Steps" for major gift officers. It will enable efficient stewardship of the $669 million annual pipeline and lay the groundwork for future AI insights. Ultimately, the scorecard empowers fundraisers to adopt a focused, data-informed approach.
**Challenges & Learnings**: Key challenges included data complexities, access delays, evolving scope, and eventually  user adoption across hundreds of different workflows. The project highlighted the importance of stakeholder alignment and the value of iterative design in addressing user pain points.
**Next Steps**: Future efforts involve transitioning the prototype to a production version through testing, adding linking GUIDs, enhancing data-driven recommendations, piloting the product, and implementing a training and change management plan.

<iframe src="/assets/projects/fundraiser_db/CSposter.pdf" width="100%" height="550px"></iframe>

<a href="/assets/projects/fundraiser_db/CSposter.pdf" target="_blank" class="button">View Full Project Poster (PDF)</a>

This work is part of a two-paper series.
In the <a href="https://arxiv.org/abs/1704.01190" target="_blank">first paper</a> we introduce the methodology and main theoretical results and
in the <a href="{{ '/assets/publications/2017_detecting_network_effects/paper.pdf' | prepend: site.baseurl }}" target="_blank">second paper</a> we present implementation guidelines for using the methodology on large-scale experimentation platforms.

**Illustration of the proposed experimental design for detecting network effects.** <br/>
{%
	include image_with_caption.html
	url="/assets/projects/2016_network-ab/main.png"
	width="100%"
%}
**(A)** Graph of all units and the connections between them; the dashed circles represent (equally-sized) clusters. <br/>
**(B)** Assigning clusters to treatment arms: completely randomized (CR) and cluster-based randomized assignment (CBR). <br/>
**(C)** Assigning units to treatment buckets---treatment and control---using the corresponding strategy. <br/>
**(D)** Computing the treatment effect within each treatment arm: $$\hat \mu_{cr}$$ and $$\hat \mu_{cbr}$$, and variance: $$\hat \sigma^2_{cr}$$ and $$\hat \sigma^2_{cbr}$$. <br/>
**(E)** Computing the difference of the estimates from each treatment arm: $$\Delta = \hat \mu_{cr} - \hat \mu_{cbr}$$, and the total variance: $$\hat \sigma^2 = \hat \sigma^2_{cr} + \hat \sigma^2_{cbr}$$. <br/>

**Short video describing the work. Recorded for KDD'17.** <br/>
<iframe width="560" height="315" src="https://www.youtube.com/embed/E3yiKJCgLE4" frameborder="0" allowfullscreen></iframe>
