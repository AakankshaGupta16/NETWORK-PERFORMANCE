# NETWORK-SPEED-AND-PERFORMANCE-LOGGING
# 🌐 Network Performance Monitoring using Wireshark & Python

This project presents a comparative analysis of **Wi-Fi vs. Cellular (4G/5G) network performance** using a hybrid approach of **active speed benchmarking** and **protocol-level packet inspection**. It automates real-time data collection and visualizes insights into latency, throughput, signal stability, and handoff behavior.

---

## 🚀 Key Features

- ✅ **Active Performance Logging**:  
  Benchmarks download/upload speed and ping using `speedtest-cli` at regular intervals via Python automation.

- ✅ **Protocol-Level Analysis**:  
  Captures and inspects real traffic using **Wireshark**, analyzing protocols like **TCP**, **TLS**, **SSDP**, and **MDNS** to detect congestion, drops, and transition delays.

- ✅ **Visualization & Insights**:  
  Plots bandwidth metrics, jitter, and packet anomalies using **Matplotlib** in **Google Colab**, highlighting transition irregularities and network instability.

---

## 🛠️ Tools & Technologies

- **Python**  
- **Speedtest CLI**  
- **Wireshark**  
- **Matplotlib / Pandas**  
- **Google Colab**

---


---

## 📊 Sample Visualizations

<p align="center">
  <img src="images/ping_variation.png" width="400"/>
  <br>
  <em>Ping variation across network types (Wi-Fi vs 4G)</em>
</p>

<p align="center">
  <img src="images/jitter_plot.png" width="400"/>
  <br>
  <em>Jitter analysis from time-series logs</em>
</p>

---

## 🔬 Real-World Use Case Context

This project evaluates how modern wireless networks behave in **latency-sensitive scenarios** like video conferencing, online gaming, and live streaming.  
By combining speed metrics with **deep traffic inspection**, it uncovers how and when networks break under load, handoffs, or noise.

---

## 📌 How to Run

1. Clone this repo and open the notebooks in [Google Colab](https://colab.research.google.com/)
2. For active testing:
3. For packet analysis:
- Use **Wireshark** to capture `.pcap` files
- Export as `.csv` or use tshark for parsing
4. Run visualizations using Matplotlib

---

## 👩‍💻 Author

**Aakanksha**  
ECE Undergraduate | Interested in Deep Learning · Embedded Systems · Network Intelligence  
📧 gupta.aakanksha2003@gmail.com | 🌐 [[LinkedIn Profile]](https://www.linkedin.com/in/aakanksha-gupta-b32b9b24b/) 

---

## 📝 License

This project is open-sourced for academic and research purposes. Contributions are welcome!



