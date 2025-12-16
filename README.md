# SocialWeb Embed

Embed a social profile preview of Ghost SocialWeb notes on any site

```html
<iframe 
    id="socialweb-embed"
    data-site="blog.alcove.news"
    data-color="light"
    data-twitter="https://x.com/alcovenews"
    data-bluesky="https://bsky.app/profile/alcove.blog"
    style="width: 100%; max-width: 600px; height: 600px; border: none; display: block; border-radius: 21px;"
    scrolling="no"
    allow="clipboard-write"
></iframe>
<script>!function(){var e=document.getElementById("socialweb-embed"),d=e.dataset,p=new URLSearchParams({site:d.site||"",color:d.color||"light",twitter:d.twitter||"",bluesky:d.bluesky||""});e.src="https://johnonolan.github.io/socialweb-embed/?"+p;window.addEventListener("message",function(m){m.data&&m.data.type==="socialweb-embed-height"&&(e.style.height=m.data.height+"px")})}();</script>
```

### Parameters

- **Site** - [your_ghost_url]
- **Color** light, dark
- **Twitter** - link to your twitter profile (optional)
- **Bluesky** - link to your bluesky profile (optional)