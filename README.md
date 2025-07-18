# 🌐 Network Performance Monitoring using Wireshark & Python

A hybrid solution for **real-time network performance analysis**, comparing **Wi-Fi** and **Cellular (4G/5G)** connectivity. This project blends **active benchmarking** with **deep protocol-level inspection** to reveal how networks behave under real-world loads, handoffs, and instability.

---

## 🚀 Key Features

- ✅ **Active Speed Logging**  
  Automates benchmarking of download/upload speeds and ping latency using `speedtest-cli` at regular intervals.

- ✅ **Packet-Level Analysis with Wireshark**  
  Captures live traffic and analyzes key protocols including **TCP**, **TLS**, **SSDP**, and **MDNS** to detect:
  - Packet drops  
  - Latency spikes  
  - Handoff delays  

- ✅ **Insightful Visualizations**  
  Uses **Matplotlib** and **Pandas** (in **Google Colab**) to visualize:
  - Bandwidth trends  
  - Jitter and latency variability  
  - Protocol anomalies and signal transitions  

---

## 🛠️ Tools & Technologies

- Python  
- Speedtest CLI  
- Wireshark / Tshark  
- Matplotlib & Pandas  
- Google Colab  

---

## 🔬 Real-World Application

This project simulates conditions relevant to:

- 🎮 Online Gaming  
- 📹 Live Video Conferencing  
- 📡 Mobile Data Handoffs  

It helps **network engineers, researchers, and power users** understand how network behavior changes during load, noise, or mobility scenarios.

---

## 📌 How to Run

### 🧪 Active Performance Testing

1. Clone this repository  
2. Open the Jupyter or Colab notebook:  
   [Open in Google Colab](https://colab.research.google.com/)
3. Run the following commands to test your network:
   ```bash
   !pip install speedtest-cli
   !speedtest-cli
   ```

### 📥 Protocol-Level Packet Analysis

1. Use **Wireshark** to capture `.pcap` traffic logs while switching networks or performing tasks  
2. Export packet logs to `.csv` using Wireshark **or** extract with `tshark`:
   ```bash
   tshark -r capture.pcap -T fields -e frame.time -e ip.src -e ip.dst -e tcp.len -E separator=, > output.csv
   ```
3. Load `.csv` into the notebook for visualization:
   ```python
   import pandas as pd
   df = pd.read_csv('output.csv')
   ```

---

## 👩‍💻 Author

**Aakanksha Gupta**  
🎓 ECE Undergraduate | 💡 Passionate about Deep Learning, Embedded Systems, and Network Intelligence  
📧 [gupta.aakanksha2003@gmail.com](mailto:gupta.aakanksha2003@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/aakanksha-gupta-b32b9b24b/)

---

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome!

1. Fork the repository  
2. Open the notebook in Colab or Jupyter  
3. Make changes and save to your fork  
4. Open a pull request  

---

## 📝 License

This project is open-sourced under the **MIT License** for academic and research use.  
See the [`LICENSE`](LICENSE) file for details.
