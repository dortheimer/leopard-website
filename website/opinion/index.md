---
title: Opinions
layout: default
---
<!--== Start Page Header Area ==-->
<div class="page-header-area bg-img" data-bg="assets/img/page-header.jpg">
    <div class="container">
        <div class="row">
            <div class="col-lg-10 col-xl-8 m-auto text-center">
                <div class="page-header-content-inner">
                    <div class="page-header-content">
                        <h2>FROM BUSINEX LATEST</h2>
                        <p>Businex always try to provide the best Business Solutions for Clinets
                            to grow up their Business very sharply and smoothly.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End Page Header Area ==-->

<!--== Start Blog Page Area Wrapper ==-->
<div class="blog-page-content-area sp-y">
    <div class="container">
        <div class="row">
            <div class="col-12">
                <div class="blog-content-wrapper">
                    <div class="row mtn-30">
                        {% for post in site.posts %}
                        <div class="col-md-6 col-lg-4">
                            <div class="blog-item">
                                <figure class="blog-thumb">
                                    <a href="{{ post.url }}"><img src="{{ post.image }}" alt="Businex-Blog" /></a>
                                </figure>
                                <div class="blog-content">
                                    <h2 class="h5"><a href="{{ post.url }}">{{ post.title }}</a></h2>
                                    <p>{{ post.excerpts }}</p>
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

                <div class="pagination-wrap">
                    <ul class="pagination">
                        <li class="prev"><a href="#"><i class="fa fa-long-arrow-left"></i> Previous</a></li>
                        <li><a href="#">1</a></li>
                        <li><a href="#">2</a></li>
                        <li><a href="#">3</a></li>
                        <li class="next"><a href="#">Next <i class="fa fa-long-arrow-right"></i></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>
<!--== End Blog Page Area Wrapper ==-->