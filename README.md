# Los Angeles NVMe VPS: Is SixtyNet Worth $200/Year, Which Plan Fits, and What the $3–$8 Alternatives Leave Out (Full Plan Table)

SixtyNet's cheapest Los Angeles NVMe plan is LAX-STARTER: 2 cores, 2 GB RAM, 40 GB NVMe and 5 TB of traffic for $200 a year, about $16.67 a month. That is two to five times what a 2 GB Los Angeles box costs at the budget end of this market, so the specs are not what you're paying for. The premium covers a single LA location with China-facing routing, residential IP options and DDoS-protected bandwidth, sold on annual terms. Below is every plan the company lists, the restrictions that decide whether you can use it at all, and the cases where a $7 plan from another host is the smarter purchase.

> **Quick pick**
>
> - Public site, API or game backend with some Asian traffic: **LAX-STARTER at $200/year** (2 cores, 2 GB, 40 GB NVMe, 5 TB, DDoS protection). 👉 [See the LAX-STARTER annual price](https://sixtynet.net/aff.php?aff=39)
> - Scraping, ad verification or social accounts that need a residential IP: **Residential-STARTER at $260/year**. Ports 80 and 443 stay closed, so this cannot serve a website.
> - Announcing your own IP space over China Unicom: the **$2,500/year AS9929 plan**. It is a BGP and transit product, not a web host.

## Every SixtyNet Los Angeles plan in one table

All four LAX plans carry DDoS protection and run on the same 2G to 10G premium network tiers. Prices below are the annual figures shown on the plan page, with the pre-discount price in brackets.

| Plan | Cores / RAM | NVMe (IOPS) | Traffic / uplink | Annual price | Order |
| --- | --- | --- | --- | --- | --- |
| LAX-STARTER | 2 / 2 GB | 40 GB (12,500) | 5 TB / 2G premium | $200 ($240, save 17%) | [Order LAX-STARTER](https://sixtynet.net/aff.php?aff=39) |
| LAX-MICRO | 4 / 4 GB | 80 GB (12,500) | 10 TB / 4G premium | $400 ($480, save 17%) | [Order LAX-MICRO](https://sixtynet.net/aff.php?aff=39) |
| LAX-MEDIUM | 8 / 8 GB | 160 GB (25,000) | 20 TB / 10G premium | $800 ($960, save 17%) | [Order LAX-MEDIUM](https://sixtynet.net/aff.php?aff=39) |
| LAX-LARGE | 8 / 16 GB | 320 GB (25,000) | 40 TB / 10G premium | $1,600 ($1,920, save 17%) | [Order LAX-LARGE](https://sixtynet.net/aff.php?aff=39) |
| Residential-STARTER | 2 / 2 GB | 40 GB (12,500) | 5 TB / 2G premium, residential IP | $260 ($300, save 13%) | [Order Residential-STARTER](https://sixtynet.net/aff.php?aff=39) |
| Los Angeles China Unicom-Premium | BGP/transit plan | — | 100M base, 3x burst, 95th percentile billing | $2,500 ($3,000, save 17%) | [Order the AS9929 plan](https://sixtynet.net/aff.php?aff=39) |

The residential line continues above STARTER with an 8 core / 8 GB / 160 GB / 20 TB tier and a 16 core / 16 GB / 320 GB / 40 TB tier. There are also AS9929 residential variants at 2 cores / 2 GB / 40 GB / 5 TB and 4 cores / 4 GB / 80 GB / 10 TB. Those four are not quoted in the same price block as the plans above, so confirm the current annual figure on the order page before you commit to one.

## What the fee covers, and the three restrictions that decide the purchase

The LAX line is the straightforward product. Each plan lists DDoS protection, NVMe storage with a stated IOPS figure, a premium network tier and a traffic allowance that runs from 5 TB to 40 TB. If you want a Los Angeles box to serve a website, an API or a game backend, LAX-STARTER is the entry point and the only question is whether 2 GB is enough for your stack.

Residential plans are a different product with a hard block. The listing states that residential IP products do not open ports 80 and 443 because of IP risk control. That kills public web hosting outright: no HTTP, no HTTPS, no Let's Encrypt renewal over the standard ports. Residential IPs are for outbound traffic where a datacenter IP gets flagged, such as marketplaces, ad verification or account management.

The AS9929 residential variants go further and reject all external probes and scans. Access is restricted unless you configure it, and only whitelisted or port-forwarded devices get in. Refunds on those specific products are issued as website balance, not back to your card. The plan listings don't spell out a general refund window for the LAX or standard residential plans, so get that in writing from support before paying, since annual billing means a lot of money sits with the host up front.

## A 2 GB LA box costs $7 elsewhere. Where does the other $9 go?

Four hosts sell a 2 GB Los Angeles NVMe plan in the same $7 to $8 monthly band. SixtyNet's equivalent is $200 a year, or roughly $16.67 a month, and it is billed annually rather than monthly.

| Provider / plan | vCPU / RAM | NVMe | Traffic | Price |
| --- | --- | --- | --- | --- |
| Cloudzy us-lax-1, 2 GB | 1 EPYC / 2 GB DDR5 | 60 GB | 3 TB | $7.48/mo (list $14.95, 50% off) |
| ExtraVM, 2 GB | 1 core / 2 GB | 30 GB | 5 TB | $8.00/mo |
| OliveVPS Pro | 1 vCPU / 2 GB DDR4 | 60 GB | 3 TB | $7.99/mo |
| Fusiora Starter | 1 vCore Ryzen 9 9950X / 2 GB DDR5 | 20 GB Gen5 | 5 TB | €2.75/mo listed, €2.47/mo paying in crypto |
| SixtyNet LAX-STARTER | 2 cores / 2 GB | 40 GB | 5 TB | $200/yr, about $16.67/mo |

The spread inside that band is the useful part. At the same 2 GB of RAM, NVMe allocation runs from 20 GB on Fusiora's Starter to 60 GB on Cloudzy and OliveVPS, and traffic from 3 TB to 5 TB. ExtraVM bundles Anti-DDoS at $8.00 and lists its LA hardware as AMD Ryzen 9 and EPYC on a product page that states port speed as "up to 10 Gbps," while its plan table shows 1 Gbps on the 2 GB tier. Fusiora runs every plan on a shared 1 Gbps uplink and prices in euros with a separate crypto rate. Cloudzy includes a dedicated IPv4 plus IPv6 and a 14-day money-back window on the 2 GB plan. OliveVPS sells Windows only from its $7.99 Pro plan upward; its $3.99 Starter is Linux-only.

What none of them sell is China Unicom premium routing or a residential IP. That is the whole case for paying SixtyNet roughly double, and it only holds if one of those two things is on your requirement list.

## Why Los Angeles, and what the latency actually looks like

Los Angeles is the main US landing point for trans-Pacific submarine cables, which is why every host in this market sells it as the Asia-facing US location. Published benchmarks from providers in this segment put Tokyo at roughly 110 to 150 ms, Singapore at 160 to 180 ms, the US West at 5 to 30 ms and the US East at 60 to 80 ms. OliveVPS publishes a similar set from its own LA facility: 1 to 3 ms locally, about 108 ms to Tokyo, 138 ms to London, 150 ms to Sydney.

Those figures come from other hosts' published tests. SixtyNet's plan page sells routing, not milliseconds: AS9929, free BGP session setup, a 100M base rate with 3x burst, 95th percentile billing. Treat any LA provider's Asia numbers as a starting point and test the actual path from your users before you migrate anything.

## The AS9929 plan is not a VPS

China Unicom's AS9929 is a premium China-facing route, and SixtyNet's China Unicom-Premium product at $2,500 a year is built around it: free BGP session setup, limited BGP technical support, 100M base network with 3x burst and 95th percentile billing, plus discounts for quarterly and annual payment. That bundle describes a transit and peering arrangement for someone with their own IP space and a router, not a server you SSH into and install WordPress on. If you arrived from a search for a cheap LA NVMe box, this plan is one tier of product above what you need.

## Who should skip SixtyNet

- **A personal site, blog or staging box.** At $16.67 a month effective for the cheapest LAX plan, you are paying for routing you probably won't use. Cloudzy, ExtraVM, OliveVPS and Fusiora all sell 2 GB in the $7 to $8 range with monthly billing.
- **Anyone who needs monthly terms to start.** Prices here are quoted annually, and a host you have not tested is an expensive thing to prepay for twelve months.
- **Public web hosting on a residential IP.** Ports 80 and 443 are closed by design.
- **Teams that need multiple regions.** SixtyNet lists one location, Los Angeles. Confirm the exact facility with support if Tier certification matters to your compliance review.

## FAQ

**Can I host a website on a residential plan?** No. Ports 80 and 443 are closed on residential IP products because of IP risk control. Use the LAX plans for anything public-facing.

**Is DDoS protection extra?** The four LAX plans list DDoS protection as part of the plan, with no separate line item shown. Residential plans list a residential IP and traffic instead. The AS9929 residential variants reject external probes and scans, and access is limited to whitelisted or port-forwarded devices.

**What happens if I want a refund?** For the AS9929 residential products, refunds are issued as website balance only. The LAX and standard residential listings don't state a refund window, so ask support to confirm one in writing before checkout.

**Do the plans come with traffic overage pricing?** The listings give a monthly traffic allowance (5 TB to 40 TB) and don't publish an overage rate. Ask before you plan around heavy transfer.

**Is there a cheaper way in?** No. LAX-STARTER at $200 a year is the floor for the DDoS-protected LA line, and Residential-STARTER at $260 a year is the floor for a residential IP.

## How to decide

- Serving a site or API mostly to US West and some Asian users, and you want one LA box with DDoS filtering: **LAX-STARTER at $200/year**. Move to LAX-MICRO at $400/year if 2 GB of RAM won't hold your database and app process together.
- Need a residential IP for outbound traffic only: **Residential-STARTER at $260/year**, with ports 80 and 443 assumed unusable from day one.
- Running your own IP space and peering with China Unicom: the **$2,500/year AS9929 plan**, after a conversation with their BGP support about what "limited" covers.
- Want the cheapest competent 2 GB LA NVMe box with monthly billing: none of the above. Buy from the $7 to $8 tier and revisit SixtyNet when China routing or a residential IP becomes a real requirement.

Before you pay, confirm two things in writing: the refund window that applies to the plan you picked, and the monthly traffic overage rate. Both are missing from the plan listings, and both matter more on an annual prepay than they would on a monthly one.

👉 [Start with LAX-STARTER at $200/year](https://sixtynet.net/aff.php?aff=39)
