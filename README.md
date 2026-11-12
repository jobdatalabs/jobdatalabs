# jobdata labs

Small, reliable data tools that run on [Apify](https://apify.com/jobdata_labs). Pay only for results, schedule them, call them from your code, or give them to your AI agent over MCP.

Every tool uses official APIs or public, robots.txt-respecting sources. No logins, no personal data.

## Tools

| Tool | What it does | Run it |
|---|---|---|
| [SEO Audit Crawler](https://github.com/jobdatalabs/seo-audit-crawler) | Crawls a site and finds broken links, missing titles and meta descriptions, redirect chains and 20+ on-page issues, with an HTML report | [Apify](https://apify.com/jobdata_labs/seo-audit-crawler) |
| [Sitemap Change Monitor](https://github.com/jobdatalabs/sitemap-change-monitor) | Extracts every URL from XML sitemaps and reports new, updated and removed pages between runs | [Apify](https://apify.com/jobdata_labs/sitemap-change-monitor) |
| [RSS Feed Monitor](https://github.com/jobdatalabs/rss-feed-monitor) | RSS and Atom monitoring with "only new items" mode, keyword and date filters | [Apify](https://apify.com/jobdata_labs/rss-feed-monitor) |
| [Review Sentiment Analyzer](https://github.com/jobdatalabs/review-sentiment-analyzer) | Sentiment score, label, topics and defect flags for any review dataset, 5 languages, no LLM costs | [Apify](https://apify.com/jobdata_labs/review-sentiment-analyzer) |
| [AI Document Extractor](https://github.com/jobdatalabs/ai-document-extractor) | PDF, DOCX and TXT to clean Markdown with RAG-ready chunks | [Apify](https://apify.com/jobdata_labs/ai-document-extractor) |
| [Tech Stack & DNS Detector](https://github.com/jobdatalabs/tech-stack-dns-detector) | Website technologies plus email provider and SaaS tools from public DNS records | [Apify](https://apify.com/jobdata_labs/tech-stack-dns-detector) |
| [ATS Jobs Monitor](https://github.com/jobdatalabs/ats-jobs-monitor) | Job postings from official Greenhouse, Lever, Ashby, Workable, Personio and other ATS APIs, with new-jobs-only mode | [Apify](https://apify.com/jobdata_labs/ats-jobs-monitor) |
| [Hiring Signals](https://github.com/jobdatalabs/hiring-signals) | Hiring activity per company: open roles, new roles, departments and change since the last check | [Apify](https://apify.com/jobdata_labs/hiring-signals) |

## Use them from an AI agent (MCP)

```json
{
  "mcpServers": {
    "jobdata-labs": {
      "url": "https://mcp.apify.com?tools=jobdata_labs/seo-audit-crawler,jobdata_labs/sitemap-change-monitor,jobdata_labs/rss-feed-monitor,jobdata_labs/review-sentiment-analyzer,jobdata_labs/ai-document-extractor,jobdata_labs/tech-stack-dns-detector,jobdata_labs/ats-jobs-monitor,jobdata_labs/hiring-signals",
      "headers": { "Authorization": "Bearer <YOUR_APIFY_TOKEN>" }
    }
  }
}
```

Questions or feature requests: open an issue in the tool's repository.
