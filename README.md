# tweety
Reverse Engineered Twitter Frontend API. (Still Maintained)

> **Important Maintenance & Temporary Service Notice**
> 
> Due to work commitments, updates to **tweety** are currently too slow. 
> 
> If you need a fully working, stable solution for `logging in to you Twitter Account and Get Cookies` right now, you can use the hosted service built for this purpose:
> 🌐 **[XAuth Web Service](https://www.77kays.xyz/xauth/ui/)** *(Note: This is a paid solution)*
> 
> **Want to speed up the open-source maintenance process?**  
> Consider supporting the project on ☕ **[Buy Me a Coffee](https://buymeacoffee.com/mahrtayyab)** to help prioritize updates!

[![Downloads](https://static.pepy.tech/personalized-badge/tweety-ns?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/tweety-ns) [![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/mahrtayyab/tweety)

## Installation: 
```bash
pip install tweety-ns
```

## Keep synced with latest fixes

##### **Pip might not be always updated , so to keep everything synced.**

```bash
pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade 
```

---
## 💖 Sponsors

<table>
  <tr>
    <td align="center">
      <a href="https://www.coreclaw.com/?utm_source=github&utm_medium=referral&utm_campaign=x.&utm_term=&utm_id=x" target="_blank">
        <img src="https://mahrtayyab.github.io/coreclaw.jpeg" alt="CoreClaw" width="100%" />
      </a>
    </td>
  </tr>
  <tr>
    <td>
      <h3><a href="https://www.coreclaw.com/?utm_source=github&utm_medium=referral&utm_campaign=x.&utm_term=&utm_id=x">CoreClaw</a> — Scraping Tool for Developers</h3>
      <p>Turns Twitter, Amazon, TikTok, Google Maps, Instagram & 100+ more sites into clean, structured data.</p>
      <p>It's ready for your leads, dashboards, or API. No maintenance. No broken scrapers. Just clean data, on demand.</p>
      <p>
        <a href="https://www.coreclaw.com/?utm_source=github&utm_medium=referral&utm_campaign=x.&utm_term=&utm_id=x">
          👉 <b>Start Free Trial on CoreClaw</b>
        </a>
      </p>
    </td>
  </tr>
</table>


## A Quick Example:
```python
    from tweety import TwitterAsync
    import asyncio
    
    async def main():
    
        app = TwitterAsync("session")  
        all_tweets = await app.get_tweets("elonmusk")
        for tweet in all_tweets:
            print(tweet)

    asyncio.run(main())
```

> [!IMPORTANT] 
> Even Twitter Web Client has a lot of rate limits now, Abusing tweety can lead to `read_only` Twitter account.

Do check [FAQs](https://github.com/mahrtayyab/tweety/wiki/FAQs)

Full Documentation and Changelogs are [here](https://mahrtayyab.github.io/tweety_docs/)
