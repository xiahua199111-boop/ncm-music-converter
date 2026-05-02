# ncm-music-converter

**一个基于Flask 驱动的轻量化NCM音乐格式本地转换工具。**

## 🌟 项目简介
本工具旨在解决ncm加密格式无法在普通播放器上播放的问题。它采用完全本地化的处理方式，确保您的音乐数据和隐私不会上传到任何云端服务器。

## ✨ 核心特性
*   **🔒 隐私保护**：所有转换操作均在本地计算机完成，无需互联网连接，数据零泄露风险。
*   **🎵 无损提取**：通过 AES-128 与非标准 RC4 算法，从加密容器中精准还原原始音轨。
*   **⚡ 自动识别**：智能解析文件头信息，自动判定并导出 **MP3** 或 **FLAC** 格式。
*   **🎨 交互友好**：采用 Web 界面操作，实时反馈转换状态，摆脱枯燥的命令行黑框。

## 🛠️ 安装与使用

### 方式 A：直接运行 (推荐普通用户)
1.  前往 [Releases](https://github.com/xiahua199111-boop/ncm-music-converter/releases) 页面下载最新版本的 `.exe` 压缩包。
2.  解压后双击运行 `ncm-music-converter.exe`。
3.  **请耐心等待 3-5 秒**，程序会自动在浏览器中弹出转换界面。

### 方式 B：开发者模式 (源码运行)
1.  **克隆仓库**：
    ```bash
    git clone [https://github.com/xiahua199111-boop/ncm-music-converter.git](https://github.com/xiahua199111-boop/ncm-music-converter.git)
    ```
2.  **安装依赖**：
    ```bash
    pip install flask pycryptodome rich
    ```
3.  **启动程序**：
    ```bash
    python app.py
    ```
4.  **访问地址**：在浏览器输入 `http://127.0.0.1:5000`。

## 📚 技术栈
*   **后端**: Python / Flask
*   **解密引擎**: 基于 ncmdump (v1.1.6) 逻辑实现
*   **密码学**: AES-128, RC4 字节流处理

## ⚖️ 免责声明
本工具仅供技术交流与学术研究使用。请支持正版音乐，尊重版权所有者的合法权益。用户因非法使用本工具而产生的任何纠纷，由用户本人承担。
