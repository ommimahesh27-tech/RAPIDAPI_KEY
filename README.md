# 🎓 Study Abroad Hub - GitHub Pages

University search platform powered by Advance Course Finder API.

## 🚀 Quick Setup

### Step 1: Fork this Repository
Click the **Fork** button (top right)

### Step 2: Add API Key as Secret
1. Go to your forked repo
2. Click **Settings** → **Secrets and variables** → **Actions**
3. Click **New repository secret**
4. Name: `RAPIDAPI_KEY`
5. Value: Your RapidAPI key (`7e7ffbce67msh05b3b0bd40376b5p147aa4jsn3e386726bda4`)
6. Click **Add secret**

### Step 3: Enable GitHub Pages
1. Go to **Settings** → **Pages**
2. Source: **GitHub Actions**
3. Save

### Step 4: Deploy
1. Go to **Actions** tab
2. Click **Deploy to GitHub Pages** workflow
3. Click **Run workflow** → **Run workflow**
4. Wait 1-2 minutes

### Step 5: Visit Your Site
Your site will be live at: `https://YOUR-USERNAME.github.io/REPO-NAME/`

---

## 📝 Files Structure

```
├── index.html              # Main HTML file (API key gets injected here)
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions workflow
└── README.md               # This file
```

---

## 🔧 How It Works

1. **GitHub Actions** runs when you push code
2. It reads your `RAPIDAPI_KEY` from Secrets
3. Replaces `YOUR_RAPIDAPI_KEY_HERE` in `index.html`
4. Deploys to GitHub Pages

---

## ✨ Features

- ✅ Real university data from Advance Course Finder API
- ✅ Filter by country
- ✅ Filter by course
- ✅ IELTS requirement filter
- ✅ Search by university name
- ✅ Responsive design

---

## 🔄 Updating

To update:
1. Edit `index.html`
2. Commit and push
3. GitHub Actions auto-deploys

---

## 📊 API Endpoints Used

- `GET /country` - List of countries
- `GET /university` - List of universities
- `GET /course` - List of courses

---

## 🔒 Security Note

Your API key is stored securely in GitHub Secrets and never exposed in the repository or deployment.

---

## 📖 API Documentation

API: **Advance Course Finder**  
Host: `advance-course-finder.p.rapidapi.com`  
Docs: Check your RapidAPI dashboard

---

## 🆘 Troubleshooting

**Site not loading?**
- Check GitHub Actions tab for errors
- Verify API key is added as secret
- Ensure GitHub Pages is enabled

**API errors?**
- Verify API key is correct
- Check API rate limits on RapidAPI

---

## 📄 License

MIT License - Feel free to modify and use!
