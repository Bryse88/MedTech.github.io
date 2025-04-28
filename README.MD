# Disability Rehabilitation Website

A modern, responsive website for Disability Rehabilitation with a vertical scrolling design, featuring information about a device to help partially able individuals exercise in supine, sitting, and standing positions.

## Features

- Modern, sleek design with vertical scrolling layout
- Responsive design that works on all devices
- Contact form with FormSpree integration
- Blue and white health-focused color scheme
- Ready to deploy on GitHub Pages

## Project Structure

```
disability-rehabilitation/
├── index.html          # Main website file
├── images/             # Image directory
│   └── device-placeholder.jpg
└── README.md           # This documentation
```

## Setting Up Your Website on GitHub Pages

### 1. Create a GitHub Repository

1. Sign in to your GitHub account (or create one at [github.com](https://github.com))
2. Click the "+" icon in the top right and select "New repository"
3. Name your repository either:
   - `your-username.github.io` (will be available at https://your-username.github.io/) 
   - Or any name like `disability-rehabilitation` (will be available at https://your-username.github.io/disability-rehabilitation/)
4. Make sure it's set to "Public"
5. Click "Create repository"

### 2. Upload Your Website Files

#### Option 1: Using GitHub Web Interface

1. Click "Add file" > "Upload files"
2. Drag and drop the HTML file and image folder
3. Click "Commit changes"

#### Option 2: Using Git Commands (for advanced users)

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
# Copy files into this directory
git add .
git commit -m "Initial website files"
git push origin main
```

### 3. Setting Up GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll down to "GitHub Pages" section
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait a few minutes for your site to deploy
7. GitHub will provide you with the URL where your site is published

### 4. Contact Form Setup with FormSpree

The contact form uses [FormSpree](https://formspree.io/), a free service that handles form submissions and forwards them to your email.

1. Go to [FormSpree](https://formspree.io/) and create a free account
2. Create a new form
3. Copy the form ID that FormSpree gives you (it will look something like `xaybdpzk`)
4. Open your `index.html` file
5. Find this line: `<form id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">`
6. Replace `YOUR_FORM_ID` with your actual FormSpree form ID
7. Save the file and upload it to GitHub again

### 5. Customizing Content

1. **Images**: Replace the placeholder image in the "images" folder with your actual device image
2. **Contact Information**: Update the address, phone and email with your actual details
3. **Form Recipients**: FormSpree will forward submissions to the email you registered with their service

## Testing Your Website

Your website will be available at:
- `https://your-username.github.io/` (if using username.github.io repository)
- `https://your-username.github.io/your-repo-name/` (if using a different repository name)

Make sure to test the contact form by submitting a test message.

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [FormSpree Documentation](https://formspree.io/docs/)
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/) for editing this README
