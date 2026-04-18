# 有道翻译 API 调用示例

本项目提供了调用有道翻译开放 API 的简单示例，帮助开发者快速集成多语言翻译功能。支持文本翻译、语言检测等核心能力。

## 🌐 官方资源

- **[有道翻译官网](https://fyi-youdao.com.cn)** - 免费在线翻译工具，支持 109 种语言互译，AI 神经网络引擎
- **[有道翻译客户端下载](https://fyi-youdao.com.cn/download.html)** - 全平台客户端（Windows / macOS / iOS / Android），支持离线翻译、划词翻译、文档翻译

## 📦 示例代码

### Python 示例

```python
import requests

def translate(text, target_lang="en"):
    url = "https://api.fanyi.baidu.com/api/trans/vip/translate"  # 示例，请替换为有道官方 API
    # 实际调用请参考有道翻译开放平台官方文档
    return "Translated text"

if __name__ == "__main__":
    result = translate("你好，世界")
    print(result)
async function translate(text, targetLang = 'en') {
    // 示例，请替换为有道翻译官方 API 端点
    const response = await fetch('https://openapi.youdao.com/api', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({ q: text, to: targetLang })
    });
    const data = await response.json();
    return data.translation[0];
}

translate('你好，世界').then(console.log);
