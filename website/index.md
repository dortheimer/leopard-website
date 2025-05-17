---
title: Home
layout: default
---
<!--== Start About Area Wrapper ==-->
<div class="about-area-wrapper sm-top">
    <div class="container">
        <div class="row align-items-lg-center">
            <div class="col-md-12">
                <div class="about-content">
                    <h6>ABOUT US</h6>
                    <h2>CREATING VALUE</h2>
                    <span class="about-since">Since 2010</span>
                    <p>
                        <strong>Leopard Asset Management</strong> is an emerging investment platform focused on value. We are opportunistic and seek value in various corners of the market
                    </p>
                    <a href="/about/" class="btn-about">MORE DETAILS <i class="mdi mdi-chevron-double-right"></i></a>
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End About Area Wrapper ==-->
<!--== Start Feature Area Wrapper ==-->
<div class="feature-area-wrapper sm-top">
    <div class="container">
        <div class="row mtn-sm-60 mtn-md-5">
            <div class="col-md-4">
                <div class="icon-box-item">
                    <div class="icon-box__icon">
                        <i class="fa fa-globe fa-lg"></i>
                    </div>
                    <div class="icon-box__info">
                        <h5>Identify Theme</h5>
                        <p>The investment manager employs a theme-based approach, targeting structural inefficiencies and transformation opportunities across regions and sectors within the global small and mid-cap universe.</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="icon-box-item">
                    <div class="icon-box__icon">
                        <i class="fa fa-search fa-lg"></i>
                    </div>
                    <div class="icon-box__info">
                        <h5>Drivers of Inefficiencies</h5>
                        <p>Once a theme is identified, a top-down approach is applied to analyze the drivers of current market inefficiencies and to assess the catalysts expected to drive structural change.</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="icon-box-item">
                    <div class="icon-box__icon">
                        <i class="fa fa-bar-chart fa-lg"></i>
                    </div>
                    <div class="icon-box__info">
                        <h5>Realization Catalyst</h5>
                        <p>The investment manager assesses catalysts by analyzing macro, regulatory, and industry forces that may trigger structural change, then evaluating whether companies are positioned to benefit.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End Feature Area Wrapper ==-->
<!--== Start Service Area Wrapper ==-->
<div class="service-area-wrapper sm-top-wt">
    <div class="service-area-top parallax" style="background:#151515">
        <div class="container">
            <div class="row">
                <div class="col-lg-6 col-xl-5 m-auto text-center">
                    <div class="section-title section-title--light">
                        <h2 class="mb-0">OUR FUNDS</h2>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="service-content-area">
        <div class="container">
            <div class="row mtn-30">
                <div class="col-sm-4">
                    <!-- Start Service Item -->
                    <div class="service-item">
                        <figure class="service-thumb">
                            <!-- <a href="service-details.html"><img src="assets/img/service/fund2.avif" -->
                                    <!-- alt="Leopard-InvestmentStrategy" /></a> -->
                            <div class="service-txt">
                                <h5>Leopard Global Equity</h5>
                                <p>Leopard Global Equity is a long-short Cayman Island-based hedge fund, focused on investments in corners of the markets in which we see long-term value</p>
                            </div>
                        </figure>
                        <!-- <div class="service-content">
                            <div class="service-content-inner">
                                <h5><a href="service-details.html" class="stretched-link"></a>Leopard Global Equity</h5>
                                <p>A global, theme-based equity strategy targeting transformational opportunities.</p>
                            </div>
                        </div> -->
                    </div>
                    <!-- End Service Item -->
                </div>
                <div class="col-sm-4">
                    <!-- Start Service Item -->
                    <div class="service-item">
                        <div class="service-thumb">
                            <div class="service-txt">
                                <h5>Leopard Real Estate</h5>
                                <p>Long-only Cayman Island-based hedge fund. The fund aims to generate excess returns over its benchmark by investing in a combination of value and growth real estate companies. The fund holds a concentrated portfolio of European-listed real estate companies and asset managers.</p>
                            </div>
                        </div>
                    </div>
                    <!-- End Service Item -->
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End Service Area Wrapper ==-->


<!--== Start Blog Area Wrapper ==-->
<div class="blog-area-wrapper sm-top">
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <div class="section-title">
                    <h6>Insights</h6>
                    <h2 class="mb-0">Latest Insights <br>from the Property Market</h2>
                </div>
            </div>
        </div>
        <div class="row mtn-35">
            {% for post in site.posts %}
            <div class="col-md-6 col-lg-4">
                <div class="blog-item">
                    <div class="blog-content">
                        <h2 class="h5"><a href="{{ post.url }}">{{ post.title}}</a></h2>
                        <p>{{ post.excerpt }}</p>
                        <div class="blog-meta">
                            <a href="#">By: {{ post.author }}</a>
                            <a href="#">{{ post.date |  date: "%b %d, %y" }}</a>
                        </div>
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</div>
<!--== End Blog Area Wrapper ==-->

<!--== Start Team Area Wrapper ==-->
<div class="team-area-wrapper bg-img sp-y home-two-about-area" >
    <div class="container-fluid">
        <div class="row align-items-center">
            <div class="col-lg-4">
                <div class="section-title section-title--light mb-lg-0">
                    <h6>Team</h6>
                    <h2>The People <br>Behind Leopard</h2>
                </div>
            </div>
            <div class="col-lg-8">
                <div class="team-content-wrap slick-dots--light mtn-md-5">
                    {% for staff_member in site.staff_members %}
                    <div class="team-mem-item">
                        <div class="member-info">
                            <h5><a href="{{ staff_member.url }}" class="stretched-link">{{ staff_member.title }}</a></h5>
                            <p>{{ staff_member.position }}</p>
                        </div>
                    </div>
                    {% endfor %}
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End Team Area Wrapper ==-->