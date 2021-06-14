---
layout: default
title: ScratchConvert - Convert Scratch Projects to .exe For Free!
description: All about how to convert Scratch Projects to Windows Programs, HTML5, and even Mobile Apps completely for free!
thumbnail: public/img/branding/thumbnail.png
permalink: /
---

<div class="page-header header-filter header-small" data-parallax="true" style="background-image: url('public/img/misc/header.jpg');">
    <div class="container">
        <div class="row">
            <div class="col-md-8 ml-auto mr-auto text-center">
                <h1 class="title">ScratchConvert</h1>
                <br />
            </div>
        </div>
    </div>
</div>
<div class="main main-raised">
    <div class="container">
        <div class="section section-text">
            <!-- Popular articles start -->
            <div class="row">
                <h3 class="title">Popular Articles</h3>

                <div class="row">
                    {% for post in site.posts %}
                        {% if post.featured == 1 or post.featured == 2 %}
                            <div class="col-md-6">
                                <div class="card card-raised card-background" style="background-image: url('{{ post.thumbnail | default: site.thumbnail }}">
                                    <div class="card-body">
                                        <h6 class="card-category text-info">{{ post.category }}</h6>
                                        <a href="https://scratchconvert.com{{ post.permalink }}">
                                            <h3 class="card-title">{{ post.title }}</h3>
                                        </a>
                                        <p class="card-description">
                                            {{ post.description }}
                                        </p>
                                        <a href="https://scratchconvert.com{{ post.permalink }}" class="btn btn-danger btn-round">
                                            <i class="material-icons">format_align_left</i> Read Article
                                            <div class="ripple-container"></div>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        {% endif %}

                        {% if post.featured == 3 %}
                            <div class="col-md-12">
                                <div class="card card-raised card-background" style="background-image: url('{{ post.thumbnail | default: site.thumbnail }}');">
                                    <div class="card-body">
                                        <h6 class="card-category text-info">{{ post.category }}</h6>
                                        <h3 class="card-title">{{ post.title }}</h3>
                                        <p class="card-description">
                                            {{ post.description }}
                                        </p>
                                        <a href="https://scratchconvert.com{{ post.permalink }}" class="btn btn-warning btn-round"> <i class="material-icons">subject</i> Read Article </a>
                                            <div class="ripple-container"></div>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        {% endif %}
                    {% endfor %}
                </div>
            </div>
            <!-- Popular articles end -->

            <!-- All articles start -->
            <div class="row">
                <h3 class="title">All Articles</h3>
                        
                <div class="row">
                    {% for post in site.posts %}
                        {% if post.featured == false %}
                            <div class="col-md-4">
                                <div class="card card-blog">
                                    <div class="card-header card-header-image">
                                        <a href="https://scratchconvert.com{{ post.permalink }}">
                                            <img src="{{ post.thumbnail | default: site.thumbnail }}" alt="{{ post.title }}" />
                                        </a>
                                        <div class="colored-shadow" style="background-image: url('{{ post.thumbnail | default: site.thumbnail }}'); opacity: 1;"></div>
                                    </div>
                                    <div class="card-body">
                                        <h6 class="card-category text-warning">{{ post.category }}</h6>

                                        <h4 class="card-title">
                                            <a href="https://scratchconvert.com{{ post.permalink }}">{{ post.title }}</a>
                                        </h4>

                                        <a href="https://scratchconvert.com{{ post.permalink }}" class="btn btn-warning btn-round"> <i class="material-icons">subject</i> Read Article </a><div class="ripple-container"></div>
                                    </div>
                                </div>
                            </div>
                        {% endif %}
                    {% endfor %}
                </div>
            </div>
            <!-- All articles end -->
        </div>
    </div>
</div>