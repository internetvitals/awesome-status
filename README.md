# Awesome Status [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of status pages, public APIs, monitoring tools, and open-source projects for tracking internet infrastructure health and service uptime.

Found something missing? [Open a PR](https://github.com/internetvitals/awesome-status/pulls) — contributions welcome.

---

## Contents

- [Internet Health Dashboards](#internet-health-dashboards)
- [Status Page Aggregators](#status-page-aggregators)
- [Official Status Pages](#official-status-pages)
- [Public APIs](#public-apis)
- [Open Source Tools](#open-source-tools)
- [Self-Hosted Status Pages](#self-hosted-status-pages)
- [Libraries & SDKs](#libraries--sdks)
- [Incident Management](#incident-management)
- [Browser Extensions](#browser-extensions)
- [Resources](#resources)

---

## Internet Health Dashboards

Real-time dashboards that aggregate multiple services into a single health view.

- **[InternetVitals](https://internetvitals.com)** — Monitors 41 backbone services (Cloudflare, AWS, Azure, GCP, GitHub, Stripe, DNS providers) and shows aggregated health as medical vital signs: pulse, temperature, blood pressure, SpO2. Free public API + MCP server for AI agents.
- **[Internet Health Report](https://ihr.iijlab.net)** — IIJ Lab's academic project tracking BGP routing health and latency across the global internet.
- **[ThousandEyes Internet Insights](https://www.thousandeyes.com/internet-insights/)** — Enterprise-grade visibility into internet outages and ISP disruptions.
- **[Cloudflare Radar](https://radar.cloudflare.com)** — Real-time internet traffic trends, outages, and BGP route leaks from Cloudflare's global network.
- **[CAIDA Outage Detection](https://www.caida.org/projects/outages/)** — Academic research project detecting internet outages using telescope data.

---

## Status Page Aggregators

Services that monitor and aggregate status pages from multiple providers.

- **[StatusGator](https://statusgator.com)** — Aggregates 2,500+ official status pages into one dashboard. Paid, with free tier.
- **[Downdetector](https://downdetector.com)** — Crowdsourced outage reports for major consumer services. Free.
- **[IsDown](https://isdown.app)** — Monitors official status pages and sends alerts. Paid.
- **[OhDear](https://ohdear.app)** — Status page monitoring plus uptime, SSL, and broken links. Paid.
- **[StatusHub](https://statushub.com)** — Creates and monitors status pages. Paid.
- **[Saashub](https://www.saashub.com/check-website-status)** — Simple multi-site status checker.
- **[NextReset](https://nextreset.ai/)** — Independent Codex reset-history dashboard combining observed reset records with links to official service incidents. Free.


---

## Official Status Pages

Status pages for major internet backbone services. Most use [Atlassian Statuspage](https://www.atlassian.com/software/statuspage).

### Cloud Infrastructure
- [AWS Health Dashboard](https://health.aws.amazon.com/health/status) — Amazon Web Services
- [Azure Status](https://azure.status.microsoft) — Microsoft Azure
- [Google Cloud Status](https://status.cloud.google.com) — Google Cloud Platform
- [Cloudflare System Status](https://www.cloudflarestatus.com) — Cloudflare CDN, DNS, Workers
- [DigitalOcean Status](https://status.digitalocean.com) — DigitalOcean cloud
- [Fastly Status](https://www.fastlystatus.com) — Fastly CDN
- [Akamai Status](https://www.akamaistatus.com) — Akamai CDN

### Developer Tools
- [GitHub Status](https://www.githubstatus.com) — GitHub + Actions + Pages
- [npm Status](https://status.npmjs.org) — npm registry
- [Docker Hub Status](https://www.dockerstatus.com) — Docker Hub registry
- [Vercel Status](https://www.vercel-status.com) — Vercel edge network
- [Netlify Status](https://www.netlifystatus.com) — Netlify hosting
- [GitLab Status](https://status.gitlab.com) — GitLab CI/CD
- [Datadog Status](https://status.datadoghq.com) — Datadog monitoring
- [iGaming Tools Status](https://statuspage.i-gaming.tools) — iGaming Tools data platform, API and MCP server

### Payments
- [Stripe Status](https://status.stripe.com) — Stripe payments API
- [PayPal Status](https://www.paypalstatus.com) — PayPal
- [Shopify Status](https://www.shopifystatus.com) — Shopify commerce

### Communication
- [Slack Status](https://status.slack.com) — Slack messaging
- [Zoom Status](https://status.zoom.us) — Zoom video
- [Discord Status](https://discordstatus.com) — Discord
- [Twilio Status](https://status.twilio.com) — Twilio communications
- [SendGrid Status](https://status.sendgrid.com) — SendGrid email

### Auth & Identity
- [Okta Status](https://status.okta.com) — Okta / Auth0 identity
- [Apple System Status](https://www.apple.com/support/systemstatus/) — Apple services

---

## Public APIs

Free and open APIs for querying service status and internet health programmatically.

- **[InternetVitals API](https://internetvitals.com/developers)** — REST API + MCP server. Get internet health score, vitals, service status, incident history. No auth required. `GET https://internetvitals.com/api/v1/health`
- **[Statuspage.io API](https://developer.statuspage.io)** — Standard API used by most major services. `GET https://{subdomain}.statuspage.io/api/v2/status.json` — returns `{"status": {"indicator": "none|minor|major|critical"}}`
- **[Cloudflare Radar API](https://developers.cloudflare.com/radar/)** — Internet traffic, BGP, and attack trends. Free with Cloudflare account.
- **[AWS Health API](https://docs.aws.amazon.com/health/latest/ug/health-api.html)** — Requires AWS account. Real-time AWS service health events.
- **[Google Cloud Status JSON](https://status.cloud.google.com/incidents.json)** — Active GCP incidents, no auth required.
- **[Apple System Status JSON](https://www.apple.com/support/systemstatus/data/system_status_en_US.js)** — Apple services status as JSONP, no auth.

---

## Open Source Tools

Self-hostable and open source monitoring projects.

- **[Uptime Kuma](https://github.com/louislam/uptime-kuma)** ⭐50k+ — Self-hosted uptime monitor with beautiful UI. Docker-ready.
- **[Gatus](https://github.com/TwiN/gatus)** ⭐6k+ — Automated service health dashboard. Config-driven, Go-based.
- **[Cachet](https://github.com/cachethq/cachet)** ⭐14k+ — Open source status page system. PHP/Laravel.
- **[Freshping](https://github.com/freshworks/freshping)** — Website uptime monitoring.
- **[Upptime](https://github.com/upptime/upptime)** ⭐14k+ — GitHub Actions-powered uptime monitor. Uses GitHub Issues for incidents.
- **[Statping-ng](https://github.com/statping-ng/statping-ng)** — Status page for monitoring sites and apps. Go-based.
- **[HetrixTools](https://hetrixtools.com)** — Uptime and blacklist monitoring. Free tier available.
- **[OpenStatus](https://github.com/openstatushq/openstatus)** ⭐5k+ — Open source status page + API monitoring. Next.js + Cloudflare.

---

## Self-Hosted Status Pages

Platforms for building your own status page.

- **[Atlassian Statuspage](https://www.atlassian.com/software/statuspage)** — The industry standard. Used by GitHub, Cloudflare, Stripe, and most major SaaS.
- **[Instatus](https://instatus.com)** — Modern Statuspage alternative. Free tier.
- **[Freshstatus](https://www.freshworks.com/statuspage/)** — Simple status page builder.
- **[Cstate](https://github.com/cstate/cstate)** — Hugo-based static status page.
- **[Hund](https://hund.io)** — Status page with subscriber management.

---

## Libraries & SDKs

Client libraries for working with status APIs.

- **[internetvitals](https://www.npmjs.com/package/internetvitals)** — JavaScript/TypeScript SDK for the InternetVitals API. `npm install internetvitals`
- **[statuspage-js](https://github.com/jloh/statuspage)** — Parse Statuspage.io JSON API in JavaScript.
- **[python-statuspage](https://github.com/domaindrivendev/python-statuspage)** — Python client for Statuspage.io API.

---

## Incident Management

Tools for managing and communicating during outages.

- **[PagerDuty](https://www.pagerduty.com)** — Industry-standard incident response and on-call management.
- **[OpsGenie](https://www.atlassian.com/software/opsgenie)** — Alerting and on-call management by Atlassian.
- **[FireHydrant](https://firehydrant.com)** — Incident management with automated runbooks.
- **[Rootly](https://rootly.com)** — Slack-native incident management.
- **[Incident.io](https://incident.io)** — Modern incident management platform.
- **[Better Uptime](https://betteruptime.com)** — On-call scheduling + status page + uptime monitoring.

---

## Browser Extensions

- **[Is it down?](https://chrome.google.com/webstore/detail/is-it-down/)** — Quick check if a site is down for everyone.
- **[StatusBar](https://chrome.google.com/webstore/detail/statusbar/)** — Shows service status in browser toolbar.

---

## Resources

### Articles
- [How Cloudflare publishes its system status](https://blog.cloudflare.com/how-cloudflare-publishes-system-status/)
- [AWS approach to service health communication](https://aws.amazon.com/blogs/mt/building-better-status-pages/)
- [Building a status page that people actually trust](https://www.atlassian.com/blog/statuspage/building-a-status-page)

### Standards & Protocols
- [Statuspage.io API Docs](https://developer.statuspage.io) — De facto standard for status page APIs
- [MCP (Model Context Protocol)](https://modelcontextprotocol.io) — Open standard for AI agent tool integrations

### Communities
- [r/sre](https://reddit.com/r/sre) — Site Reliability Engineering community
- [r/devops](https://reddit.com/r/devops) — DevOps community
- [SRE Weekly Newsletter](https://sreweekly.com) — Weekly roundup of reliability engineering

---

## Contributing

Contributions welcome! Please:

1. Check that the link works and the project is actively maintained
2. Add a short description (one sentence)
3. Place it in the right category
4. Keep alphabetical order within sections
5. Open a pull request

For new categories — open an issue first to discuss.

---

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Andrii Tkachenko](https://x.com/tkachenko) has waived all copyright and related rights to this work.
