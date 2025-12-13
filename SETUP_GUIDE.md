# Setup Guide for Arvind Kumar Chaudhary's Website

This guide will help you deploy your personalized academic website to GitHub Pages.

## Quick Overview

Your website has been customized with:
- ✅ Your name and current position (Solution Architect at Cognizant)
- ✅ Your professional background and experience
- ✅ All three published papers from 2025
- ✅ Your ORCID ID (0009-0000-8382-4598) and Scopus ID (60103614900)
- ✅ Professional memberships (IEEE ComSoc, ACM, IETE)
- ✅ EuroHPC grant information
- ✅ Complete employment history

## Step-by-Step Deployment

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in (or create an account)
2. Click the "+" icon in the top right → "New repository"
3. Repository name options:
   - For `https://yourusername.github.io`: name it exactly `yourusername.github.io`
   - For `https://yourusername.github.io/portfolio`: name it `portfolio`
4. Make it **Public**
5. Don't initialize with README (we already have one)
6. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Via GitHub Web Interface (Easiest)**
1. On your new repository page, click "uploading an existing file"
2. Drag and drop ALL these files:
   - index.html
   - about.html
   - publications.html
   - styles.css
   - README.md
   - IMAGES_GUIDE.md
3. Write commit message: "Initial website commit"
4. Click "Commit changes"

**Option B: Via Git Command Line**
```bash
git init
git add .
git commit -m "Initial website commit"
git branch -M main
git remote add origin https://github.com/yourusername/repository-name.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Click **Pages** in the left sidebar
3. Under "Source":
   - Select branch: **main**
   - Select folder: **/ (root)**
4. Click **Save**
5. Wait 2-3 minutes for deployment
6. Your site will be live at the URL shown!

### Step 4: Add Your Images

You need to create an `images` folder and add the following images:

#### Required Images:
1. **profile.jpg** - Your professional headshot
2. **cognizant-logo.png** - Cognizant company logo
3. **iot-healthcare.jpg** - Visual for IoT healthcare paper
4. **5g-security.jpg** - Visual for 5G security paper
5. **ai-ethics-rpa.jpg** - Visual for AI ethics paper
6. **scopus-profile.jpg** - Placeholder for Scopus
7. **orcid-profile.jpg** - Placeholder for ORCID

#### How to Add Images:

**Via GitHub:**
1. In your repository, click "Add file" → "Create new file"
2. Type: `images/placeholder.txt`
3. Commit to create the folder
4. Click "Add file" → "Upload files"
5. Drag your images into the upload area
6. Commit changes

**Recommended Image Sizes:**
- Profile photo: 560×560px
- Company logo: 240×120px (PNG with transparency)
- Research images: 600×400px

**Temporary Placeholder Option:**
If you don't have images ready, the site will work with broken image links. You can:
- Use placeholder services like `https://placehold.co/600x400`
- Add images later
- Create simple graphics with tools like Canva

### Step 5: Customize Further (Optional)

#### Update Social Media Links
In all three HTML files, update these placeholders:
- GitHub: Replace `arvindkchaudhary` with your actual username
- Twitter/X: Replace `arvindkchaudhary` with your actual handle
- LinkedIn: Replace `arvindkchaudhary` with your actual profile name
- Email: Verify `arvind.chaudhary@cognizant.com` is correct

#### Update Colors (Optional)
Edit `styles.css` at the top:
```css
:root {
    --primary-color: #1a1a1a;      /* Main text */
    --link-color: #0066cc;         /* Link color */
    --link-hover: #004499;         /* Link hover */
}
```

## Your Website Structure

```
your-repository/
├── index.html              # Home page with intro & research
├── about.html             # About page with full bio
├── publications.html      # All your publications
├── styles.css            # Styling
├── README.md             # Documentation
├── IMAGES_GUIDE.md       # Image guide
└── images/               # Your images folder
    ├── profile.jpg
    ├── cognizant-logo.png
    ├── iot-healthcare.jpg
    ├── 5g-security.jpg
    ├── ai-ethics-rpa.jpg
    ├── scopus-profile.jpg
    └── orcid-profile.jpg
```

## Content Already Included

### Home Page (index.html)
- Introduction paragraph about your current role
- Social media links with ORCID and Scopus
- Recent updates section with:
  - IETE Fellowship (Dec 2025)
  - EuroHPC Grant (Nov 2025)
  - CISES paper (Aug 2025)
  - AIC paper (Jul 2025)
  - ICOCT paper (2025)
  - Cognizant position (2014)
- Spotlight research with all 3 papers

### About Page (about.html)
- Professional biography
- Education (B.E. from Dr. Bhim Rao Ambedkar University)
- Research interests (8 key areas)
- Complete employment history:
  - Cognizant (2014-Present)
  - TCS (2008-2014)
  - CMT Limited (2005-2008)
  - Texport Industries (2004-2005)
  - Coincap Systems (2003-2004)
- Memberships:
  - IETE Fellow
  - IEEE ComSoc Senior Member
  - ACM Professional Member
- EuroHPC Grant information

### Publications Page (publications.html)
1. **IoT Healthcare Paper** - CISES 2025
   - DOI: 10.1109/cises66934.2025.11265584
2. **5G Security Paper** - IEEE AIC 2025
   - DOI: 10.1109/aic66080.2025.11211993
3. **AI Ethics Paper** - ICOCT 2025
   - DOI: 10.1109/ICOCT64433.2025.11118464
   - Scopus EID: 2-s2.0-105016310450
- Links to Scopus and ORCID profiles

## Testing Your Website

Before going live:
1. ✅ Check all links work
2. ✅ Verify email address is correct
3. ✅ Test on mobile devices
4. ✅ Add actual social media URLs
5. ✅ Upload professional images

## Updating Your Website

To add new content:
1. Edit the HTML files in your repository
2. Commit changes
3. Wait 1-2 minutes for GitHub to rebuild
4. Refresh your website

### Adding New Publications

In `publications.html`, add:
```html
<div class="publication-item">
    <div class="pub-image">
        <img src="images/new-paper.jpg" alt="Paper title">
    </div>
    <div class="pub-content">
        <h3>Your New Paper Title</h3>
        <p class="pub-authors"><strong>Arvind Kumar Chaudhary</strong>, et al.</p>
        <p class="pub-venue"><em>Conference Name 2026</em></p>
        <div class="pub-links">
            <a href="DOI-LINK" class="btn-paper" target="_blank">PDF</a>
        </div>
    </div>
</div>
```

### Adding Updates

In `index.html` under Updates section:
```html
<div class="update-item">
    <strong>[Month Year]</strong> Your update text here.
</div>
```

## Troubleshooting

**Site not loading?**
- Wait 3-5 minutes after enabling Pages
- Check Settings → Pages shows "Your site is published"
- Clear browser cache

**Images not showing?**
- Verify images are in `images/` folder
- Check filename matches exactly (case-sensitive)
- Ensure images are committed to repository

**Links not working?**
- Verify URLs start with `https://`
- Check for typos in DOI links
- Test each link after adding

## Professional Tips

1. **Keep it updated**: Add new papers within a week of publication
2. **Professional photo**: Use a high-quality headshot with good lighting
3. **Consistent style**: Maintain the clean, academic aesthetic
4. **Mobile-first**: Always test on phone/tablet
5. **SEO**: Page titles are already optimized with your name
6. **Backup**: Keep local copies of your files

## Next Steps

1. ✅ Deploy to GitHub Pages (Steps 1-3)
2. ✅ Add your images (Step 4)
3. ✅ Update social media URLs
4. ✅ Test everything works
5. ✅ Share your new website!

## Custom Domain (Optional)

Want to use your own domain (e.g., arvindchaudhary.com)?
1. Buy domain from registrar (Namecheap, GoDaddy, etc.)
2. Add `CNAME` file to repository with your domain
3. Configure DNS at your registrar
4. Follow [GitHub's guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## Support

Need help?
- GitHub Pages Docs: https://docs.github.com/pages
- Create issue in your repository
- Check the README.md for general guidance

---

**Your website is ready to go live!** Just follow the deployment steps above and you'll have a professional academic portfolio online in minutes.

Good luck with your website! 🚀
