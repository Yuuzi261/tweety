# tweety
Reverse Engineered Twitter Frontend API. (Still Maintained)

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

## 💖 Sponsors

<a href="https://www.swiftproxy.net/?ref=tweety">
  <img src="https://mahrtayyab.github.io/swift.png" alt="Swiftproxy" width="640">
</a>

### **[Swiftproxy](https://www.swiftproxy.net/?ref=tweety)**
> Premium residential proxies for X (Twitter) automation, web scraping, and browser automation. Access 80M+ residential IPs across 190+ countries with rotating and sticky sessions, non-expiring traffic, and support for HTTP, HTTPS, and SOCKS5. 

> * 🎁 **Free Trial Available**
> * 🏷️ **10% OFF** with coupon code: `PROXY90`

<br clear="left"/>

---

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
