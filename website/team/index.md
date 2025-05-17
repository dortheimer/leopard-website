---
title: Team
layout: default
---

<!--== Start About Area Wrapper ==-->
<div class="about-area-wrapper sm-top">
    <div class="container">
        <div class="row align-items-lg-center">
            <div class="col-md-6 col-lg-7 order-1">
                <div class="about-content ml-0">
                    <h6>Our Team</h6>
                    <h2>Meet Our Team</h2>
                    <p>
                        At <strong>Leopard Asset Management</strong>, our experienced team is dedicated to delivering exceptional investment solutions for our clients. 
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End About Area Wrapper ==-->

<!--== Start Team Area Wrapper ==-->
<div class="team-page-area-wrapper bg-offwhite sp-y sm-top">
    <div class="container">
        <div class="row mtn-30">
            {% for staff_member in site.staff_members %}
            <div class="col-sm-6 col-lg-3">
                <div class="team-mem-item">
                    <figure class="member-pic">
                        <img src="{{ staff_member.image }}" alt="{{ staff_member.name }}" />
                    </figure>
                    <div class="member-info">
                        <h5><a href="{{ staff_member.url }}" class="stretched-link">{{ staff_member.title }}</a></h5>
                        <span class="designation">{{ staff_member.position }}</span>
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</div>
<!--== End Team Area Wrapper ==-->