---
feature_text: |
  ## [ E R A D A S H ]
  Analyst programmer, TLM
feature_image: "https://picsum.photos/1300/400?image=989"
---

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%m-%d-%Y" }}">{{ post.date | date_to_long_string }}</time>
    <p>
    {{ post.description }}
    </p>
    <a href="{{ post.url }}">
            Learn more...
    </a>
  </article>
{% endfor %} 