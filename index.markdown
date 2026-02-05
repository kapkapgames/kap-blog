---
title: The Collection
layout: default
permalink: /

hero_image: "assets/images/blue_skies.jpg"
---

<h1 class="text-4xl">Latest News</h1>

<hr class="my-8">

<div class="grid grid-cols-1 lg:grid-cols-2 text-amber-100 gap-4">
    {% for post in site.posts %}
        <a href="{{ post.url | relative_url }}" class="flex flex-col border-2 border-amber-100 h-100 lg:max-h-100">
            <img src="{{ '/assets/images/blue_skies.jpg' | relative_url }}" alt="blog_img" class="object-cover max-h-2/3 w-full">

            <article class="flex flex-col bg-amber-100 text-zinc-900 max-h-1/3 w-full p-4">
                <h3 class="text-2xl font-bold">{{ post.title }}</h3>
                <p class="line-clamp-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias obcaecati voluptate quo delectus praesentium nam aut quos suscipit eveniet fugit repellendus fuga officia, debitis perspiciatis voluptas a minus nobis vitae.</p>
            </article>
        </a>
    {% endfor %}
</div>

<h1 class="text-4xl mt-20">Oddities</h1>

<hr class="my-8">

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