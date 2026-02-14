# 🏦 MudraGuru

**AI-Powered Voice Assistant for Mudra Loan Applications**

<p align="center">
  <img src="https://img.shields.io/badge/Hackathon-AI%20for%20Bharat-orange" alt="AI for Bharat"/>
  <img src="https://img.shields.io/badge/Problem%20Statement-PS3-blue" alt="PS3"/>
  <img src="https://img.shields.io/badge/Sponsor-AWS-yellow" alt="AWS"/>
  <img src="https://img.shields.io/badge/Status-In%20Development-green" alt="Status"/>
</p>

---

## 📖 Problem Statement

**AI for Communities, Access & Public Impact (PS3)**

60 million MSMEs in India are eligible for government-backed Mudra Loans but remain unaware or unable to navigate the complex, English-only application process. Small business owners like kirana store operators, salon owners, and repair shop workers face:

- ❌ Lack of awareness about Mudra loan schemes
- ❌ Intimidating application forms (English-only)
- ❌ No simple guidance in regional languages
- ❌ Difficulty accessing financial support for business growth

---

## 💡 Our Solution

**MudraGuru** is a voice-first AI assistant that democratizes access to Mudra Loans through:

✅ **Voice & Text Input** - Speak in Hindi or English  
✅ **Simple Eligibility Check** - Just 4-5 questions  
✅ **AI-Powered Guidance** - Step-by-step application help  
✅ **Loan Category Recommendations** - Shishu/Kishor/Tarun explained simply  
✅ **Form Pre-filling** - Auto-complete with user data  
✅ **Bank Branch Locator** - Find nearest branches  
✅ **Offline Support** - Works without constant internet  
✅ **2G Optimized** - Functions on slow networks  

---

## 🎯 Key Features

### 🎤 Voice-First Interface
- Amazon Transcribe for speech-to-text (Hindi & English)
- Amazon Polly for natural text-to-speech responses
- Works for users with limited digital literacy

### 🤖 Conversational AI
- Powered by Amazon Bedrock (Claude 3.5 Sonnet)
- Context-aware multi-turn conversations
- Simple, jargon-free explanations

### 📱 Progressive Web App (PWA)
- Install on any device
- Offline-first architecture
- Works on 2G networks

### 🗺️ Smart Features
- Eligibility checker with instant results
- Nearest bank branch finder
- Application form assistance
- Real-time progress tracking

---

## 🛠️ Technology Stack

### Frontend
- **Framework:** Next.js 14 (React 18)
- **Styling:** Tailwind CSS
- **Language:** TypeScript
- **PWA:** next-pwa with Workbox
- **State:** React Context API

### Backend
- **Runtime:** Node.js 18+
- **Framework:** Express.js
- **Language:** TypeScript
- **API:** RESTful design

### AWS Services
- **AI:** Amazon Bedrock (Claude 3.5 Sonnet)
- **Voice:** Amazon Transcribe + Amazon Polly
- **Database:** Amazon DynamoDB
- **Storage:** Amazon S3
- **CDN:** CloudFront
- **Auth:** AWS Cognito
- **Monitoring:** CloudWatch

### Offline & Performance
- **Client Storage:** IndexedDB
- **Service Worker:** Workbox
- **Compression:** Opus audio codec
- **Optimization:** Code splitting, lazy loading

---

## 📂 Project Structure
```
mudraguru-ai-for-bharat/
├── requirements.md          # Detailed requirements (EARS notation)
├── design.md               # System architecture & technical design
├── frontend/               # Next.js PWA application
├── backend/                # Node.js/Express API server
├── docs/                   # Additional documentation
└── README.md              # This file
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- AWS Account with Bedrock, Transcribe, Polly access
- npm or yarn

### Installation
```bash
# Clone repository
git clone https://github.com/YOUR_USERNAME/mudraguru-ai-for-bharat.git
cd mudraguru-ai-for-bharat

# Install frontend dependencies
cd frontend
npm install

# Install backend dependencies
cd ../backend
npm install

# Configure environment variables
cp .env.example .env
# Add your AWS credentials and API keys

# Run development servers
npm run dev
```

### Environment Variables
```env
# AWS Configuration
AWS_REGION=ap-south-1
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key

# Amazon Bedrock
BEDROCK_MODEL_ID=anthropic.claude-3-5-sonnet-20240620-v1:0

# Amazon S3
S3_BUCKET_NAME=mudraguru-voice-recordings

# DynamoDB Tables
DYNAMODB_USERS_TABLE=MudraGuru-Users
DYNAMODB_SESSIONS_TABLE=MudraGuru-Sessions

# API Configuration
API_BASE_URL=http://localhost:3001
FRONTEND_URL=http://localhost:3000
```

---

## 📊 Architecture Overview
```
User (Voice/Text)
    ↓
Next.js PWA (Offline-capable)
    ↓
Express API Server
    ↓
┌─────────────────────────────────┐
│  AWS Services                    │
├─────────────────────────────────┤
│  • Bedrock (AI Chat)            │
│  • Transcribe (Speech-to-Text)  │
│  • Polly (Text-to-Speech)       │
│  • DynamoDB (Database)          │
│  • S3 (Voice Storage)           │
│  • CloudFront (CDN)             │
└─────────────────────────────────┘
```

For detailed architecture, see [design.md](./design.md)

---

## 🎨 Screenshots

*Coming soon - UI mockups and demo screenshots*

---

## 🏆 Hackathon Details

- **Event:** AI for Bharat Hackathon
- **Problem Statement:** PS3 - AI for Communities, Access & Public Impact
- **Sponsor:** Amazon Web Services (AWS)
- **Tools Used:** Kiro (for requirements & design generation)
- **Submission Date:** February 2025

---

## 👥 Team: Nivasa AI

**Nivasa AI** builds foundation-level AI solutions rooted in Bharat's real-world contexts. We focus on inclusive, multilingual, and scalable intelligence that solves everyday problems across education, accessibility, and public systems with trust and impact.

### Team Members
- **Subham Singh** - Full Stack Developer
- **Udipti Nagar** - Full Stack Developer

---

## 📄 Documentation

- [requirements.md](./requirements.md) - Comprehensive requirements in EARS format
- [design.md](./design.md) - System design and architecture
- API Documentation - *Coming soon*
- User Guide - *Coming soon*

---

## 🔮 Future Roadmap

- [ ] Expand to more Indian languages (Tamil, Telugu, Bengali)
- [ ] Add support for other government schemes (PMEGP, Stand-Up India)
- [ ] WhatsApp bot integration
- [ ] SMS-based fallback for feature phones
- [ ] OCR for document scanning
- [ ] Integration with DigiLocker for KYC

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **AWS** for providing cloud infrastructure and AI services
- **Kiro** for streamlining requirements and design generation
- **AI for Bharat Hackathon** organizers for the opportunity
- Small business owners who inspired this solution

---

## 📞 Contact

For questions or collaboration:
- **Team:** Nivasa AI
- **GitHub:** [github.com/YOUR_USERNAME/mudraguru-ai-for-bharat]
- **Email:** contact@nivasaai.com *(placeholder)*

---

<p align="center">
  <strong>Built with ❤️ for Bharat's small businesses</strong>
</p>
```

---

## **🎯 HOW TO USE THIS:**

### **Option 1: Ask Kiro to Create It**

**Paste this to Kiro:**
```
Please create a README.md file with the exact content I'm providing below:

[Paste the entire README content from above]
```

---

### **Option 2: Create Manually**

1. **In Kiro:** Right-click on project folder → New File → `README.md`
2. **Paste** the entire content above
3. **Save**

---

## **⚠️ IMPORTANT: Replace Placeholders**

Before pushing to GitHub, replace:

1. **`YOUR_USERNAME`** → Your actual GitHub username (appears 2 times)
2. **`contact@nivasaai.com`** → Your actual email or keep as placeholder

---

## **✅ VERIFICATION:**

After creating README.md, your file structure should be:
```
mudraguru-ai-for-bharat/
├── .kiro/
├── requirements.md     ✅
├── design.md          ✅
├── README.md          ✅ (NEW!)
└── requirements_backup.md (delete this)
