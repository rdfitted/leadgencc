# /leads_audit Command

Automated lead generation and outreach workflow for AI Audit service.

## Usage
```
/leads_audit [profession] [location] [count]
```

## Parameters
- `profession`: Target profession/role (e.g., "lawyers", "dentists", "real estate agents")
- `location`: Target location (e.g., "Toronto", "Miami")  
- `count`: Number of leads (optional, defaults to 3)

## Example
```
/leads_audit lawyers Toronto 5
```

## Process
1. **LinkedIn Search**: Use LinkedIn MCP server to find specified number of leads with email addresses
   - MCP Server: `mcp__pd-linkedin__linkedin-search-organization` (for company searches)
   - MCP Server: `mcp__pd-linkedin__linkedin-get-multiple-member-profiles` (for lead profiles)
2. **Research Phase**: 
   - **News/Podcasts/Press**: Use Metaphor MCP server for recent developments
     - MCP Server: `mcp__pd-metaphor__metaphor-search`
   - **Company Updates**: Use Firecrawl MCP server for additional recent posts
     - MCP Server: `mcp__firecrawl__firecrawl_search`
3. **Email Drafting**: Use Gmail MCP server to create personalized email drafts
   - MCP Server: `mcp__pd-gmail__gmail-create-draft` (draft creation)
   - Include relevant recent developments found in research
   - Promote AI Audit: 20-30 minute voice agent interview
   - Highlight scored report of AI readiness and implementation recommendations
   - Service link: https://www.fittedaiautomation.com/

## Output
- Lead contact information from LinkedIn
- Research summary for each lead
- Personalized email drafts ready for sending