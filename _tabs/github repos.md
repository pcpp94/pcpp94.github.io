---
layout: page
icon: fa-brands fa-github
order: 2
---

### Only showing public repositories

<div id="post-list" class="flex-grow-1 px-xl-1">
  {% for repo in site.github.public_repositories %}
  <article class="card-wrapper card">
    <a href="{{ repo.html_url }}" target="_blank" class="post-preview row g-0 flex-md-row-reverse">
      <div class="col-md-12">
        <div class="card-body">
          <h1 class="card-title my-2 mt-md-0">{{ repo.name }}</h1>
          <div class="card-text content mt-0 mb-3">
            <p>{{ repo.description }}</p>
          </div>
        </div>
      </div>
    </a>
  </article>
  {% endfor %}
</div>
