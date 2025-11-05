# 🚀 EduScribe - Quick Start Guide

## ⚡ **Get Started in 5 Minutes!**

---

## **Step 1: Start Backend** (2 minutes)

```bash
cd backend
python optimized_main.py
```

**Expected output:**
```
hai
🔗 Connecting to: mongodb+srv://...
✅ MongoDB Atlas connected successfully!
✅ MongoDB initialized for document storage and vector search
INFO:     Uvicorn running on http://0.0.0.0:8001
```

✅ **Backend is running!**

---

## **Step 2: Start Frontend** (1 minute)

Open a **new terminal**:

```bash
cd frontend
npm run dev
```

**Expected output:**
```
  VITE v5.x.x  ready in xxx ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
```

✅ **Frontend is running!**

---

## **Step 3: Create Account** (1 minute)

1. Open browser: **http://localhost:5173**
2. Click **"Sign up"**
3. Fill form:
   - Username: Your Name
   - Email: your@email.com
   - Password: (min 6 characters)
   - Confirm Password: (same)
4. Click **"Create Account"**

✅ **You're logged in!**

---

## **Step 4: Create Subject** (30 seconds)

1. Click **"New Subject"** button
2. Fill form:
   - Name: Machine Learning
   - Code: CS-401
   - Description: (optional)
3. Click **"Create"**

✅ **Subject created!**

---

## **Step 5: Start Lecture** (30 seconds)

1. Click **"Start Lecture"** on your subject
2. Enter lecture title: "Introduction to ML"
3. (Optional) Upload PDF/PPT documents
4. Click **"Start Lecture"**

✅ **Lecture setup complete!**

---

## **Step 6: Record & See Real-Time Notes** (Test it!)

1. Click **"Start Recording"**
2. **Allow microphone access**
3. Start speaking about your topic
4. **Watch the magic happen:**
   - ✨ Transcription appears in real-time
   - ✨ Enhanced notes generate automatically
   - ✨ Structured notes update every 60 seconds
5. Click **"Stop Recording"**
6. **Final comprehensive notes generated!**
7. Click **"Save"** to save notes
8. Click **"Download"** to get Markdown file

✅ **Your first lecture is recorded!**

---

## **Step 7: View Your Notes**

1. Click **"My Notes"** or navigate to `/my-notes`
2. See all your saved notes
3. Search by title
4. Click **"View"** to see full notes
5. Click **"Download"** to export

✅ **Access your notes anytime!**

---

## 🎉 **You're All Set!**

Your EduScribe app is now fully functional!

### **What You Can Do:**
- ✅ Create multiple subjects
- ✅ Record unlimited lectures
- ✅ Get AI-powered notes in real-time
- ✅ Upload reference documents
- ✅ Search and filter notes
- ✅ Download notes as Markdown
- ✅ Access notes from anywhere

---

## 📱 **Key Pages**

- **Dashboard:** http://localhost:5173/
- **Subjects:** http://localhost:5173/subjects
- **My Notes:** http://localhost:5173/my-notes
- **Login:** http://localhost:5173/login

---

## 🔧 **Troubleshooting**

### **Backend Error: "Cannot import 'get_database'"**
```bash
# Already fixed! Just restart:
cd backend
python optimized_main.py
```

### **Frontend Error: "axios not found"**
```bash
cd frontend
npm install axios
npm run dev
```

### **WebSocket not connecting**
- Make sure backend is running on port 8001
- Check browser console for errors
- Refresh the page

### **Microphone not working**
- Allow microphone permission in browser
- Check system microphone settings
- Try a different browser (Chrome recommended)

---

## 💡 **Pro Tips**

1. **Upload documents before recording** - Better note quality
2. **Speak clearly and pause between topics** - Better transcription
3. **Use a quiet environment** - Less background noise
4. **Review notes immediately** - Edit while fresh
5. **Download important notes** - Keep backups

---

## 🎯 **Test Checklist**

- [ ] Backend starts without errors
- [ ] Frontend loads at localhost:5173
- [ ] Can sign up and login
- [ ] Dashboard shows statistics
- [ ] Can create subject
- [ ] Can start lecture
- [ ] Recording works
- [ ] Transcription appears in real-time
- [ ] Notes generate automatically
- [ ] Can save and download notes
- [ ] My Notes page shows saved notes

---

## 📚 **Learn More**

- **Complete Guide:** Read `COMPLETE_IMPLEMENTATION_GUIDE.md`
- **Authentication:** Read `AUTHENTICATION_GUIDE.md`
- **MongoDB Setup:** Read `MONGODB_SETUP_GUIDE.md`

---

## 🆘 **Need Help?**

Check the console logs:
- **Backend:** Terminal where you ran `python optimized_main.py`
- **Frontend:** Browser Developer Tools (F12) → Console

---

## 🎊 **Enjoy Your Professional Note-Taking App!**

You now have a fully functional, AI-powered, real-time lecture transcription and note-taking system!

**Happy Learning! 📝✨**
