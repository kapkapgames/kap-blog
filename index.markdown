---
title: The Collection
layout: default
permalink: /

hero_image: "assets/images/blue_skies.jpg"
---

<h1 class="text-4xl">Latest News</h1>

<hr class="my-4">

<div class="grid grid-cols-1 lg:grid-cols-2 text-amber-100 gap-4">
    {% for post in site.posts %}
        <a href="{{ post.url | relative_url }}" class="min-h-100 p-4">
            <img src="" alt="blog_img" class="">
        </a>
    {% endfor %}
</div>

<h1 class="text-4xl">Oddities</h1>

<hr class="my-4">

<div class="grid grid-cols-1 lg:grid-cols-3 text-amber-100 gap-4">
    {% for post in site.posts %}
        <a href="{{ post.url | relative_url }}" class="min-h-100 p-4">
            <img src="" alt="blog_img" class="">
        </a>
    {% endfor %}
</div>

<!-- <a href="{{ post.url | relative_url }}" class="block p-6 bg-zinc-800 rounded-xl hover:bg-slate-700 transition">
    <h3 class="text-xl font-semibold text-white">{{ post.title }}</h3>
    <p class="text-slate-400 text-sm">{{ post.date | date_to_string }}</p>
</a> -->