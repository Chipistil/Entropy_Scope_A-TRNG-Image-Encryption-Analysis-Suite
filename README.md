# EntropyScope

**Browser-based TRNG Image Encryption Analysis Suite**

EntropyScope 是一个纯浏览器端的真随机数生成器（TRNG）综合评估平台。通过图像加密这一载体，从比特流统计、颜色分布、像素相关性、保真度和鲁棒性五个维度，全方位衡量忆阻器双时钟 TRNG 熵源的随机性质量。

无需后端服务，无需安装依赖——打开 HTML 即可使用。

---

## Features

### 1. Bitstream Analysis
- Shannon entropy calculation with step-by-step breakdown
- Bitmap visualization of raw bitstream
- Autocorrelation function (ACF) with 95% confidence interval

### 2. Image XOR Encryption / Decryption
- Full-color image encryption using TRNG bitstream as key
- Bit-level XOR with configurable key offset
- Side-by-side original / encrypted / decrypted comparison
- Key usage statistics (consumed, remaining, cycle count)

### 3. Statistical Analysis
- **Color histogram** comparison (R/G/B channels)
  - Original: filled area chart
  - Encrypted: dashed outline for clear contrast
- **Adjacent pixel correlation** scatter plots
  - Horizontal, vertical, diagonal directions
  - High-contrast color coding with zero-border rendering
- Correlation coefficient summary table

### 4. Fidelity Analysis (MSE / PSNR / SSIM)
- Per-channel and overall MSE, PSNR, SSIM
- Configurable SSIM window size, K1, K2 parameters
- Pixel difference range statistics
- Full computation detail log

### 5. Robustness Testing
- Salt-and-pepper noise injection at configurable ratios (0%, 6.25%, 12.5%, 25%, 50%)
- Decrypted image gallery with embedded PSNR/MSE per noise level
- PSNR degradation curve chart
- Color-coded quality indicator (Excellent / Good / Fair / Poor)
# Open directly in browser
open index.html
