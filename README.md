# 🎨 HubSpot Portfolio Theme

A professional, fully customizable portfolio theme built for HubSpot CMS. This theme includes a hero section, skills showcase, project display, and contact form—all designed to help you create a stunning personal portfolio or professional landing page.

---

## 📋 Project Overview

This HubSpot theme is designed to showcase your work and skills through a modern, responsive interface. It includes four main modules that can be easily customized through HubSpot's drag-and-drop editor:

- **Hero Module**: Display your name, tagline, bio, profile photo, and social media links
- **Skills Module**: Showcase your technical skills with animated progress bars
- **Project Showcase Module**: Highlight your portfolio projects with images, descriptions, and links
- **Contact Module**: Embed a HubSpot form for visitors to get in touch

---

## 📁 Project Structure

```text
hubspot-project/
├── modules/
│   ├── Contact_Module.module/
│   │   ├── fields.json
│   │   ├── meta.json
│   │   ├── module.css
│   │   ├── module.html
│   │   └── module.js
│   ├── Hero Module.module/
│   │   ├── fields.json
│   │   ├── meta.json
│   │   ├── module.css
│   │   ├── module.html
│   │   └── module.js
│   ├── Project_Showcase.module/
│   │   ├── fields.json
│   │   ├── meta.json
│   │   ├── module.css
│   │   ├── module.html
│   │   └── module.js
│   └── skills_module.module/
│       ├── fields.json
│       ├── meta.json
│       ├── module.css
│       ├── module.html
│       └── module.js
├── templates/
│   └── portfolio-landing.html
├── fields.json
└── theme.json
```

---

## 🚀 Quick Start

### 1. Install HubSpot CLI

```bash
npm install -g @hubspot/cli
```

### 2. Authenticate with HubSpot

```bash
hs auth
```

Follow the prompts to connect to your HubSpot account.

### 3. Upload the Theme

```bash
hs upload hubspot-project hubspot-project
```

### 4. Create a New Page

1. Navigate to **Marketing** > **Website** > **Website Pages**
2. Click **Create** > **Website Page**
3. Select the **portfolio-landing** template
4. Customize the modules using the page editor
5. Publish your page

---

## 📖 Full Documentation

### Hero Module

**Customizable Fields:**
- **Name**: Your full name or professional title
- **Tagline**: A catchy subtitle or role description
- **Bio Description**: Rich text area for your professional bio
- **Profile Photo**: Upload your professional headshot
- **Background Color**: Customize the section background
- **Reverse Layout**: Toggle to flip image and text positions
- **Social Links**: Add URLs for LinkedIn, GitHub, Email, and Facebook

**Features:**
- Responsive design that adapts to mobile and tablet devices
- Animated social media icons with hover effects
- Google Fonts integration (Roboto family)

### Skills Module

**Customizable Fields:**
- **Section Title**: Heading for your skills section
- **Background Color**: Customize the section background
- **Skills**: Repeatable group field where you can add:
  - Skill Name
  - Skill Level (0-100%)

**Features:**
- Animated progress bars showing skill proficiency
- Two-column grid layout (responsive to single column on mobile)
- Color-coded progress indicators

### Project Showcase Module

**Customizable Fields:**
- **Project Title**: Name of your project
- **Project Description**: Rich text description of the project
- **Project Image**: Screenshot or preview image
- **Project Link**: External or internal link to the live project
- **Card Background Color**: Customize individual project card colors

**Features:**
- Hover animations for enhanced interactivity
- Flexible layout that adapts to screen size
- "View Project" call-to-action button

### Contact Module

**Customizable Fields:**
- **Section Title**: Heading for the contact section
- **Section Description**: Rich text intro or instructions
- **Contact Form**: Connect a HubSpot form via form selector
- **Background Color**: Customize the section background

**Features:**
- Native HubSpot form integration
- Inline form submission responses
- Fully styled form inputs with focus states

---

## ✨ Features

- [x] Fully responsive design (mobile, tablet, desktop)
- [x] Drag-and-drop page builder support
- [x] Google Fonts integration
- [x] Customizable color schemes per module
- [x] Social media icons with hover effects
- [x] Animated skill progress bars
- [x] HubSpot form integration
- [x] SEO-friendly HTML structure
- [x] Accessibility features (ARIA labels, semantic HTML)
- [x] Fast loading with optimized CSS

---

## 🛠️ Development

### Local Development Setup

1. Clone or download the project
2. Ensure you have Node.js and npm installed
3. Install HubSpot CLI globally:

```bash
npm install -g @hubspot/cli
```

4. Authenticate with your HubSpot account:

```bash
hs auth
```

5. Use watch mode to automatically sync changes:

```bash
hs watch hubspot-project hubspot-project
```

### File Structure Explained

- **fields.json**: Defines the customizable fields in the module editor
- **meta.json**: Contains module metadata (ID, content types, availability)
- **module.css**: Styles for the module
- **module.html**: HubL template markup
- **module.js**: JavaScript for interactive features (if needed)

### Customization Tips

- Modify CSS files to change colors, fonts, and spacing
- Update `fields.json` to add new customizable options
- Edit HubL templates in `module.html` for layout changes
- Use HubSpot's design manager for live preview

---

## ✅ Requirements Met

- [x] **Hero Section**: Profile photo, name, tagline, bio, and social links
- [x] **Skills Section**: Dynamic skill bars with percentage levels
- [x] **Projects Section**: Showcase multiple projects with images and links
- [x] **Contact Section**: Integrated HubSpot form
- [x] **Responsive Design**: Works seamlessly on all devices
- [x] **Customizable**: All content editable through HubSpot's UI
- [x] **Modern Design**: Clean, professional aesthetic
- [x] **SEO Optimized**: Proper HTML semantics and meta tag support

---

## 🐛 Troubleshooting

### Module Not Appearing in Editor

- Ensure `is_available_for_new_content` is set to `true` in `meta.json`
- Check that the module is properly uploaded to HubSpot
- Clear your browser cache and refresh the page editor

### Styles Not Loading

- Verify the CSS file is uploaded correctly
- Check for syntax errors in your CSS
- Ensure the module is using the correct CSS file path

### Form Not Displaying

- Confirm you've selected a valid HubSpot form in the module settings
- Ensure the form ID exists in your HubSpot account
- Check form permissions and publication status

### Upload Errors

- Verify your HubSpot CLI is authenticated: `hs auth`
- Check your internet connection
- Ensure you have the correct permissions in your HubSpot account

---

## 📚 Resources

- [HubSpot CMS Documentation](https://developers.hubspot.com/docs/cms)
- [HubSpot CLI Documentation](https://developers.hubspot.com/docs/cms/developer-reference/local-development-cli)
- [HubL Template Language](https://developers.hubspot.com/docs/cms/hubl)
- [HubSpot Design Manager](https://knowledge.hubspot.com/design-manager/design-manager-overview)
- [Module Development Guide](https://developers.hubspot.com/docs/cms/building-blocks/modules)

---

## 📄 License

This project is open source and available for personal and commercial use.

---

## 👤 Author

Created with ❤️ for the HubSpot developer community

---

**Need Help?** Feel free to open an issue or reach out through the contact form on your portfolio site!
