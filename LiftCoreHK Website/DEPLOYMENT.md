# 🚀 Deployment Guide: Vercel + GoDaddy Domain

This guide will help you deploy your LiftCore website to Vercel and connect it to your GoDaddy domain.

## 📋 Prerequisites

- [Vercel Account](https://vercel.com/signup) (free)
- GoDaddy domain
- Git repository (GitHub, GitLab, or Bitbucket)

## 🎯 Step 1: Deploy to Vercel

### Option A: Deploy via Vercel Dashboard (Recommended)

1. **Go to Vercel Dashboard**
   - Visit [vercel.com](https://vercel.com)
   - Sign up/login with your GitHub, GitLab, or Bitbucket account

2. **Import Your Project**
   - Click "New Project"
   - Import your Git repository containing the website files
   - Vercel will automatically detect it's a static HTML site

3. **Configure Project**
   - **Project Name**: `liftcore-website` (or your preferred name)
   - **Framework Preset**: Other (or Static)
   - **Root Directory**: `./` (leave as default)
   - **Build Command**: Leave empty (not needed for static sites)
   - **Output Directory**: Leave empty (not needed for static sites)

4. **Deploy**
   - Click "Deploy"
   - Vercel will build and deploy your site
   - You'll get a URL like: `https://liftcore-website.vercel.app`

### Option B: Deploy via Vercel CLI

1. **Install Vercel CLI**
   ```bash
   npm i -g vercel
   ```

2. **Login to Vercel**
   ```bash
   vercel login
   ```

3. **Deploy**
   ```bash
   vercel
   ```

## 🌐 Step 2: Connect GoDaddy Domain

### 1. Get Vercel Nameservers

1. **In Vercel Dashboard**
   - Go to your project
   - Click "Settings" → "Domains"
   - Add your GoDaddy domain (e.g., `liftcore.com`)
   - Vercel will show you nameservers to use

2. **Note the Nameservers**
   - You'll see something like:
     - `ns1.vercel-dns.com`
     - `ns2.vercel-dns.com`
     - `ns3.vercel-dns.com`

### 2. Update GoDaddy Nameservers

1. **Login to GoDaddy**
   - Go to [godaddy.com](https://godaddy.com)
   - Sign in to your account

2. **Access Domain Settings**
   - Go to "My Products" → "Domains"
   - Find your domain and click "Manage"

3. **Change Nameservers**
   - Click "DNS" or "Nameservers"
   - Select "Change nameservers"
   - Choose "I'll use my own nameservers"
   - Add the Vercel nameservers:
     ```
     ns1.vercel-dns.com
     ns2.vercel-dns.com
     ns3.vercel-dns.com
     ```
   - Click "Save"

### 3. Verify Domain Connection

1. **Wait for Propagation**
   - DNS changes can take 24-48 hours
   - Usually works within 1-2 hours

2. **Check Status**
   - In Vercel dashboard, check domain status
   - Should show "Valid Configuration" when ready

## 🔧 Step 3: SSL Certificate

- **Automatic**: Vercel provides free SSL certificates
- **No action needed**: HTTPS will work automatically
- **Force HTTPS**: Vercel redirects HTTP to HTTPS by default

## 📱 Step 4: Test Your Website

1. **Visit your domain**: `https://yourdomain.com`
2. **Test all features**:
   - Navigation
   - Language switching
   - Contact information
   - Responsive design
   - Animations

## 🔄 Step 5: Future Updates

### Automatic Deployments
- **Git Integration**: Push to your repository
- **Auto-deploy**: Vercel automatically deploys changes
- **Preview URLs**: Get preview URLs for each commit

### Manual Deployments
```bash
vercel --prod
```

## 🛠️ Troubleshooting

### Domain Not Working?
1. **Check DNS propagation**: [whatsmydns.net](https://whatsmydns.net)
2. **Verify nameservers** in GoDaddy
3. **Wait 24-48 hours** for full propagation

### SSL Issues?
1. **Vercel handles SSL automatically**
2. **Check domain status** in Vercel dashboard
3. **Ensure domain is properly connected**

### Performance Issues?
1. **Images optimized**: Already configured in `vercel.json`
2. **Caching enabled**: Static assets cached for 1 year
3. **CDN**: Vercel uses global CDN

## 📞 Support

- **Vercel Support**: [vercel.com/support](https://vercel.com/support)
- **GoDaddy Support**: [godaddy.com/help](https://godaddy.com/help)

## 🎉 Success!

Once completed, your website will be:
- ✅ Live at your custom domain
- ✅ SSL secured (HTTPS)
- ✅ Globally distributed via CDN
- ✅ Auto-deploying on updates
- ✅ Professional and fast

---

**Your LiftCore website will be live and ready to serve customers worldwide!** 🌍 