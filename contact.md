---
ref: contact
lang: en
permalink: /contact/
title: "Get in touch."
eyebrow: "Contact"
lead: "We're in Madrid and Seoul and reply in English, Spanish or Korean, usually within two business days."
description: "Contact Lococo: brand partnerships, press, investors and general inquiries."
no_cta: true
---

<div class="contact-grid">
<div class="card">
<h3>Brand partnerships</h3>
<p>Retail in Spain, creator campaigns, pop-ups.</p>
<a href="mailto:{{ site.data.site.email_partners }}?subject=Partnership%20inquiry%20-%20Lococo">{{ site.data.site.email_partners }}</a>
</div>
<div class="card">
<h3>Press</h3>
<p>Interviews, materials, event coverage.</p>
<a href="mailto:{{ site.data.site.email_press }}?subject=Press%20inquiry%20-%20Lococo">{{ site.data.site.email_press }}</a>
</div>
<div class="card">
<h3>Investors and careers</h3>
<p>We're a small team and always happy to meet people who care about K-beauty in Europe.</p>
<a href="mailto:{{ site.data.site.email_general }}?subject=Hello%20Lococo">{{ site.data.site.email_general }}</a>
</div>
<div class="card">
<h3>Customers</h3>
<p>Orders, shipping and returns are handled by our store team.</p>
<a href="{{ site.data.site.shop_url }}/pages/contact" target="_blank" rel="noopener">lococo.beauty help</a>
</div>
</div>

## Where we are

{% for e in site.data.site.entities %}
**{{ e.name }}**  
{{ e.address }}

{% endfor %}

Instagram [{{ site.data.site.instagram_handle }}]({{ site.data.site.instagram }})
