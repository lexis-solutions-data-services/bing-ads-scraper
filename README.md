# Microsoft Bing Ads Scraper

![banner](https://lexis-solutions-apify.fra1.cdn.digitaloceanspaces.com/banners/bing-ads.png)

## What is the Bing Ads Scraper?

## 📊 Actor Stats

| Stat | Value |
|------|-------|
| **Version** | `0.0.2` |
| **Last Update** | Dec 1, 2025 |

---



## 💻 Integration Examples

This repository includes example code showing how to integrate the `bing-ads-scraper` actor into your projects.

You can find example implementations in the [`examples/`](./examples) folder:
- **TypeScript/JavaScript**: See [`examples/typescript/`](./examples/typescript) for a complete TypeScript example
- **Python**: See [`examples/python/`](./examples/python) for a complete Python example

Each example includes:
- Ready-to-use code templates
- Setup instructions
- Documentation links

---



The Bing Ads Scraper is designed to extract data from Microsoft Ad Library. It enables users to gather information about ads displayed on Bing. The scraper can be used for competitor analysis, ad copy brainstorming, and more.

<p align="center">
  <img src="https://apify-image-uploads-prod.s3.us-east-1.amazonaws.com/rYbjZxrCaAR9K4Xax/FKRr6pN9JziydPak9-bing-logo.png" alt="Bing Ads Scraper" style="height: 60px; margin-right: 15px;" /><a href="https://apify.com/lexis-solutions/bing-ads-scraper" target="_blank">
    <img src="https://img.shields.io/badge/Try%20it%20on-Apify-0066FF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDA4IiBoZWlnaHQ9IjQwOCIgdmlld0JveD0iMCAwIDQwOCA0MDgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxnIGNsaXAtcGF0aD0idXJsKCNjbGlwMF8zNDFfNDE1NykiPgo8cGF0aCBkPSJNMjE4LjY5NSAxMDRIMzAwLjk3QzMwMi42NDMgMTA0IDMwNCAxMDUuMzU3IDMwNCAxMDcuMDNWMjMyLjc2NkMzMDQgMjM1Ljc3OCAzMDAuMDgzIDIzNi45NDUgMjk4LjQzNCAyMzQuNDI1TDIxNi4xNTkgMTA4LjY5QzIxNC44NDEgMTA2LjY3NCAyMTYuMjg3IDEwNCAyMTguNjk1IDEwNFoiIGZpbGw9IndoaXRlIi8+CjxwYXRoIGQ9Ik0xODkuMzA1IDEwNEgxMDcuMDNDMTA1LjM1NyAxMDQgMTA0IDEwNS4zNTcgMTA0IDEwNy4wM1YyMzIuNzY2QzEwNCAyMzUuNzc4IDEwNy45MTcgMjM2Ljk0NSAxMDkuNTY2IDIzNC40MjVMMTkxLjg0IDEwOC42OUMxOTMuMTU5IDEwNi42NzQgMTkxLjcxMyAxMDQgMTg5LjMwNSAxMDRaIiBmaWxsPSJ3aGl0ZSIvPgo8cGF0aCBkPSJNMjAyLjU5MSAyMDQuNjY4TDEwOS4xMjcgMjk4LjgzNUMxMDcuMjI5IDMwMC43NDcgMTA4LjU4MyAzMDQgMTExLjI3OCAzMDRIMjk2LjhDMjk5LjQ4MyAzMDQgMzAwLjg0MiAzMDAuNzcgMjk4Ljk2NyAyOTguODUyTDIwNi45MDggMjA0LjY4NUMyMDUuNzI2IDIwMy40NzUgMjAzLjc4MiAyMDMuNDY4IDIwMi41OTEgMjA0LjY2OFoiIGZpbGw9IndoaXRlIi8+CjwvZz4KPGRlZnM+CjxjbGlwUGF0aCBpZD0iY2xpcDBfMzQxXzQxNTciPgo8cmVjdCB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEwNCAxMDQpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==&logoColor=white" alt="Try it on Apify" style="border-radius: 12px; height: 60px;" />
  </a>
</p>


## What data can the Bing Ads Scraper extract?

The Bing Ads Scraper can extract the following data from the Microsoft Ad Library:

- Ad ID
- Ad text
- Ad impressions range
- Ad shown countries
- Impressions share by country (only EU countries)
- Advertiser name
- Advertiser ID

and more.

## What use cases does the Bing Ads Scraper have?

- Ad copy brainstorming and inspiration for your own ads 🧠
- Competitor analysis and benchmarking of your ads 📊
- Advertiser research and analysis 🕵️‍♀️

## How to use the Bing Ads Scraper

1. Create a free Apify account
2. Open Bing Ads Scraper
3. Add a query to the input field, this could be a company name, domain, or a search string that appears in the ad
4. Click Start and wait for the results
5. Download the results in JSON, XML or CSV format or connect the actor to your backend via API

## 📥 Input

To run the actor, you can input a:

- **Query** - A query to search for ads. This can be a company name, domain, or a search string that appears in the ad.

- **Advertiser ID** - An advertiser ID to search for ads. This can be found in the URL of the advertiser's page on Microsoft Ad Library.

Or _both_, in which case the actor will search for ads that match both the query and the advertiser ID.

## 📤 Output

The results are stored in the default dataset associated with the actor. Each item is an ad, having the following format:

```json
{
  "adId": 72568100319632,
  "adTitle": "Apify® - Apify.com - Official Website",
  "adDescription": "Build Reliable Web Scrapers in Minutes with Apify's User-Friendly Interface. Get Accurate Data Fast and Easy with Apify! Power Your Data-Driven Insights",
  "adDestination": "https://apify.com/",
  "advertiserId": 4294982386,
  "advertiserName": "Retainup Inc",
  "advertiserPaidForBy": null,
  "adStartDate": "2023-09-13",
  "adEndDate": "2023-10-01",
  "adImpressions": "<1K",
  "impressionsByCountry": [
    {
      "country": "Germany",
      "impressionShare": 49.5
    },
    {
      "country": "Croatia",
      "impressionShare": 14.7
    },
    {
      "country": "Lithuania",
      "impressionShare": 10.5
    },
    {
      "country": "Spain",
      "impressionShare": 5.3
    },
    {
      "country": "Italy",
      "impressionShare": 4.2
    },
    {
      "country": "Netherlands",
      "impressionShare": 4.2
    },
    {
      "country": "Romania",
      "impressionShare": 4.2
    },
    {
      "country": "France",
      "impressionShare": 3.2
    },
    {
      "country": "Finland",
      "impressionShare": 1.1
    },
    {
      "country": "Luxembourg",
      "impressionShare": 1.1
    },
    {
      "country": "Poland",
      "impressionShare": 1.1
    },
    {
      "country": "Cyprus",
      "impressionShare": 1.1
    }
  ],
  "targets": [
    {
      "targetType": "Location",
      "usedForExclusion": false
    }
  ]
}
```

## How many Bing Ads can the Bing Ads Scraper extract?

The Bing Ads Scraper uses pagination to extract all ads from the Microsoft Ad Library. The scraper can extract 24 ads per page, and 999 pages per search query. This means that the scraper can extract up to 23,976 ads per search query.

You can control the number of pages to scrape by setting the `maxPages` input parameter.

## Why use the Bing Ads Scraper?

- ⚡️ **Fast** - The scraper is fast and efficient, allowing you to scrape ads in a programmatic way.

- 🤙 **Easy to use** - The scraper is easy to use and requires no coding knowledge. All you need to do is input the query you want to scrape and the scraper will do the rest.

- ☑️ **Well-Maintained** - The scraper is maintained by the Lexis Solutions team, ensuring that it is always up-to-date and working properly.

## FAQ

- **How to find a company's ads on Bing?**

  To find a company's ads on Bing, you can use the Microsoft Ad Library. This tool allows you to search for ads by advertiser name, domain, or country.

- **How to search for ads on Bing?**

  Microsoft Ad Library allows you to search for ads by advertiser name, domain. You can also filter ads by date range and format. If you need to obtain the data programmatically, you can use the Bing Ads Scraper.

- **What is the Microsoft Ad Library?**

  The Microsoft Ad Library is a website that allows users to view ads that are displayed on Bing's advertising network. It also provides information about the advertisers who are running these ads.

- **What is the Bing Ads Scraper?**

  The Bing Ads Scraper is a web scraping tool designed specifically for Microsoft Ad Library. This tool offers an effective way to mine valuable data from ads displayed on Bing's advertising network.

- **Is Scraping Bing Ads Legal?**

  Scraping public information from Microsoft Ad Library is legal as long as you are not violating any terms of service or privacy policies. However, it is important to note that scraping ads can be considered a violation of the terms of service of some websites, so it is always best to check before scraping.

- **How much does it cost?**

  The cost for using the Bing Ads Scraper is shown on the top of this page. You can also check the Apify Store page for more information.

## Roadmap 🚴‍♀️

Currently the Bing Ads Scraper does not allow filtering by date range and countries. We plan to add these features in the future.

## Need to scrape ads from Google?

👉 Check out our [Google Ads Scraper](https://apify.com/lexis-solutions/google-ads-scraper)

## Need to scrape ads from TikTok?

👉 Check out our [TikTok Ads Scraper](https://apify.com/lexis-solutions/tiktok-ads-scraper)

---

👀 p.s.

Got feedback or need an extension?

Lexis Solutions is a [certified Apify Partner](https://apify.com/partners/find). We can help you with custom solutions or data extraction projects.

Contact us over [Email](mailto:scraping@lexis.solutions) or [LinkedIn](https://www.linkedin.com/company/lexis-solutions)

## Support Our Work 💝

If you're happy with our work and scrapers, you're welcome to leave us a company review [here](https://apify.com/partners/find/lexis-solutions/review) and leave a review for the scrapers you're subscribed to. It will take you less than a minute but it will mean a lot to us!

Image Credit: Microsoft Ad Library
