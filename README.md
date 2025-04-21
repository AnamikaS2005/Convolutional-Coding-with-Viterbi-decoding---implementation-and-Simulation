# 🧠 **Convolutional Coding with Viterbi Decoding**

A Python-based simulation of a digital communication system using **Convolutional Encoding** and **Viterbi Decoding**, implemented as part of the *Information Theory and Coding (ECT30)* course project at **College of Engineering Trivandrum**.

---

## 📌 **Project Overview**

This project demonstrates how convolutional codes and the Viterbi algorithm can be used to improve the reliability of digital communications in noisy environments. The system is evaluated under an **Additive White Gaussian Noise (AWGN)** channel using **Bit Error Rate (BER)** simulations for both **hard** and **soft** decision decoding.

---

## 🎯 **Aim**

To design and simulate a digital communication system using:
- **Convolutional Encoding**
- **Hard and Soft Decision Viterbi Decoding**
- **BER analysis under varying noise conditions**

---

## 📚 **Theoretical Background**

### 🔁 **Convolutional Encoding**
- Introduces redundancy using shift registers and XOR operations.
- Generator polynomials:
  - `g1 = (1, 0, 1)` → *g₁(D) = 1 + D²*
  - `g2 = (1, 1, 1)` → *g₂(D) = 1 + D + D²*

### 🧮 **Viterbi Decoding**
- A maximum likelihood decoding algorithm.
- Works by selecting the most probable path in a trellis structure.
- Two types:
  - **Hard Decision**: Operates on binary values (0/1)
  - **Soft Decision**: Operates on real-valued signals for better performance

---

## 🛠️ **Implementation Details**

- **Language**: Python
- **Libraries**: `numpy`, `matplotlib`
- **Features**:
  - Convolutional Encoder
  - Hard & Soft Viterbi Decoder
  - BPSK modulation
  - BER vs Eb/N0 simulation and plotting

---

## ⚙️ **Execution Flow**

1. Generate random binary data  
2. Encode using convolutional coding  
3. Modulate with BPSK  
4. Add Gaussian noise  
5. Decode using hard and soft Viterbi algorithms  
6. Compare results and compute BER  
7. Plot BER vs Eb/N0  

---

## 📊 **Results Summary**

- **Soft Decision Viterbi Decoding** shows clear performance gains over **Hard Decision**.
- At lower SNRs (e.g., 0 dB), soft decoding achieves nearly **2x improvement in BER**.
- The simulation validates the coding gain and effectiveness of convolutional codes in noisy environments.

---

## 💡 **Applications**

- Cellular systems (e.g., GSM, LTE)
- Satellite and space communications
- Wireless protocols (e.g., Wi-Fi)
- Digital TV broadcasting (DVB)
- Low-power embedded and IoT devices

---

## 🚀 **How to Run**

```bash
# Clone the repository
git clone https://github.com/your-username/convolutional-viterbi-decoder.git
cd convolutional-viterbi-decoder

# Install required packages
pip install numpy matplotlib

# Run the simulation
python simulation.py
