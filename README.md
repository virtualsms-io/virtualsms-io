# 👋 VirtualSMS

**Developer-first SMS verification service.** Real SIM cards, 145+ countries, instant codes.

### 🚀 What we do

We provide SMS verification numbers for platforms like WhatsApp, Telegram, TikTok, and more. Unlike virtual number services, we use **real physical SIM cards** across Europe — delivering higher success rates and faster code delivery.

### 🔗 Quick Links

- 🌐 **Website:** [virtualsms.io](https://virtualsms.io)
- 📖 **API Docs:** [virtualsms.io/api](https://virtualsms.io/api)
- 💬 **Free Numbers:** [virtualsms.io/free-numbers](https://virtualsms.io/free-numbers)
- 📝 **Blog:** [virtualsms.io/blog](https://virtualsms.io/blog)

### 🛠️ For Developers

```bash
# Get available services
curl https://virtualsms.io/api/v1/services

# Get a number for WhatsApp verification
curl -X POST https://virtualsms.io/api/v1/activations \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -d '{"service": "whatsapp", "country": "GB"}'
```

### 📊 Coverage

- 🇬🇧 United Kingdom · 🇩🇪 Germany · 🇭🇷 Croatia · 🇺🇦 Ukraine · 🇫🇷 France
- 145+ countries via partner network
- Real EU SIM cards — not VoIP, not virtual

---

**Built for developers who need reliable SMS verification.**
