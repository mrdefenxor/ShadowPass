# 🕶️ ShadowPass – Advanced 403 Bypass Framework

**ShadowPass** is a high-end tool designed for professional web penetration testers to **detect and bypass 403 Forbidden responses** using modern, stealthy, and multi-layered evasion techniques.

---

## 🚀 Features

- ✅ Smart Path Manipulation Engine
- ✅ Verb Tampering with fallback handling
- ✅ Header injection (Spoofing internal IPs, original paths, custom agents)
- ✅ Dynamic User-Agent & Referer randomization
- ✅ Heuristic 403/200 detector
- ✅ Threaded and fast
- ✅ Wordlist support (for fuzzing protected paths)
- ✅ JSON, plain text, or colorized CLI output
- ✅ Proxy & verbose debug mode
- ✅ Built with modular code (easy to extend)

---

## 💣 Techniques Implemented

| Category | Example Techniques |
|---------|--------------------|
| **Path Tricks** | `/admin/`, `/admin/.`, `/admin//`, `/..;/admin`, `%2e/admin`, etc. |
| **Header Spoofing** | `X-Forwarded-For: 127.0.0.1`, `X-Original-URL: /admin` |
| **Method Override** | `POST`, `HEAD`, `OPTIONS`, `DELETE` |
| **User-Agent Abuse** | `Googlebot`, `Slackbot`, `curl`, `Burp`, etc. |
| **Referer Fakes** | `Referer: target.com` or internal spoofed origins |
| **Encodings** | URL encoded (`%2e`, `%2f`), double encodings |

---

## 🛠️ Example Usage

```bash
python3 shadowpass.py --url https://target.com/admin --wordlist paths.txt
