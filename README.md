# Bitcoin Puzzle Solving Tools Guide 🧩

This guide compares popular tools for solving Bitcoin puzzles and explains their optimal use cases.

---

## 📊 Tool Comparison Table

| Tool               | Hardware       | Key Features                                                                 | Use Case                                  | Pros                                        | Cons                                         | Links                                      |
|--------------------|----------------|-----------------------------------------------------------------------------|-------------------------------------------|--------------------------------------------|----------------------------------------------|--------------------------------------------|
| **Keyhunt**        | 💻 CPU         | BSGS algorithm, high RAM usage                                              | Large puzzles (#66+, CPU limited)         | Wide keyspace coverage                     | No GPU support, slow                        | [GitHub](https://github.com/albertobsd/keyhunt) |
| **Keyhunt-CUDA**   | 🎮 NVIDIA GPU  | CUDA-optimized Keyhunt, high speed                                           | Massive puzzles (#70+)                    | 30% faster than Bitcrack, multi-GPU        | Complex setup                                | [GitHub](https://github.com/kanhavishva/keyhunt-cuda) |
| **Bitcrack**       | 🎮 NVIDIA GPU  | Basic brute-force, manual multi-GPU                                         | Small ranges (#50-65)                     | Simple usage                               | No progress tracking, low efficiency         | [GitHub](https://github.com/brichard19/BitCrack) |
| **Kangaroo**       | 💻 CPU/GPU     | Pubkey-based search, Pollard's Kangaroo algorithm                           | Addresses with known pubkeys              | Efficient for large keyspaces              | Requires pubkey                              | [GitHub](https://github.com/JeanLucPons/Kangaroo) |
| **BSGS-CUDA**      | 🎮 NVIDIA GPU  | CUDA-optimized BSGS                                                         | Mid-range puzzles (#50-70)                | Fast scanning                              | Requires PureBasic v5.3 (legacy)             | [GitHub](https://github.com/Etayson/BSGS-CUDA) |
| **Brainflayer**    | 💻 CPU/GPU     | Brainwallet brute-force, wordlist support                                   | Brainwallet cracking                      | Flexible input formats                     | High RAM usage                               | [GitHub](https://github.com/ryancdotorg/brainflayer) |
| **VanBitCracken**  | 🎮 NVIDIA GPU  | Optimized for RTX 3070, random/sequential modes                             | Windows-specific solutions                | User-friendly interface                    | Closed-source (risky)                        | [Forum](https://bitcointalk.org/index.php?topic=1306983.0) |

---

## 🎯 Optimal Use Cases

### 1. **Large Puzzles (#70+)**  
- **Recommended Tools:** `Keyhunt-CUDA` (speed) or `Rotor-CUDA` (flexibility).  

### 2. **Addresses with Known Pubkeys**  
- **Recommended Tool:** `Kangaroo` (algorithmic advantage).  

### 3. **Brainwallet Cracking**  
- **Recommended Tool:** `Brainflayer` (optimized for wordlists).  

### 4. **Small Ranges (#1-50)**  
- **Recommended Tools:** `BSGS` (CPU efficiency) or `Bitcrack` (simplicity).  

---

## ⚠️ Critical Notes
- **Security:** Avoid closed-source tools like `VanBitCracken` unless verified. Only use official links.
- **Performance:** GPU tools (Keyhunt-CUDA, Bitcrack) work best with NVIDIA cards.
- **Updates:** Check version compatibility for older tools like `BSGS-CUDA`.

---

## 🔗 Useful Resources
- [Bitcoin Puzzle Discussion Forum](https://bitcointalk.org)
- [CUDA Installation Guide](https://developer.nvidia.com/cuda-downloads)
