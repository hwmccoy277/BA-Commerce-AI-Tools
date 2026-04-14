# BA-Commerce-AI-Tools

# Triple Whale MCP — Marketer's Guide

**Ask questions about your store's performance directly in Claude. No dashboards, no spreadsheets — just answers.**

Connect your Triple Whale data to Claude and get instant answers about revenue, ad performance, customers, creatives, and more — just by asking in plain English.

---

## What It Can Do

### 📊 Business Health
The big picture — revenue, profit, and overall performance.

Get a full snapshot of how your business is performing: revenue, orders, average order value, ad spend, profit margin, and blended ROAS. Compare any two time periods side by side to see exactly what changed and by how much.

**Example prompts:**
- *"Give me a business health summary for Sunny Within for the last 30 days."*
- *"How did The Fidget Games perform this month compared to last month? Show me revenue, orders, and ad spend."*
- *"Compare Q1 this year vs Q1 last year for FOCL — revenue, ROAS, and profit."*

`tw_get_business_summary` · `tw_get_period_comparison`

---

### 📣 Ad Performance
Channel, campaign, and ad set level — how your paid media is working.

See how each channel is performing (Facebook, Google, TikTok, etc.), drill into campaigns, and go all the way down to individual Facebook ads with new customer revenue and NC ROAS per ad. All numbers use Triple Whale's attribution — more accurate than what the platforms self-report.

**Example prompts:**
- *"How are Facebook and Google performing for Stars & Honey this month? Compare spend, ROAS, and CPA."*
- *"Show me the top 10 campaigns by spend for FOCL in the last 30 days."*
- *"Which Facebook ads are driving the most new customer revenue for Stars & Honey this month? Sort by NC ROAS."*
- *"Show me every Facebook ad for FOCL with its NC CPA — which ones are actually acquiring new customers efficiently?"*

`tw_get_channel_performance` · `tw_get_campaign_performance` · `tw_get_ad_spend_overview` · `tw_get_ad_set_performance` · `tw_get_facebook_ad_performance`

---

### 🎨 Creative Intelligence
Which ads are working, which are tired, and what format wins.

Find your best-performing creatives by ROAS, CTR, or revenue. Spot ads that are losing steam before they drain budget. Compare how different formats perform — video vs image, or Facebook vs TikTok.

**Example prompts:**
- *"What are the top 5 creatives by ROAS for Sophie Grace on Facebook in the last 30 days?"*
- *"Are any of our creatives showing signs of fatigue for Stars & Honey? Check the last 60 days."*
- *"Do videos or images perform better for FOCL on TikTok?"*

`tw_get_creative_performance` · `tw_get_creative_trends` · `tw_get_creative_comparison`

---

### 👥 Customer Insights
Who's buying, who's coming back, and what they're spending.

Understand the new vs returning customer split, track acquisition cost, see which products drive the most revenue, and analyse whether customers acquired months ago are still buying. Also covers revenue trends over time, repeat purchase intervals, and geographic breakdowns.

**Example prompts:**
- *"What's the new vs returning customer split for The Fidget Games this month? And what's our CAC?"*
- *"Show me revenue trend week by week for FOCL in the last 90 days — are we growing or plateauing?"*
- *"What percentage of Stars & Honey customers buy again? How many days on average between their first and second order?"*
- *"Which countries and US states are driving the most revenue for Sophie Grace this month?"*

`tw_get_customer_metrics` · `tw_get_revenue_breakdown` · `tw_get_cohort_analysis` · `tw_get_revenue_trends` · `tw_get_repurchase_analysis` · `tw_get_geographic_breakdown`

---

### 🏷️ Discounts & Promotions
Which codes are working — and who's actually using them.

See which discount codes are pulling their weight: revenue driven, orders placed, and average discount amount. Find out whether codes are bringing in new customers or just rewarding people who would have bought anyway. Compare AOV for discounted vs full-price orders.

**Example prompts:**
- *"Which discount codes drove the most revenue for FOCL this month?"*
- *"What's the average order value for customers using a discount vs paying full price for Stars & Honey?"*
- *"Are our discount codes bringing in new customers or mostly being used by people who'd have bought anyway for Sunny Within?"*

`tw_get_discount_performance`

---

### 🔄 Subscription Business
MRR, churn, subscriber retention, and which products drive recurring revenue.

Track monthly recurring revenue, see how many subscribers you're gaining and losing, understand churn trends over time, and find out which products have the healthiest subscription retention.

**Example prompts:**
- *"Give me a subscription health overview for FOCL — MRR, active subscribers, and churn rate."*
- *"How has churn trended month by month for Stars & Honey over the last 6 months?"*
- *"Which products have the highest subscription churn for FOCL?"*

`tw_get_subscription_overview` · `tw_get_subscription_trends` · `tw_get_subscription_cohorts` · `tw_get_subscription_product_performance`

---

### 📦 Amazon Advertising
Sponsored Products, Brands, and Display performance by campaign and product.

See how your Amazon ad campaigns are performing. Drill into individual products (ASINs) to see which ones are profitable and which aren't pulling their weight.

**Example prompts:**
- *"Show me Amazon campaign performance for The Fidget Games this month — sorted by ROAS."*
- *"Which Sponsored Products campaigns have the worst ACoS for Sophie Grace?"*
- *"What's the ad-attributed revenue by product (ASIN) for FOCL in the last 30 days?"*

`tw_get_amazon_ad_campaigns` · `tw_get_amazon_product_performance`

---

### 🔍 Attribution & Tracking
Where sales really come from — the full customer journey.

Understand the difference between what platforms claim they drove vs what Triple Whale actually measured. See the full sequence of touchpoints that led to a purchase, and track how spend and ROAS are trending over time.

**Example prompts:**
- *"How does Triple Whale's ROAS compare to what Facebook is reporting for Sunny Within this month?"*
- *"Show me the customer journey breakdown for FOCL — what touchpoints are customers hitting before they buy?"*
- *"Compare first-click vs last-click attribution for Sophie Grace — which channels look different?"*

`tw_get_attribution_comparison` · `tw_get_customer_journeys` · `tw_get_spend_trends`

---

### 🌐 Website & Funnel
Where visitors drop off — and which pages and channels drive real traffic.

See exactly how many visitors make it from your site all the way through to a purchase, and where the biggest drop-offs happen. Find your highest-traffic landing pages and understand session quality by channel: bounce rate, pages per session, and time on site.

**Example prompts:**
- *"Show me the conversion funnel for Stars & Honey this month — how many sessions turn into add-to-carts, checkouts, and purchases?"*
- *"Which landing pages are getting the most traffic for FOCL in the last 30 days?"*
- *"What's our bounce rate by channel for Sophie Grace? Which channels bring the most engaged visitors?"*
- *"Where are people dropping off in the checkout funnel for Sunny Within? Compare Facebook vs Google traffic."*

`tw_get_conversion_funnel` · `tw_get_top_pages` · `tw_get_web_sessions`

---

### 🚨 Alerts & Monitoring
Catch underperforming channels and wasted spend before it adds up.

Run a quick health check across all your channels. Flags any channel with ROAS below 1.0 (losing money) or channels spending money but getting zero conversions. You can also set custom thresholds for any metric.

**Example prompts:**
- *"Are any channels losing money for Sunny Within this month?"*
- *"Check for any channels with ROAS below 2 for The Fidget Games in the last 30 days."*
- *"Run a full performance health check for Stars & Honey — flag anything with CPA over $50."*

`tw_get_metric_alerts`

---

## How To Use It

You don't need special commands or technical knowledge. Just talk to Claude like you'd talk to an analyst.

### Vague vs specific — the difference it makes

| ❌ Too vague | ✅ Much better |
|---|---|
| "How are ads doing?" | "How are Facebook and Google ads performing for Sunny Within this month? Show me ROAS and CPA." |
| "Show me customers" | "What's the new vs returning customer split for The Fidget Games in the last 30 days?" |
| "Check creatives" | "Are any of our TikTok creatives showing fatigue for FOCL in the last 60 days?" |
| "How's revenue?" | "How did Sophie Grace's revenue compare this month vs last month?" |
| "Check Facebook" | "Show me which Facebook ads are driving the most new customer revenue for [store] this month, sorted by NC ROAS." |
| "How's the website?" | "Show me the conversion funnel for [store] this month — where are visitors dropping off between landing and purchase?" |

### 8 tips that make a real difference

1. **Always name the store.** If you have multiple stores set up, Claude needs to know which one you mean.
2. **Always include a time period.** "This month", "last 30 days", "Q1", "year to date" — without one, Claude defaults to the last 30 days.
3. **Start broad, then drill down.** Ask for a business summary first. See something interesting? Ask: "Can you break that down by channel?" Claude remembers the whole conversation.
4. **Compare periods whenever possible.** A number on its own tells you less than a number vs last month. Comparisons surface problems and wins you'd otherwise miss.
5. **Trust Triple Whale's ROAS over platform ROAS.** Facebook and Google both claim credit for more sales than they actually drove. TW's pixel tracks the full picture.
6. **Check for creative fatigue weekly.** Ads naturally wear out. Make it a standing part of your weekly review before deciding on budget changes.
7. **Use alerts as your Monday morning check-in.** Ask "are any channels losing money this week?" at the start of each week — it takes 10 seconds.
8. **Use NC ROAS to find your real growth ads.** Overall ROAS includes returning customers who'd have bought anyway. NC ROAS tells you which ads are actually growing your customer base. An ad with great overall ROAS but terrible NC ROAS is mostly just retargeting people who already know you.

---

## Getting Started

### Requirements
- [Claude Desktop](https://claude.ai/download)
- Triple Whale API key (Settings → API Keys in your TW dashboard)
- Node.js 18+
- Your Shopify store domain(s)

### Installation

**1. Clone the repo and build**
```bash
git clone https://github.com/your-org/tw-mcp.git
cd tw-mcp
npm install
npm run build
```

**2. Find your Claude Desktop config file**
- **Mac:** `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`

**3. Add Triple Whale to the config**
```json
{
  "mcpServers": {
    "triple-whale": {
      "command": "node",
      "args": ["/absolute/path/to/tw-mcp/dist/index.js"],
      "env": {
        "TRIPLE_WHALE_API_KEY": "your-api-key-here",
        "TRIPLE_WHALE_SHOPS": "mystore.myshopify.com:My Store Name"
      }
    }
  }
}
```

**Multiple stores:**
```
"TRIPLE_WHALE_SHOPS": "store1.myshopify.com:Store One,store2.myshopify.com:Store Two"
```

**4. Restart Claude Desktop**

Fully quit Claude Desktop (right-click the icon → Quit) and reopen it.

**5. Test it**

Open a new chat and ask: *"What shops do I have configured?"*

If everything worked, Claude will list your stores.

---

## Complete Tool List

| Tool | What it does |
|---|---|
| `tw_get_business_summary` | Revenue, orders, AOV, spend, ROAS, profit snapshot |
| `tw_get_period_comparison` | Side-by-side comparison of any two date ranges |
| `tw_get_channel_performance` | Performance by ad channel (Facebook, Google, TikTok, etc.) |
| `tw_get_campaign_performance` | Performance by campaign |
| `tw_get_ad_spend_overview` | Spend and attribution overview with NC metrics by channel |
| `tw_get_ad_set_performance` | Performance by ad set |
| `tw_get_facebook_ad_performance` | Per-ad breakdown with NC Revenue, NC ROAS, NC CPA |
| `tw_get_creative_performance` | Creative performance by asset |
| `tw_get_creative_trends` | Creative fatigue and trend detection |
| `tw_get_creative_comparison` | Compare creatives across formats or channels |
| `tw_get_facebook_creative_report` | Facebook-specific creative report |
| `tw_get_customer_metrics` | New vs returning, CAC, LTV |
| `tw_get_revenue_breakdown` | Revenue by product, variant, or category |
| `tw_get_cohort_analysis` | Retention by acquisition cohort |
| `tw_get_revenue_trends` | Revenue and orders over time (daily/weekly/monthly) |
| `tw_get_repurchase_analysis` | Repeat purchase rate and time between orders |
| `tw_get_geographic_breakdown` | Revenue and orders by country and state |
| `tw_get_discount_performance` | Discount code performance — revenue, AOV, new vs returning |
| `tw_get_subscription_overview` | MRR, active subscribers, churn rate |
| `tw_get_subscription_trends` | Subscription metrics over time |
| `tw_get_subscription_cohorts` | Subscriber retention by signup cohort |
| `tw_get_subscription_product_performance` | Churn and retention by product |
| `tw_get_amazon_ad_campaigns` | Amazon Sponsored Ads by campaign |
| `tw_get_amazon_product_performance` | Amazon ad performance by ASIN |
| `tw_get_attribution_comparison` | TW vs platform-reported attribution |
| `tw_get_customer_journeys` | Touchpoint sequences before purchase |
| `tw_get_spend_trends` | Spend and ROAS over time |
| `tw_get_conversion_funnel` | Sessions → ATC → checkout → purchase funnel |
| `tw_get_top_pages` | Top landing pages by traffic |
| `tw_get_web_sessions` | Session quality by channel — bounce rate, duration |
| `tw_get_metric_alerts` | Flag underperforming channels and wasted spend |
| `tw_get_available_shops` | List configured shops |
