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
                    <h2>CREATING VALUE</h2>
                    <p>
                        <strong>Leopard Asset Management</strong> is an emerging investment platform focused on value. We are opportunistic and seek value in various corners of the market
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End About Area Wrapper ==-->

<!--== Start Service Area Wrapper ==-->
<div class="service-area-wrapper sm-top-wt">
    <div class="service-area-top parallax" style="background:#080b1a">
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
                <div class="col-sm-6">
                    <div class="service-item">
                        <!-- Start Service Item -->
                        <h5>Leopard Global Equity</h5>
                        <p>Leopard Global Equity is a long-short Cayman Island-based hedge fund, focused on investments in corners of the markets in which we see long-term value</p>
                    </div>
                </div>
                <div class="col-sm-6">
                    <div class="service-item">
                        <h5>Leopard Real Estate</h5>
                        <p>Long-only Cayman Island-based hedge fund. The fund aims to generate excess returns over its benchmark by investing in a combination of value and growth real estate companies. The fund holds a concentrated portfolio of European-listed real estate companies and asset managers</p>
                        <!-- End Service Item -->
                    </div>
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
                    <h2 class="mb-0">Insights </h2>
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
                            <a href="{{ post.url }}">{{ post.date |  date: "%b %d, %y" }}</a>
                        </div>
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</div>
<!--== End Blog Area Wrapper ==-->
