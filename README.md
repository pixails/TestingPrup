# TestingPrup

A testing and demo repository focused on web performance analysis and reporting for the fictional web application **Speedy**.

## 📋 Project Overview

**TestingPrup** is a proof-of-concept project that simulates a performance testing suite for a multi-page web application. Its main goal is to demonstrate how Core Web Vitals and load metrics can be collected, analyzed, and visualized over time in a rich HTML report.

> **Note:** All data, URLs, and product references in this project are **fictional** and exist solely for demo/presentation purposes.

---

## 🚀 Product: Speedy

**Speedy** is a simulated web application with **20 pages**, each featuring unique functionality. The performance of each page is tracked across **100 test executions**, providing historical trend analysis.

### Pages

| # | Page | Description |
|---|------|-------------|
| 1 | Home | Landing page and main entry point |
| 2 | Dashboard | User activity and stats overview |
| 3 | Search | Product/content search engine |
| 4 | Catalog | Product listing and filters |
| 5 | Product Detail | Individual product information |
| 6 | Cart | Shopping cart management |
| 7 | Checkout | Order placement flow |
| 8 | Payment | Payment processing page |
| 9 | Order Confirmation | Post-purchase summary |
| 10 | User Profile | Account settings and preferences |
| 11 | Order History | Past orders and tracking |
| 12 | Notifications | System alerts and messages |
| 13 | Settings | App configuration panel |
| 14 | Help Center | FAQs and support resources |
| 15 | Blog | Articles and content feed |
| 16 | About | Company and team information |
| 17 | Contact | Contact form and map |
| 18 | Login | Authentication page |
| 19 | Register | New user registration |
| 20 | 404 Error | Not found / error page |

---

## 📊 Performance Metrics

The following **Core Web Vitals** and additional metrics are tracked per page per execution:

### Core Web Vitals

| Metric | Full Name | Description | Good Threshold |
|--------|-----------|-------------|----------------|
| **LCP** | Largest Contentful Paint | Time until the largest visible content is rendered | ≤ 2.5 s |
| **CLS** | Cumulative Layout Shift | Measure of unexpected layout shifts | ≤ 0.1 |
| **FID** | First Input Delay | Time from first interaction to browser response | ≤ 100 ms |
| **INP** | Interaction to Next Paint | Responsiveness to user interactions | ≤ 200 ms |
| **FCP** | First Contentful Paint | Time until the first content element is painted | ≤ 1.8 s |
| **TTFB** | Time to First Byte | Server response latency | ≤ 800 ms |

### Additional Metrics

| Metric | Description |
|--------|-------------|
| **Total Blocking Time (TBT)** | Sum of long task blocking time |
| **Speed Index** | Visual page load progression speed |
| **Page Weight** | Total transferred bytes (JS, CSS, images, fonts) |
| **Concurrent Users** | Simultaneous users during the test run |
| **Error Rate** | % of requests that resulted in errors |
| **Requests Count** | Total HTTP requests per page load |

---

## 📈 Historical Test Data

- **100 test executions** recorded over time
- Each execution captures metrics for all 20 pages
- Concurrent user load is recorded per run to evaluate **load balancer behavior**
- Charts visualize performance trends and correlate load levels with degradation

### Load Testing Scenarios

| Scenario | Concurrent Users | Purpose |
|----------|-----------------|---------|
| Baseline | 10 | Normal traffic baseline |
| Low Load | 50 | Light usage simulation |
| Medium Load | 200 | Typical peak hours |
| High Load | 500 | Stress test |
| Spike | 1000 | Traffic spike simulation |

---

## 📁 Project Structure

```
TestingPrup/
├── README.md          # Project documentation
└── reports/           # Generated HTML performance reports
    └── performance-report.html
```

---

## 🛠️ Reports

The HTML performance report includes:

- **Summary dashboard** with overall scores per page
- **Core Web Vitals** breakdown per page and per execution
- **Trend charts** showing performance evolution across 100 runs
- **Load correlation charts** linking concurrent user count with metric degradation
- **Interactive filters** by page, metric, and date range
- **Color-coded indicators** (Good / Needs Improvement / Poor) per Web Vitals threshold

---

## 🤝 Contributing

This is a demo project. Contributions, suggestions, and feedback are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is for demo and educational purposes only. All data is fictional.
