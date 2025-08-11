# Custom Domain Setup Guide for hrudu.me

## 📋 Prerequisites
- GitHub account
- Access to your domain's DNS settings (wherever you purchased hrudu.me)
- Your portfolio code ready in the repository

## 🌐 Step-by-Step Domain Configuration

### 1. DNS Configuration at Your Domain Provider

You need to configure DNS records where you purchased your domain (GoDaddy, Namecheap, Cloudflare, etc.):

#### For Apex Domain (hrudu.me):
Add these **A records**:
```
Type: A
Name: @ (or leave empty for root domain)
Value: 185.199.108.153

Type: A
Name: @ (or leave empty for root domain)
Value: 185.199.109.153

Type: A
Name: @ (or leave empty for root domain)
Value: 185.199.110.153

Type: A
Name: @ (or leave empty for root domain)
Value: 185.199.111.153
```

#### For WWW Subdomain (optional but recommended):
Add a **CNAME record**:
```
Type: CNAME
Name: www
Value: your-github-username.github.io
```

### 2. GitHub Repository Setup

1. **Create repository** (if not already done):
   - Name: `your-github-username.github.io` (recommended for user pages)
   - Or any name like `portfolio` or `my-portfolio`
   - Make it **public**

2. **Upload your files**:
   ```bash
   git init
   git add .
   git commit -m "Add portfolio website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

### 3. GitHub Pages Configuration

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section
4. Configure:
   - **Source**: Deploy from a branch
   - **Branch**: main
   - **Folder**: / (root)
   - **Custom domain**: `hrudu.me`
   - **Enforce HTTPS**: ✅ (check this after domain is verified)

### 4. Verification Process

GitHub will automatically:
- Verify your domain ownership
- Generate SSL certificate (for HTTPS)
- Create the CNAME file in your repository

**Wait time**: 24-48 hours for full DNS propagation

### 5. Testing Your Setup

Check these URLs after setup:
- `https://hrudu.me` ✅ (should work)
- `http://hrudu.me` ✅ (should redirect to HTTPS)
- `https://www.hrudu.me` ✅ (should redirect to hrudu.me)

### 6. Troubleshooting

#### Common Issues:

**Domain not working after 24 hours:**
- Double-check DNS records at your domain provider
- Ensure A records point to GitHub's IPs
- Try clearing your browser cache

**SSL Certificate issues:**
- Uncheck "Enforce HTTPS" temporarily
- Wait for domain verification to complete
- Re-enable "Enforce HTTPS"

**404 Error:**
- Ensure your repository is public
- Check that index.html is in the root directory
- Verify branch name is set to "main" in Pages settings

### 7. Domain Provider Specific Instructions

#### GoDaddy:
1. Go to DNS Management
2. Add A records with GitHub IPs
3. Add CNAME for www

#### Namecheap:
1. Go to Advanced DNS
2. Add A records with GitHub IPs
3. Add CNAME for www

#### Cloudflare:
1. Go to DNS settings
2. Add A records (turn off proxy initially)
3. Add CNAME for www
4. Enable proxy after verification

### 8. Verification Commands

Test your DNS setup:
```bash
# Check A records
nslookup hrudu.me

# Check CNAME
nslookup www.hrudu.me

# Check if GitHub recognizes your domain
curl -I https://hrudu.me
```

## 🎉 Success!

Once everything is configured, your portfolio will be live at:
- **Primary**: https://hrudu.me
- **Alternative**: https://www.hrudu.me (redirects to primary)

Your professional portfolio will now have a custom domain that looks much more professional than a GitHub subdomain!

## 📝 Notes

- Keep the CNAME file in your repository
- DNS changes can take up to 48 hours to propagate globally
- Always use HTTPS for better SEO and security
- GitHub Pages provides free SSL certificates for custom domains
