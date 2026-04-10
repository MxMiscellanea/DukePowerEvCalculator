# Duke Energy EV Plan Calculator

A browser-based tool that compares Duke Energy's **RES (Residential)** plan against the **EV Overnight** plan using your actual usage data. Everything runs locally in your browser — your data never leaves your computer.

**Try it now:** [Here](https://mxmiscellanea.github.io/DukePowerEvCalculator/)

## Background

Duke Energy offers an [EV Overnight Advantage](https://www.duke-energy.com/home/billing/ev-overnight-advantage) rate plan for customers who own or lease an electric vehicle. Instead of the standard residential tiered rate, EV Overnight gives you a discount on all electricity used between **11 PM and 5 AM EPT** — ideal for overnight EV charging.

The trade-off is that the standard (non-discount) rate on EV Overnight is slightly higher than the RES plan. Whether you come out ahead depends on how much of your usage falls in those nighttime hours. This tool does that math for you using your real meter data.

This applies to both [Duke Energy Progress](https://www.duke-energy.com/-/media/pdfs/for-your-home/rates/dep-nc/leaf-no-504-schedule-r-tou-ev.pdf?rev=074cc2a2ec734b1d9bb8f589369b5b73) and [Duke Energy Carolinas](https://www.duke-energy.com/-/media/pdfs/for-your-home/rates/electric-nc/ncschedulert-ev.pdf).

## Rate Comparison

| | Standard Rate | Discount Rate (11 PM - 5 AM) |
|---|---|---|
| **RES** | 12.623¢/kWh (first 800 kWh, Oct-Apr) | N/A |
| | 11.623¢/kWh (additional kWh, Oct-Apr) | |
| | 12.623¢/kWh (all kWh, May-Sep) | |
| **EV Overnight** | 13.096¢/kWh | 6.548¢/kWh |

Even without an EV, the overnight discount on normal usage can save ~$60/year. With an EV adding ~400 kWh/month of night charging, savings jump to ~$350/year.

## How to Sign Up for EV Overnight

1. Go to the [EV Overnight enrollment page](https://www.duke-energy.com/info/unindexed/rates/enroll-ev-overnight-advantage)
2. Invitation code `001` (now optional)
3. You'll get a confirmation email — the rate begins within one or two billing cycles

Note: The plan is limited to the first 20,000 customers who sign up, and Duke isn't heavily marketing it.

Also worth checking: Duke offers a [Charger Prep Credit](https://www.duke-energy.com/home/products/ev-complete/charger-prep-credit) that covers breaker upgrades, conduit, wiring, and outlet installation (not the charger itself or permits).

## How to Use the Calculator

1. **Download your usage data** from Duke Energy:
   - Log into [Energy Usage](https://p-auth.duke-energy.com/my-account/energy-usage)
   - Scroll down and click the 'Download my Data' green button.

2. **Open the calculator** [Here](https://mxmiscellanea.github.io/DukePowerEvCalculator/)

3. **Drag and drop** your XML file onto the page (or click to browse)

4. **View your results** — the tool automatically analyzes the last 12 full months of 15-minute interval data and shows:
   - Monthly cost breakdown under each plan
   - Which plan saves you money and by how much
   - A second scenario modeling EV charging

## EV Charging Scenarios

The calculator includes two modes for modeling EV charging impact:

- **Add New Usage** — Adds extra kWh per month (all at night). Use this if you're considering getting an EV and want to see how the added charging would affect your bill.

- **Shift Existing Usage** — If you already have an EV and charged during the day last year, this mode simulates moving that charging to nighttime hours. An additional slider lets you control what percentage of the kWh to shift (since you may already do some night charging).

## Privacy

All processing happens entirely in your browser using JavaScript. Your usage data is never uploaded to any server.

## License

Apache 2.0
