# 🎓 EduScribe Real-Time - AI-Powered Lecture Note Generation

EduScribe is a **production-ready** AI-powered system that transforms live lectures into intelligent, organized study notes by combining real-time transcription with document context analysis using RAG (Retrieval-Augmented Generation).

## ✨ **What's New in This Version**

- ✅ **Web Audio API** - Reliable 20-second WAV chunks (no MediaRecorder issues!)
- ✅ **Real-Time Transcription** - Every 20 seconds with enhanced notes
- ✅ **Structured Notes** - Every 60 seconds with proper markdown formatting
- ✅ **Final Comprehensive Notes** - Complete lecture summary on stop
- ✅ **Optimized Token Usage** - 61% reduction, stays within Groq free tier
- ✅ **Professional UI** - Beautiful, responsive interface with real-time updates
- ✅ **Authentication System** - Secure user management with JWT
- ✅ **MongoDB Atlas** - Cloud database with vector search

## 🏗️ **Project Structure (Monorepo)**

```
d:\store\notify\
├── frontend/           # React frontend application
│   ├── src/
│   ├── package.json
│   └── ...
├── backend/            # Python FastAPI backend
│   ├── app/
│   ├── requirements.txt
│   └── ...
├── docs/               # Documentation files
└── README.md          # This file
```

## 🚀 **Quick Start**

### **Prerequisites**
- Node.js 18+ and npm
- Python 3.10+
- MongoDB Atlas account (free tier works!)
- Groq API key (free tier: 6000 tokens/min)

### **1. Backend Setup**
```bash
cd backend

# Install dependencies
pip install -r requirements.txt

# Create .env file
cp .env.example .env

# Add your credentials to .env:
# - MONGODB_URL=your_mongodb_atlas_url
# - GROQ_API_KEY=your_groq_api_key
# - JWT_SECRET_KEY=your_secret_key

# Run backend
python optimized_main.py
# Opens at http://localhost:8001
```

### **2. Frontend Setup**
```bash
cd frontend

# Install dependencies
npm install

# Run frontend
npm run dev
# Opens at http://localhost:3000
```

### **3. First Use**
1. Open http://localhost:3000
2. Sign up for an account
3. Create a subject
4. Start a lecture
5. Upload PDF documents (optional)
6. Click "Start Recording" and speak!
7. Watch real-time transcription and notes appear!

## 🎯 **Features**

### **Frontend Features:**
- **Subject-based Organization** - Organize lectures by courses/subjects
- **Document Upload Workflow** - Upload lecture materials for AI context
- **Live Recording Interface** - Real-time transcription and note generation
- **Webinar Support** - Join and host webinar sessions
- **Export Functionality** - Download notes as PDF/DOCX
- **Responsive Design** - Works on all devices

### **Backend Features:**
- **Web Audio API Recording** - Reliable 20-second WAV chunks
- **Faster Whisper Transcription** - Real-time speech-to-text (tiny model, CPU)
- **Document Processing** - Extract text from PDFs with embeddings
- **Vector Search** - MongoDB Atlas vector search + FAISS fallback
- **RAG Note Generation** - Context-aware notes using uploaded documents
- **Groq LLM Integration** - Fast, efficient note synthesis
- **WebSocket Real-Time** - Live updates every 20s/60s
- **Optimized Token Usage** - Stays within free tier limits

## 🔄 **Real-Time Workflow**

### **Every 20 Seconds:**
1. Web Audio API captures 20s of audio
2. Converts to 16kHz WAV file
3. Sends via HTTP POST to backend
4. Whisper transcribes audio
5. RAG generates enhanced notes using document context
6. WebSocket sends to frontend
7. **Live Transcription updates!**

### **Every 60 Seconds (3 chunks):**
1. Backend accumulates 3 transcriptions
2. Queries document context via vector search
3. Groq LLM synthesizes structured notes
4. Fixes transcription errors
5. Formats with markdown
6. WebSocket sends to frontend
7. **Structured Notes update!**

### **On Stop Recording:**
1. Backend collects all structured notes
2. Performs comprehensive synthesis
3. Generates final notes with:
   - Complete summary
   - Organized sections
   - Key takeaways
   - Glossary
4. **Final Notes appear!**

## 🛠️ **Technology Stack**

### **Frontend:**
- **React 18** + Vite 7
- **Tailwind CSS** for styling
- **React Router DOM** for navigation
- **Lucide React** for icons
- **React Markdown** for note rendering
- **Web Audio API** for recording
- **WebSocket** for real-time updates
- **React Hot Toast** for notifications

### **Backend:**
- **Python 3.10** + FastAPI
- **Faster Whisper** (tiny model, CPU-optimized)
- **MongoDB Atlas** (cloud database + vector search)
- **FAISS** (local vector search fallback)
- **Sentence Transformers** (all-MiniLM-L6-v2)
- **Groq API** (llama-3.1-8b-instant)
- **PyPDF2** for document processing
- **JWT** for authentication

## 📚 **Documentation**

### **Setup Guides:**
- [Quick Start Guide](./QUICK_START.md) - Get started in 5 minutes
- [Complete Implementation Guide](./COMPLETE_IMPLEMENTATION_GUIDE.md) - Full setup details
- [Authentication Guide](./AUTHENTICATION_GUIDE.md) - User management setup

### **Technical Documentation:**
- [Web Audio API Fix](./FINAL_FIX_WEB_AUDIO_API.md) - Why Web Audio API vs MediaRecorder
- [Optimization Fixes](./OPTIMIZATION_FIXES.md) - Token usage optimization
- [Frontend Fixes](./FRONTEND_FIXES_COMPLETE.md) - UI display fixes
- [Audio Processing](./AUDIO_PROCESSING_FIX.md) - Audio pipeline details
- [Final Working Solution](./FINAL_WORKING_SOLUTION.md) - Complete architecture

## ✅ **Production Ready**

- ✅ **Frontend**: Complete with authentication, subjects, live recording
- ✅ **Backend**: Optimized transcription, RAG synthesis, real-time updates
- ✅ **Database**: MongoDB Atlas with vector search
- ✅ **Authentication**: JWT-based secure user management
- ✅ **Real-Time**: WebSocket updates every 20s/60s
- ✅ **Optimized**: 61% token reduction, free tier compatible

## 🤝 **Contributing**

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## 📄 **License**

MIT License - see LICENSE file for details.
