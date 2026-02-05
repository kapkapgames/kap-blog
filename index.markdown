---
layout: landing
---

<h2 class="text-2xl font-bold mb-6">Recent Posts</h2>
<div class="grid gap-6">
    {% for post in site.posts %}
        <a href="{{ post.url | relative_url }}" class="block p-6 bg-zinc-800 rounded-xl hover:bg-slate-700 transition">
            <h3 class="text-xl font-semibold text-white">{{ post.title }}</h3>
            <p class="text-slate-400 text-sm">{{ post.date | date_to_string }}</p>
        </a>
    {% endfor %}
</div>