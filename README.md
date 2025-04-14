# The Indoor Eden Co. - GitHub Pages Website

This is a static website for The Indoor Eden Co., designed to be deployed on GitHub Pages. This website meets the requirements for Amazon Associates program application with all necessary pages (About, Contact, Privacy Policy, and Affiliate Disclosure).

## Deployment Instructions

### First-Time GitHub Users

1. **Create a GitHub Account**
   - Go to [GitHub.com](https://github.com/) and sign up for a free account
   - Verify your email address

2. **Create a New Repository**
   - Click the "+" icon in the top right corner and select "New repository"
   - Name your repository `the-indoor-eden-co`
   - Choose "Public" visibility
   - Leave the "Initialize this repository with" options unchecked
   - Click "Create repository"

3. **Connect Your Local Repository**
   - Open your terminal and navigate to the `github-pages` directory:
     ```bash
     cd github-pages
     ```
   - Connect your local repository to the remote repository on GitHub:
     ```bash
     git remote add origin https://github.com/yourusername/the-indoor-eden-co.git
     ```
     (Replace `yourusername` with your actual GitHub username.)

4. **Push Your Files**
   - Push your local code to the `main` branch of the remote repository:
     ```bash
     git push -u origin main
     ```
   - You may be prompted to enter your GitHub username and personal access token (PAT).

5. **Enable GitHub Pages**
   - Go to your repository settings (click the "Settings" tab)
   - Scroll down to "GitHub Pages" section
   - Under "Source", select the `main` branch
   - Click "Save"
   - It may take a few minutes for your site to be published
   - Once published, GitHub will show you the URL (typically `https://yourusername.github.io/the-indoor-eden-co/`)

### For Experienced GitHub Users

```bash
# Clone the repository you created
git clone https://github.com/yourusername/the-indoor-eden-co.git

# Copy all files from the github-pages directory to your repo
cp -r github-pages/* the-indoor-eden-co/

# Navigate to your repository
cd the-indoor-eden-co

# Add all files to git
git add .

# Commit the changes
git commit -m "Initial website files"

# Push to GitHub
git push origin main
```

Then enable GitHub Pages in the repository settings.

## Using Your Own Domain

If you have a custom domain (like theindooreden.co):

1. Go to your repository settings
2. Scroll down to "GitHub Pages" section
3. Under "Custom domain", enter your domain name and click "Save"
4. Configure your domain's DNS settings:
   - If using an apex domain (example.com), create an A record pointing to GitHub Pages' IP addresses
   - If using a subdomain (www.example.com), create a CNAME record pointing to your GitHub Pages URL
5. Wait for DNS changes to propagate (can take up to 24 hours)

## Customizing the Website

### Images

*   Replace the placeholder images in the `img` folder with your own images
*   For best results, keep the same filenames and dimensions

### Content

*   Edit the HTML files to update content as needed
*   Each page follows the same structure for consistency

### Styling

*   Customize colors and styling in `css/style.css`
*   The site uses CSS variables for easy theming:

```css
:root {
    --primary-color: #4a7c59; /* Main green color */
    --secondary-color: #d8ae5e; /* Accent yellow color */
    /* etc... */
}
```

## Adding a Contact Form

The contact form is currently non-functional as GitHub Pages doesn't support server-side processing. To make it work:

1.  Sign up for a form service like \[Formspree](https://formspree.io/) or \[Netlify Forms](https://www.netlify.com/products/forms/)
2.  Follow their instructions to update the form HTML code

## Need Help?

If you need assistance with this website or want to make custom changes, please reach out at contact@theindooreden.co.
