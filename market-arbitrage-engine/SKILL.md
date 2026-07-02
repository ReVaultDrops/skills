# Skill: Market Arbitrage Engine
> Professional-grade arbitrage monitoring for sneakers and collectibles across StockX, GOAT, and eBay.

# Market Arbitrage Engine
Professional-grade arbitrage monitoring for sneakers and collectibles across StockX, GOAT, and eBay.

## Capabilities
- **Cross-Platform Price Mapping**: Real-time comparison of "Lowest Ask" on one platform vs. "Highest Bid" on another.
- **Fee-Adjusted Profit Engine**: Automatically calculates net profit after platform commissions (GOAT 9.5%, StockX 8-10%, eBay 12.9%) and estimated shipping.
- **Instant-Flip Alerts**: Identifies "Bid/Ask Overlaps" where you can buy on one platform and immediately sell into an existing bid on another.
- **Global Floor Tracking**: Monitors regional price differences (US vs EU vs Asia) to identify cross-border arbitrage opportunities.

## Robust Workflow
1. **Input**: Style code (e.g., "DZ5485-612") and size.
2. **Fetch**: Pull real-time data from StockX, GOAT, and eBay APIs.
3. **Calculate**: 
   - `Potential Profit = (Target Bid * (1 - Fee)) - (Source Ask + Shipping)`.
   - `ROI % = (Profit / Total Cost) * 100`.
4. **Report**: Structured list of opportunities ranked by ROI and liquidity.

## Error Handling
- **Size Discrepancy**: Normalizes US/UK/EU sizing to prevent incorrect price comparisons.
- **Condition Guard**: Filters out "Used" or "Defects" listings to ensure apples-to-apples comparisons for DS (Deadstock) pairs.