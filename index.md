## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/izrchen/blog/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.


<h2>{{ page.title }}</h2>

<p>最新文章</p>

<ul>

　{% for post in site.posts %}

　　　<li>{{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>

　{% endfor %}

</ul>
