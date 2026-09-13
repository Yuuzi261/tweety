# tweety
Reverse Engineered Twitter Frontend API. (Still Maintained)

> **Important Maintenance & Temporary Service Notice**
> 
> Due to work commitments, updates to **tweety** are currently too slow. 
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
