# Simple-SRE-Uptime-Monitor-Golang-

```markdown
# 🔧 Simple SRE Uptime Monitor (Golang)

A lightweight Site Reliability Engineering (SRE) tool built in **Golang** to monitor service uptime, log failures, and send alerts. Designed for learning and experimentation with reliability principles, automation, and observability.



## 🚀 Features

- ✅ Periodic health checks for configured endpoints  
- 📉 Logs response times and failure rates  
- 🔔 Slack alert integration for downtime notifications  
- 🐳 Dockerized for easy deployment  
- 🔄 CI/CD pipeline using GitHub Actions



## 📦 Tech Stack

- **Language**: Golang  
- **Containerization**: Docker  
- **CI/CD**: GitHub Actions  
- **Alerting**: Slack Webhooks  
- **Logging**: Local file-based logs (can be extended to ELK or Prometheus)


```
## ⚙️ Setup Instructions

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-username/sre-uptime-monitor.git
   cd sre-uptime-monitor
   

2. **Configure endpoints**
   - Edit `config.json` to add the URLs you want to monitor.

3. **Set up Slack alerts**
   - Add your Slack webhook URL in `config.json`.

4. **Build and run**
   ```bash
   go build -o monitor
   ./monitor
   ```

5. **Docker (optional)**
   ```bash
   docker build -t sre-monitor .
   docker run -d sre-monitor
   ```

---

## 📈 Sample Output

```
[2025-09-17 10:00:01] Health check passed: https://example.com (200 OK)
[2025-09-17 10:05:01] Health check failed: https://example.com (Timeout)
[2025-09-17 10:05:02] Slack alert sent for https://example.com
```

---

## 🧠 Lessons Learned

- Golang’s concurrency model makes multi-endpoint monitoring efficient and clean.
- Automating alerts and logging is key to proactive reliability.
- Even simple tools can teach powerful principles of uptime and observability.

---

## 📌 Future Improvements

- Add Prometheus metrics endpoint  
- Integrate with Grafana dashboards  
- Retry logic and exponential backoff  
- Email alerting option  
- Extend to support HTTPS certificate expiry checks

---

## 🤝 Contributing

Pull requests are welcome! If you have ideas for improving reliability, automation, or observability, feel free to fork and submit a PR.

---

## 📜 License

MIT License

---

## 🙌 Acknowledgments

Inspired by real-world SRE practices and the need for hands-on learning through building.

```

