# SocialWeb Embed

Embed a social profile preview of Ghost SocialWeb notes on any site


### Demo

https://codepen.io/JohnONolan/pen/qEZzPvQ?editors=1000

<img width="2450" height="1634" alt="CleanShot 2025-12-17 at 03 18 48@2x" src="https://github.com/user-attachments/assets/01e33581-8e82-4a32-8412-0ede42becfad" />


### Embed

```html
<iframe 
    id="socialweb-embed"
    data-site="blog.alcove.news"
    data-posts="3"
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

- **Site** - [your_ghost_url] (required)
- **Posts** - How many recent notes to show (default: 3)
- **Color** light, dark (default: light)
- **Twitter** - link to your twitter profile (optional)
- **Bluesky** - link to your bluesky profile (optional)


### Customizing & self-hosting

It's just an HTML page that runs on GitHub pages. Fork this repo, deploy main branch to GitHub pages, and modify however you like.

---

Copyright (c) 2025 John O'Nolan - Released under the [MIT license](LICENSE).
