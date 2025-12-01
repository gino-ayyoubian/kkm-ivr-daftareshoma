# kkm-ivr-System
Professional Multi-layer IVR System for KKM International Group - Platform Implementation
========================================
COPYRIGHT NOTICE
========================================

© 2025 KKM International Group. All Rights Reserved.

This software and associated documentation files (the "Software") are the exclusive 
property of KKM International Group. All intellectual property rights, including but not 
limited to copyrights, trademarks, trade secrets, and patents, are owned by KKM 
International Group.

========================================
DESIGNER & DEVELOPER
========================================

Lead Designer & Full-Stack Developer: Gino Ayyoubian
Architecture, Design, and Implementation

========================================
PROPRIETARY LICENSE
========================================

This is NOT open source software. This Software is proprietary and confidential.

1. OWNERSHIP
   KKM International Group retains all right, title, and interest in and to the Software, 
   including all intellectual property rights therein. This License does not grant you any 
   rights to trademarks, service marks, or trade names of KKM International Group.

2. RESTRICTIONS
   You may NOT, without prior written permission from KKM International Group:
   
   a) Copy, reproduce, or distribute the Software or any portion thereof
   b) Modify, adapt, translate, or create derivative works based on the Software
   c) Reverse engineer, decompile, or disassemble the Software
   d) Remove or alter any copyright, trademark, or other proprietary notices
   e) Rent, lease, lend, sell, sublicense, or transfer the Software
   f) Use the Software for any commercial purpose without authorization
   g) Extract or harvest data from the Software
   h) Use the Software to create competing products or services

3. CONFIDENTIALITY
   The Software contains trade secrets and proprietary information of KKM International 
   Group. You agree to maintain the confidentiality of the Software and not disclose it 
   to any third party without express written consent.

4. NO WARRANTY
   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
   INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A 
   PARTICULAR PURPOSE, AND NONINFRINGEMENT.

5. LIMITATION OF LIABILITY
   IN NO EVENT SHALL KKM INTERNATIONAL GROUP OR GINO AYYOUBIAN BE LIABLE FOR ANY CLAIM, 
   DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT, OR OTHERWISE, 
   ARISING FROM, OUT OF, OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS 
   IN THE SOFTWARE.

6. TERMINATION
   This License is effective until terminated. KKM International Group may terminate this 
   License at any time if you fail to comply with any term or condition. Upon termination, 
   you must destroy all copies of the Software.

7. GOVERNING LAW
   This License shall be governed by and construed in accordance with applicable 
   international copyright laws and the laws of the jurisdiction where KKM International 
   Group operates.

8. ENTIRE AGREEMENT
   This License constitutes the entire agreement between you and KKM International Group 
   concerning the Software and supersedes all prior or contemporaneous understandings.

========================================
PERMISSIONS & LICENSING INQUIRIES
========================================

For authorization to use, modify, or distribute this Software, please contact:

KKM International Group
Website: https://kkm-intl.org
Email: legal@kkm-intl.org
General Inquiries: info@kkm-intl.org

========================================
VIOLATION NOTICE
========================================

Unauthorized copying, modification, distribution, or use of this Software is strictly 
prohibited and constitutes a violation of copyright law and this License Agreement. 
Violators will be prosecuted to the fullest extent of the law.

========================================
ACKNOWLEDGMENT
========================================

By accessing or using this Software, you acknowledge that you have read this License 
Agreement, understand it, and agree to be bound by its terms and conditions.

========================================

© 2025 KKM International Group. All Rights Reserved.
Designer & Developer: Gino Ayyoubian

https://kkm-intl.org | info@kkm-intl.org

========================================




========================================
# TECHNICAL DOCUMENTATION
========================================

## 📋 درباره پروژه | About the Project

**فارسی:**
این پروژه شامل طراحی و پیاده‌سازی کامل یک سیستم IVR (تعاملی پاسخگویی صوتی) چندلایه حرفه‌ای برای گروه بین‌المللی KKM است که بر روی پلتفرم ابری دفترشما پیاده‌سازی می‌شود.

**English:**
A comprehensive professional multi-layer IVR (Interactive Voice Response) system designed and implemented for KKM International Group on the Daftareshoma cloud platform.

### ویژگی‌های کلیدی | Key Features

- ✅ Bilingual IVR System (Farsi/English)
- ✅ Three-Layer Organizational Architecture
- ✅ Management of Three Dedicated Phone Lines
- ✅ CRM Integration & Caller ID
- ✅ HSE Emergency Protocol
- ✅ VIP Access with Confidential Code
- ✅ Smart Queue Management
- ✅ VoIP Connection to Site Offices

---

## 📞 شماره‌های تماس | Contact Numbers

| خط | شماره | نقش | Role |
|:---:|:---:|:---:|:---:|
| **اصلی** | +98 21 2842 4430 | دروازه اصلی | Main Gateway |
| **عملیات** | +98 21 2842 4630 | تیم‌های پروژه | Project Teams |
| **پشتیبانی** | +98 21 9103 0822 | منابع انسانی | HR & Support |

---

## 📁 ساختار پروژه | Project Structure

```
kkm-ivr-daftareshoma/
├── README.md
├── QUICK_START.txt
├── requirements.txt
├── .gitignore
│
├── docs/
│   ├── installation_guide.txt
│   ├── tts_services_comparison.txt
│   ├── daftareshoma_configuration_guide.txt
│   └── project_timeline.txt
│
├── scripts/
│   ├── generate_audio_elevenlabs.py
│   ├── generate_audio_google.py
│   └── convert_to_8khz.py
│
└── config/
    ├── phone_numbers_config.csv
    ├── ivr_scripts_farsi.csv
    ├── ivr_scripts_english.csv
    ├── extensions_directory.csv
    ├── implementation_checklist.csv
    ├── call_flow_main_line.json
    ├── call_flow_operations.json
    ├── call_flow_support.json
    └── daftareshoma_import_config.json
```

---

## 🚀 شروع سریع | Quick Start

### پیش‌نیازها | Prerequisites

```bash
# Python 3.7+
python --version

# Git
git --version
```

### نصب | Installation

```bash
# Clone the repository
git clone https://github.com/gino-ayyoubian/kkm-ivr-daftareshoma.git
cd kkm-ivr-daftareshoma

# Install dependencies
pip install -r requirements.txt

# Read quick start guide
cat QUICK_START.txt
```

---

## 🎙️ تولید فایل‌های صوتی | Audio Generation

### Using ElevenLabs (Recommended)

```bash
# 1. Get free API Key from elevenlabs.io
# 2. Edit file and add your key
nano scripts/generate_audio_elevenlabs.py

# 3. Generate audio files
python scripts/generate_audio_elevenlabs.py

# 4. Convert to phone format (8kHz)
python scripts/convert_to_8khz.py ivr_audio_files/
```

**Cost:** Free up to 10,000 characters/month ✅

---

## ⚙️ پیکربندی | Configuration

### Daftareshoma Platform Setup

1. **Panel Access:** https://panel.daftareshoma.com
2. **Activate Lines:** Verify phone numbers
3. **Enable IVR:** Professional IVR package
4. **Upload Audio:** 12 Farsi + 7 English files (WAV, 8kHz, Mono)
5. **Configure Flows:** Use JSON files from `config/` directory

---

## 🏗️ معماری سیستم | System Architecture

### Layer 1: Strategic (C-Suite)
- 🔒 VIP Access Code: `*8888`
- 👔 Board Members, Senior Management
- 📱 Mobile Transfer (After Hours)

### Layer 2: Operations (Project Teams)
- 🏗️ Project Managers (Qeshm, Sarakhs, Tehran)
- 🚨 HSE Emergency Protocol
- 🌐 VoIP to Site Offices

### Layer 3: Support (HR & PR)
- 👥 Human Resources
- 📰 Public Relations
- 🤖 Automated Job Tracking

---

## 📊 جدول زمانی | Implementation Timeline

| Week | Activity | Status |
|:---:|:---|:---:|
| **1** | Audio File Generation | ⏳ In Progress |
| **2** | System Configuration | 📋 Ready |
| **3** | CRM Integration | 📋 Ready |
| **4** | Testing & Launch | 📋 Ready |

---

## 🔗 منابع | Resources

- 🌐 [Daftareshoma Platform](https://daftareshoma.com)
- 🤖 [ElevenLabs TTS](https://elevenlabs.io)
- 📖 [Platform Documentation](https://daftareshoma.com/blog)
- 🏢 [KKM International](https://kkm-intl.org)

---

## 👥 تیم پروژه | Project Team

- **Lead Designer & Developer:** Gino Ayyoubian
- **Platform:** Daftareshoma (Cloud-based)
- **Version:** 1.0.0
- **Date:** December 2025

---

## 📝 نکات مهم | Important Notes

⚠️ **Security:**
- Keep VIP codes confidential
- Store API Keys in `.env` file (in .gitignore)
- Strategic layer access is restricted

✅ **Best Practices:**
- Complete testing before final launch
- Regular backup of configurations
- Weekly performance reporting

---

## 📞 پشتیبانی | Support

**For Technical Support:**
- 📧 Email: info@kkm-intl.org
- 📞 Phone: +98 21 2842 4430
- 🌐 Website: https://kkm-intl.org

**For Legal/Licensing Inquiries:**
- 📧 Email: legal@kkm-intl.org

========================================

**ساخته شده با ❤️ توسط Gino Ayyoubian برای گروه بین‌المللی KKM**

**Built with ❤️ by Gino Ayyoubian for KKM International Group**

========================================
