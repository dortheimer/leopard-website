---
title: Team
layout: default
---
<!--== Start Page Header Area ==-->
<div class="page-header-area bg-img" >
    <div class="container">
        <div class="row">
            <div class="col-lg-10 col-xl-8 m-auto text-center">
                <div class="page-header-content-inner">
                    <div class="page-header-content">
                        <h2>TEAM</h2>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End Page Header Area ==-->

<!--== Start Team Area Wrapper ==-->
<div class="team-page-area-wrapper sp-y ">
    <div class="container">
        <div class="row mtn-30">
            {% for staff_member in site.staff_members %}
            <div class="col-sm-6 col-lg-3">
                <div class="team-mem-item">
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