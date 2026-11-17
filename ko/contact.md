---
ref: contact
lang: ko
permalink: /ko/contact/
title: "연락 주세요."
eyebrow: "문의"
lead: "마드리드와 서울에 있습니다. 한국어·영어·스페인어로, 보통 2영업일 안에 답합니다."
description: "Lococo 문의: 브랜드 파트너십, 언론, 투자·채용, 일반 문의."
no_cta: true
---

<div class="contact-grid">
<div class="card">
<h3>브랜드 파트너십</h3>
<p>스페인 판매, 크리에이터 캠페인, 팝업.</p>
<a href="mailto:{{ site.data.site.email_partners }}?subject=Partnership%20inquiry%20-%20Lococo">{{ site.data.site.email_partners }}</a>
</div>
<div class="card">
<h3>언론</h3>
<p>인터뷰, 자료, 행사 취재.</p>
<a href="mailto:{{ site.data.site.email_press }}?subject=Press%20inquiry%20-%20Lococo">{{ site.data.site.email_press }}</a>
</div>
<div class="card">
<h3>투자·채용</h3>
<p>작은 팀입니다. 유럽의 K-뷰티에 진심인 분이라면 언제든 만나고 싶습니다.</p>
<a href="mailto:{{ site.data.site.email_general }}?subject=Hello%20Lococo">{{ site.data.site.email_general }}</a>
</div>
<div class="card">
<h3>고객</h3>
<p>주문·배송·반품은 스토어 팀이 답합니다.</p>
<a href="{{ site.data.site.shop_url }}/pages/contact" target="_blank" rel="noopener">lococo.beauty 고객센터</a>
</div>
</div>

## 주소

{% for e in site.data.site.entities %}
**{{ e.name }}**  
{{ e.address }}

{% endfor %}

Instagram [{{ site.data.site.instagram_handle }}]({{ site.data.site.instagram }})
