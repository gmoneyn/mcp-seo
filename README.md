# mcp-seo

SEO toolkit as an MCP server. Analyze meta tags, robots.txt, sitemaps, keyword density, readability, and heading structure from any AI assistant that supports MCP.

## Install

Add to your MCP client config (Claude, Cursor, etc.):

```json
{
  "mcpServers": {
    "mcp-seo": {
      "command": "npx",
      "args": ["-y", "mcp-seo"]
    }
  }
}
```

## Tools

| Tool | Description |
|------|-------------|
| `meta_tags` | Analyze a page's SEO meta tags (title, description, OG, Twitter, canonical) |
| `robots_txt` | Parse robots.txt rules, sitemaps, and crawl directives |
| `sitemap_check` | Validate sitemap.xml format, URL count, and common issues |
| `keyword_density` | Keyword frequency analysis with single words, bigrams, and trigrams |
| `readability` | Flesch-Kincaid readability scoring with actionable tips |
| `heading_structure` | Heading hierarchy (H1-H6) analysis with structure validation |

## Example Prompts

- "Analyze the meta tags on https://example.com"
- "Check the robots.txt for example.com"
- "Validate the sitemap at https://example.com/sitemap.xml"
- "What's the keyword density of this text for 'machine learning'?"
- "Score this blog post for readability"
- "Check the heading structure of https://example.com/blog/post"

## License

MIT
