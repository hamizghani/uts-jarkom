# UTS Jaringan Komputer (Jarkom) — Rangkuman & Visualisasi Interaktif

Repositori persiapan Ujian Tengah Semester (UTS) mata kuliah **Jaringan Komputer (CSIM603154)**, Fakultas Ilmu Komputer, Universitas Indonesia.
Referensi utama: *Kurose & Ross, Computer Networking: A Top-Down Approach (8th Edition)*.

---

## 📖 Konten Pembelajaran

File interaktif utama adalah [**`Jarkom — Belajar UTS.html`**](Jarkom%20%E2%80%94%20Belajar%20UTS.html).
- **100% Offline & Standalone:** Dapat dibuka langsung di peramban web (browser) apa pun tanpa membutuhkan koneksi internet atau library eksternal.
- **Dark Mode Native:** Tampilan minimalis berlatar hitam yang nyaman untuk sesi belajar panjang.
- **28 Diagram SVG Responsif:** Ilustrasi vektor mendalam untuk mempermudah pemahaman konsep abstrak jaringan.

---

## 📑 Silabus Materi (W01 – W08)

| Minggu | Topik | Pokok Bahasan & Visualisasi Kunci |
| :--- | :--- | :--- |
| **W01** | **Computer Networks and the Internet** | Host, packet switching vs circuit switching, 4 komponen nodal delay ($d_{proc}, d_{queue}, d_{trans}, d_{prop}$), throughput bottleneck, hierarki 5-layer Internet, enkripsi & enkapsulasi Matryoshka. |
| **W02** | **Application Layer & DNS** | Arsitektur Client-Server vs P2P, socket identifier (IP + Port), layanan transport (TCP vs UDP vs TLS), HTTP/1.0 vs HTTP/1.1 (perhitungan RTT), cookies & session, web caching, dan hierarki DNS terdistribusi (resolusi iterated vs recursive). |
| **W03** | **Video Streaming, CDN & UDP** | Kompresi spasial & temporal video, DASH (Dynamic Adaptive Streaming over HTTP), playout buffering, arsitektur CDN (*Enter Deep* vs *Bring Home*), pengalihan via DNS CNAME, multiplexing/demultiplexing port, dan protokol UDP (Internet Checksum 1's complement). |
| **W04** | **Transport Layer & TCP** | Socket API Python (`SOCK_STREAM` vs `SOCK_DGRAM`), 3-way handshake & teardown lifecycle (TIME_WAIT), struktur header TCP 20 byte, estimasi RTT (EWMA) & safety margin DevRTT, skenario retransmisi TCP, cumulative ACK, dan Fast Retransmit (3 duplicate ACKs). |
| **W05** | **HTTP Evolution, QUIC & MoQ** | Analisis 3 tingkatan Head-of-Line (HOL) blocking (App-level HTTP/1.1, TCP-level HTTP/2, dan stream independen HTTP/3), arsitektur QUIC di atas UDP di user-space, Connection Migration via CID 64-bit, handshake terintegrasi TLS 1.3 (1-RTT & 0-RTT), dan Media over QUIC (MoQ). |
| **W06** | **Network Layer Data Plane & Subnetting** | Forwarding (data plane) vs Routing (control plane), model Best Effort, arsitektur internal router (input ports, switching fabric memory/bus/crossbar, output buffer), Longest Prefix Match via TCAM, packet scheduling (FIFO, Priority, RR, WFQ), IPv4 header, IPv6 header fixed 40 byte, tunneling IPv6 over IPv4, serta perhitungan subnetting FLSM & VLSM terurut. |
| **W07** | **DHCP, NAT, Middleboxes & IP Architecture** | Aturan penyingkatan IPv6 (RFC 5952), protokol DHCP 4 tahap (DORA broadcast), alokasi IP hierarkis & route aggregation, NAT (Network Address Translation) & rewriting port 16-bit, Generalized Forwarding OpenFlow match-plus-action, Middleboxes, arsitektur Internet Hourglass (IP thin waist), dan fragmentasi datagram IPv4. |
| **W08** | **Network Layer Control Plane** | Abstraksi pemodelan graf, algoritma Link-State (Dijkstra) vs Distance-Vector (Bellman-Ford), routing hierarki Autonomous System (AS), protokol intra-AS OSPF (Area 0 Backbone & ABR/ASBR), protokol inter-AS BGP (eBGP, iBGP, AS-PATH loop prevention, hot-potato routing), arsitektur SDN 3-tier (Northbound REST & Southbound OpenFlow), diagnosa jalur ICMP & Traceroute, serta evolusi manajemen jaringan SNMP/MIB menuju NETCONF/YANG. |

---

## 🚀 Cara Menjalankan

Cukup klon atau unduh repositori ini, lalu buka file HTML di browser:
```bash
git clone https://github.com/hamizghani/uts-jarkom.git
cd uts-jarkom
# Buka file di browser:
start "Jarkom — Belajar UTS.html"   # Windows
# open "Jarkom — Belajar UTS.html"    # macOS
# xdg-open "Jarkom — Belajar UTS.html" # Linux
```
