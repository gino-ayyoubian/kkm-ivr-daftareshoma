# KKM IVR SYSTEM - COMPLETE PROJECT FILES GUIDE

**Designed & Developed by:** Gino Ayyoubian  
**For:** KKM International Group  
**Date:** December 2025

---

## 📋 TABLE OF CONTENTS

1. [Current Status](#current-status)
2. [Quick Implementation Guide](#quick-implementation-guide)
3. [Complete File Contents](#complete-file-contents)
   - Documentation Files (docs/)
   - Script Files (scripts/)
   - Configuration Files (config/)
4. [Step-by-Step Instructions](#step-by-step-instructions)
5. [Next Steps](#next-steps)

---

## ✅ CURRENT STATUS

### Files Already Created:
1. ✅ `.gitignore` - Python template
2. ✅ `README.md` - Legal + Technical documentation (300+ lines)
3. ✅ `requirements.txt` - Python dependencies  
4. ✅ `QUICK_START.txt` - Bilingual quick start guide

### Repository:
🔗 https://github.com/gino-ayyoubian/kkm-ivr-daftareshoma

---

## 🚀 QUICK IMPLEMENTATION GUIDE

### Option 1: Using GitHub Web Interface
Continue creating files one by one (slow but no local setup needed)

### Option 2: Using Git Command Line (RECOMMENDED ⭐)

```bash
# 1. Clone the repository
git clone https://github.com/gino-ayyoubian/kkm-ivr-daftareshoma.git
cd kkm-ivr-daftareshoma

# 2. Create folder structure
mkdir -p docs scripts config

# 3. Create all files (copy content from sections below)
# Use your favorite text editor to create each file

# 4. Commit and push
git add .
git commit -m "➕ Add complete project structure with all files"
git push origin main
```

---

## 📁 COMPLETE FILE CONTENTS

---

### 📖 DOCUMENTATION FILES (docs/)

---

#### File: `docs/installation_guide.txt`

```
========================================
KKM IVR SYSTEM - INSTALLATION GUIDE
========================================

Complete step-by-step installation guide
for the KKM IVR System on Daftareshoma platform.

Designed & Developed by: Gino Ayyoubian
Version: 1.0.0
========================================

TABLE OF CONTENTS
-----------------
1. System Requirements
2. Pre-installation Checklist
3. Installation Steps
4. Configuration
5. Testing
6. Troubleshooting

========================================
1. SYSTEM REQUIREMENTS
========================================

**Local Development:**
- Python 3.7 or higher
- Git 2.0 or higher
- Text editor (VS Code, Sublime, Notepad++)
- Internet connection
- ElevenLabs API Key (free tier available)

**Cloud Platform:**
- Daftareshoma account
- Phone numbers: +98 21 2842 4430, +98 21 2842 4630, +98 21 9103 0822
- IVR Professional package

**Disk Space:**
- Minimum: 100 MB
- Recommended: 500 MB (including audio files)

========================================
2. PRE-INSTALLATION CHECKLIST
========================================

□ Python 3.7+ installed
□ Git installed and configured  
□ GitHub account access
□ Daftareshoma panel access
□ ElevenLabs account created
□ API Keys secured
□ Phone numbers verified

========================================
3. INSTALLATION STEPS
========================================

Step 1: Clone Repository
------------------------
git clone https://github.com/gino-ayyoubian/kkm-ivr-daftareshoma.git
cd kkm-ivr-daftareshoma

Step 2: Install Dependencies
----------------------------
pip install -r requirements.txt

# If you get permission errors:
pip install --user -r requirements.txt

# Or use virtual environment (recommended):
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt

Step 3: Configure Environment
-----------------------------
# Create .env file
echo "ELEVENLABS_API_KEY=your_api_key_here" > .env
echo "GOOGLE_CLOUD_API_KEY=optional_key_here" >> .env

# Edit .env with your actual keys
nano .env  # or use your favorite editor

Step 4: Verify Installation
---------------------------
python --version
pip list | grep elevenlabs
pip list | grep pydub

========================================
4. CONFIGURATION
========================================

Phone Numbers Configuration
--------------------------
Edit config/phone_numbers_config.csv

IVR Scripts
-----------
Review and customize:
- config/ivr_scripts_farsi.csv
- config/ivr_scripts_english.csv

Call Flow
---------
Configure JSON files:
- config/call_flow_main_line.json
- config/call_flow_operations.json  
- config/call_flow_support.json

========================================
5. TESTING
========================================

Local Testing
-------------
python scripts/generate_audio_elevenlabs.py --test

Audio Generation
----------------
python scripts/generate_audio_elevenlabs.py
python scripts/convert_to_8khz.py ivr_audio_files/

========================================
6. TROUBLESHOOTING
========================================

Common Issues:

Issue: "Module not found"
Solution: pip install -r requirements.txt

Issue: "API Key invalid"
Solution: Check .env file, regenerate key at elevenlabs.io

Issue: "Permission denied"
Solution: Use --user flag or virtual environment

Issue: "Audio quality poor"
Solution: Check sample rate (8kHz for phone), use Mono

========================================
SUPPORT
========================================

Technical Support:
- Email: info@kkm-intl.org
- Phone: +98 21 2842 4430

Legal/Licensing:
- Email: legal@kkm-intl.org

© 2025 KKM International Group
Designed & Developed by Gino Ayyoubian
========================================
```

---

#### File: `docs/tts_services_comparison.txt`

```
========================================
TTS SERVICES COMPARISON
========================================

Comprehensive comparison of Text-to-Speech
services for KKM IVR System

========================================

SERVICES COMPARED:
1. ElevenLabs (Recommended ⭐)
2. Google Cloud Text-to-Speech
3. Amazon Polly
4. Microsoft Azure Speech
5. Narakeet

========================================

1. ELEVENLABS
   Rating: ⭐⭐⭐⭐⭐

   Pros:
   + Most natural-sounding voices
   + Excellent Persian support
   + Free tier: 10,000 chars/month
   + Easy API integration
   + Emotional AI capabilities
   + 100+ voices available

   Cons:
   - Limited free tier
   - Requires internet

   Pricing:
   - Free: 10,000 chars/month
   - Starter: $5/month (30,000 chars)
   - Creator: $22/month (100,000 chars)

   Best For: Professional IVR with natural voices

========================================

2. GOOGLE CLOUD TTS
   Rating: ⭐⭐⭐⭐

   Pros:
   + 4 Persian WaveNet voices
   + Free tier: 1M chars/month
   + SSML support
   + Audio profiles for phone
   + Reliable infrastructure

   Cons:
   - Less natural than ElevenLabs
   - Complex setup

   Pricing:
   - Free: 1M chars/month
   - Standard: $4/1M chars
   - WaveNet: $16/1M chars

   Best For: High-volume applications

========================================

3. AMAZON POLLY
   Rating: ⭐⭐⭐

   Pros:
   + AWS integration
   + Neural voices available
   + Free tier: 5M chars/month

   Cons:
   - Limited Persian support
   - Requires AWS account

========================================

RECOMMENDATION FOR KKM:

Primary: ElevenLabs
- Best voice quality
- Perfect for professional image
- Free tier sufficient for pilot

Backup: Google Cloud TTS  
- For high-volume future
- More cost-effective at scale
- Reliable uptime

========================================
```

---

## 🔄 CONTINUATION...

**Due to length constraints, the complete file with ALL remaining contents (scripts, configs, etc.) would be too large for a single file.**

---

## 📝 IMMEDIATE ACTION PLAN

### What You Should Do Now:

1. **Clone the repository locally:**
   ```bash
   git clone https://github.com/gino-ayyoubian/kkm-ivr-daftareshoma.git
   cd kkm-ivr-daftareshoma
   ```

2. **Create folder structure:**
   ```bash
   mkdir -p docs scripts config
   ```

3. **I will create separate commits for:**
   - ✅ All documentation files (docs/)
   - ✅ All script files (scripts/)
   - ✅ All configuration files (config/)

4. **You can then pull and continue locally or use the files as templates**

---

## 📞 SUPPORT

For questions or assistance:
- **Email:** info@kkm-intl.org
- **Phone:** +98 21 2842 4430

---

© 2025 KKM International Group  
Designed & Developed by **Gino Ayyoubian**

---
