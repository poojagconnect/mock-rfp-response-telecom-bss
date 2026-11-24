# Executive Summary, Assumptions and Risks
Response to the SkyBridge Mobile India RFP (fictional). Written by Pooja G Madlimath as a learning exercise. The vendor is a generic cloud BSS product.

## Summary
SkyBridge runs an old billing system and several separate CRM tools. Launching a new plan takes 8 to 10 weeks. The company wants to launch plans in days, add 5G plans and start enterprise IoT services.

We propose one cloud BSS that covers CRM, product catalog, order management, charging and billing, linked through TM Forum APIs. SkyBridge would then have one customer record, one catalog and one bill across prepaid, postpaid and enterprise.

Of the 16 requirements, 12 are fully met, 3 are partly met and 1 is on the roadmap (the optional 5G slicing item). The rollout takes 12 months in four phases: design, build, migrate in groups, and cut over with extra support.

## Assumptions
1. SkyBridge gives us clean subscriber and balance data within the first 3 months.
2. The network and payment partners offer standard interfaces we can connect to.
3. SkyBridge's tax advisers confirm the GST and e-invoicing setup.
4. Subscribers move in groups, starting with a small pilot.
5. SkyBridge names one business owner and one technical lead who can decide quickly.
6. Pricing is not covered in this exercise.

## Risks
| Risk | Impact | What we would do |
|------|--------|------------------|
| Legacy data is messy and delays migration | High | Audit data early, clean it in months 1 to 3, run trial migrations |
| Downtime when prepaid customers move | High | Move in groups, run old and new in parallel, keep a rollback plan |
| Legacy network integration is harder than expected | Medium | Test the integration early, use an API gateway |
| Tax or data rules change during the project | Medium | Keep tax rules configurable, offer India-region hosting |
| Staff are slow to adopt the new system | Medium | Role-based training, super-users, extra support after go-live |

## Questions I would ask SkyBridge
1. How many old systems have to be retired, and what format is their data in?
2. What is the busiest hour of usage, in events per second?
3. Do enterprise customers have special billing terms in their contracts?
4. Can subscriber data go on public cloud, or does it need an India-region or private setup?
5. Which 5G and IoT services launch first?
