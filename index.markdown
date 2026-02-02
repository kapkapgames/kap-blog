---
layout: default
---

<div class="bg-slate-900 rounded-3xl p-12 mb-12 border border-slate-800">
    <h1 class="text-4xl font-bold">Current Project: <span class="text-cyan-400">Project Neon</span></h1>
    <p class="mt-4 text-slate-400">Status: In Alpha. Currently working on enemy AI and lighting systems.</p>
</div>

<h2 class="text-2xl font-bold mb-6">Recent Posts</h2>
<div class="grid gap-6">
    {% for post in site.posts %}
        <a href="{{ post.url | relative_url }}" class="block p-6 bg-slate-800 rounded-xl hover:bg-slate-700 transition">
            <h3 class="text-xl font-semibold text-white">{{ post.title }}</h3>
            <p class="text-slate-400 text-sm">{{ post.date | date_to_string }}</p>
        </a>
    {% endfor %}
</div>