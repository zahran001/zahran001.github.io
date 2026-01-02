# Portfolio Website - Claude Code Context

> **Project**: Personal Portfolio for Zahran Yahia Khan
> **Type**: Static HTML/CSS/JavaScript Website
> **Hosting**: GitHub Pages (zahran001.github.io)
> **Template Base**: Stellar HTML5 UP (customized)

---

## Project Overview

This is a personal portfolio website showcasing professional experience, projects, education, and career milestones. The site is built with static HTML, custom CSS (with minor responsive tweaks), and jQuery-powered interactions. It's designed to be lightweight, performant, and easy to maintain without build tools.

**Key Purpose**: Present technical expertise, work experience, and project portfolio to recruiters, colleagues, and potential collaborators.

---

## Architecture & Technology Stack

### Core Technologies
- **HTML5**: Semantic markup across 9 pages
- **CSS3**: Compiled from SASS (but currently edited directly in `assets/css/main.css`)
- **JavaScript**: jQuery + custom plugins for navigation and scroll effects
- **Hosting**: GitHub Pages (manual push deployment)

### Dependencies
- jQuery 3.x
- jQuery.scrollex (scroll-triggered events)
- jQuery.scrolly (smooth anchor scrolling)
- Font Awesome 5+ (icons)
- Google Fonts (Source Sans Pro)

### No Build System
- Direct HTML/CSS/JS delivery
- SASS files exist in `assets/sass/` but are **not actively compiled**
- All edits made directly to `assets/css/main.css`
- No package.json, no npm, no bundlers

---

## File Structure

```
zahran001.github.io/
├── index.html                      # Landing page - intro, featured projects, milestones
├── aboutme.html                    # Education & work experience (MOST FREQUENTLY UPDATED)
├── projects.html                   # All projects index
├── project_showcase.html           # Flask portfolio builder project
├── bookatour.html                  # React tour booking app
├── notemart.html                   # React note-sharing platform
├── attendance.html                 # PDF-to-Excel extraction tool
├── lineFollowerRobot.html          # Robotics project
├── more.html                       # Career timeline & reflections (2023-2025)
│
├── assets/
│   ├── css/
│   │   ├── main.css               # PRIMARY STYLESHEET - edit this directly
│   │   ├── noscript.css           # No-JS fallback
│   │   └── fontawesome-all.min.css
│   ├── js/
│   │   ├── main.js                # Custom navigation & scroll logic
│   │   ├── util.js                # jQuery plugins (navList, panel, etc.)
│   │   └── [jquery libraries]     # jQuery core + plugins
│   └── sass/                       # Legacy SASS files (not actively used)
│
├── images/                         # ~30+ project screenshots, photos, logos
│   ├── portrait.jpeg              # Profile photo
│   ├── portfolioImage.jpg         # Header image
│   ├── [project]-[1-5].png        # Project screenshots
│   └── [milestone photos]
│
├── lion-head.png                   # Profile logo
├── rocket-lunch.png                # Favicon
├── LICENSE.txt                     # Template license
├── README.md                       # Basic project info
└── claude.md                       # This file (AI context)
```

---

## Pages & Content Map

### Primary Pages (Update These Most Often)

1. **[aboutme.html](aboutme.html)** - Experience & Education
   - Work experience section (Rocket Mortgage internships, TA roles)
   - Education section (Wayne State University)
   - Tech stack lists
   - **MOST FREQUENTLY UPDATED** - add new roles, skills, education changes here

2. **[projects.html](projects.html)** - Project Index
   - Grid of all projects with descriptions
   - Links to detailed project pages
   - **UPDATE WHEN**: Adding new projects to portfolio

### Project Detail Pages (Link from projects.html)

3. **[bookatour.html](bookatour.html)** - BookATour Project
   - Tech: React, Express.js, MongoDB, PayPal API
   - Features: Tour customization, payment integration

4. **[notemart.html](notemart.html)** - NoteMart Project
   - Tech: React, Appwrite, TanStack Query, Tailwind CSS
   - Features: Note sharing, real-time collaboration

5. **[project_showcase.html](project_showcase.html)** - Portfolio Builder
   - Tech: Flask, Python
   - Features: Dynamic portfolio generation for non-developers

6. **[attendance.html](attendance.html)** - Attendance Sheet Tool
   - Tech: Python, PDF processing
   - Features: Extract student IDs from PDFs to Excel

7. **[lineFollowerRobot.html](lineFollowerRobot.html)** - Robotics Project
   - Tech: Arduino, sensors, algorithms
   - Features: Autonomous line-following robot

### Supporting Pages

8. **[index.html](index.html)** - Landing Page
   - Hero section with intro
   - Featured projects (3 spotlight cards)
   - Quick links to other sections
   - Social/contact links

9. **[more.html](more.html)** - Career Milestones
   - Timeline of achievements (2023-2025)
   - Reflections on internships and growth
   - Photos from events (stadium, corvette, etc.)

---

## Common Tasks & Workflows

### 1. Adding a New Project

**Steps:**
1. Create a new HTML file (e.g., `myproject.html`) by copying an existing project page structure
2. Update the content:
   - Project title and description
   - Technology stack
   - Features list
   - Add screenshots to `images/` directory (name them `myproject1.png`, `myproject2.png`, etc.)
   - Update image references in HTML
3. Add project card to [projects.html](projects.html):
   - Add a new `<article>` block in the projects grid
   - Include thumbnail, title, description, and link to detail page
4. (Optional) Feature on [index.html](index.html) if it's a spotlight project

**Files to Update:**
- `projects.html` - Add project card
- `myproject.html` - New detail page
- `images/` - Add project screenshots
- `index.html` - (Optional) Add to featured projects

---

### 2. Updating Work Experience

**Location:** [aboutme.html](aboutme.html) (around line 78)

**Steps:**
1. Open [aboutme.html](aboutme.html)
2. Find the "Work Experience" section
3. Add new role using existing HTML structure:
   ```html
   <h3>Job Title</h3>
   <p>Company Name | Start Date - End Date</p>
   <ul>
       <li>Responsibility/achievement 1</li>
       <li>Responsibility/achievement 2</li>
   </ul>
   ```
4. Update tech stack section if new technologies were used

**Current Structure:**
- Software Engineer Intern at Rocket Mortgage (Summer 2025)
- Software Engineer Intern at Rocket Mortgage (Summer 2024)
- Teaching Assistant roles (2023-2025)

---

### 3. Updating Education

**Location:** [aboutme.html](aboutme.html)

**Steps:**
1. Find the "Education" section
2. Update degree information, GPA, graduation date
3. Add new certifications or courses if relevant

---

### 4. Updating Tech Stack

**Location:** [aboutme.html](aboutme.html)

**Steps:**
1. Find the skills/tech stack lists
2. Add new technologies, frameworks, or tools
3. Organize by category (languages, frameworks, cloud, databases, etc.)

---

### 5. Responsive CSS Tweaks

**Location:** [assets/css/main.css](assets/css/main.css)

**Approach:**
- Edit `main.css` directly (no SASS compilation needed)
- Focus on media queries for different screen sizes
- Test on multiple devices (mobile, tablet, desktop)

**Breakpoints in Use:**
- xxsmall: < 480px
- xsmall: 480px - 736px
- small: 736px - 980px
- medium: 980px - 1280px
- large: 1280px - 1680px
- xlarge: > 1680px

**Common Tweaks:**
- Font sizes for mobile
- Grid layouts for tablets
- Image scaling
- Navigation behavior

---

### 6. Updating Contact/Social Links

**Locations:**
- [index.html](index.html) - Footer or header section
- [aboutme.html](aboutme.html) - Contact section

**Links Currently Present:**
- LinkedIn
- GitHub
- Resume (external link)
- Email

**Note:** These are functioning fine and low priority for updates.

---

---

## Deployment Workflow

### Current Process: Manual Push

**Steps:**
1. Make changes to HTML/CSS/JS files locally
2. Test in browser (open HTML files directly)
3. Commit changes:
   ```bash
   git add .
   git commit -m "Description of changes"
   ```
4. Push to GitHub:
   ```bash
   git push origin main
   ```
5. GitHub Pages automatically deploys from `main` branch
6. Wait ~1-2 minutes for changes to go live

**No Pre-deployment Scripts:**
- No build step required
- No linting or testing automated (manual review)
- No CI/CD pipeline

---

## Design System & Conventions

### Current Approach
- **No strict naming conventions** - ad-hoc approach works fine for now
- **Responsive-first** - CSS tweaks prioritize cross-device compatibility
- **jQuery-based interactions** - smooth scrolling, navigation effects
- **Component reuse** - copy existing HTML structures for consistency

### CSS Structure (Legacy SASS)
Even though SASS isn't actively compiled, the structure informs the CSS organization:
- **Base**: Page layout, reset, typography
- **Components**: Buttons, forms, boxes, icons, tables
- **Layout**: Header, footer, navigation, main sections
- **Libs**: Breakpoints, mixins, variables

### Color Scheme
- Check `main.css` for color variables (search for hex codes)
- Consistent palette used across all pages
- Dark backgrounds with light text for modern aesthetic

---

## Key JavaScript Files

### [assets/js/main.js](assets/js/main.js)
**Purpose:** Custom navigation and scroll effects
**Key Functions:**
- Responsive breakpoint configuration
- Smooth scroll animation with jQuery.scrolly
- Navigation shrink effect on scroll
- Section activation/deactivation based on scroll position

**Edit When:** Changing navigation behavior, scroll effects, or breakpoints

---

### [assets/js/util.js](assets/js/util.js)
**Purpose:** jQuery utility plugins
**Key Functions:**
- `navList()` - Generates navigation lists from HTML
- `panel()` - Creates collapsible panels
- `placeholder()` - Polyfill for form placeholders (older browsers)
- `prioritize()` - Dynamic element repositioning for responsive design

**Edit When:** Adding new UI components or utilities (rare)

---

## Images & Assets

### Directory: [images/](images/)

**Organization:**
- Profile photos: `portrait.jpeg`, `portfolioImage.jpg`
- Project screenshots: `[project-name][1-5].png`
  - Examples: `attendance1.png`, `note1.png`, `git1.png`
- Milestone photos: `stadium.jpeg`, `corvette.jpeg`, etc.
- Logos: `logo.svg`, `rocket2025.jpeg`

**Adding New Images:**
1. Place in `images/` directory
2. Use descriptive names (lowercase, no spaces)
3. Optimize file size before adding (for fast load times)
4. Reference in HTML with relative path: `images/filename.png`

---

## Projects Showcased

### Current Portfolio Projects

1. **BookATour** - Campus tour customization app
   - React, Express.js, MongoDB, PayPal API
   - User authentication, tour booking, payment processing

2. **NoteMart** - Distraction-free note sharing
   - React, Appwrite, TanStack Query, Tailwind CSS
   - Real-time collaboration, markdown support

3. **Project Showcase** - Portfolio builder for non-developers
   - Flask, Python
   - Dynamic portfolio generation from user input

4. **Attendance Sheet** - PDF processing tool
   - Python, PDF libraries
   - Extract student IDs to Excel format

5. **Line Follower Robot** - Autonomous robotics
   - Arduino, sensors, algorithms
   - PID control, sensor calibration

---

## Career Timeline (more.html)

**Key Milestones:**
- **2025**: Rocket Mortgage internship - Cloud engineering, Kubernetes, AI agents
- **2024**: Rocket Mortgage internship - Full-stack .NET/Angular development
- **2023-Present**: Teaching assistant roles at Wayne State University
- Academic achievements and leadership experiences

---

## Troubleshooting & Tips

### Common Issues

**1. CSS Changes Not Reflecting**
- Hard refresh browser: `Ctrl+F5` (Windows) or `Cmd+Shift+R` (Mac)
- Clear browser cache
- Check file paths in HTML `<link>` tags

**2. jQuery Scroll Effects Not Working**
- Verify jQuery loads before custom scripts in HTML
- Check browser console for JavaScript errors
- Ensure `jquery.scrolly.min.js` and `jquery.scrollex.min.js` are loaded

**3. Images Not Loading**
- Verify file path is correct (relative to HTML file location)
- Check file name capitalization (case-sensitive on some servers)
- Ensure image file exists in `images/` directory

**4. Mobile Responsiveness Issues**
- Edit media queries in `main.css`
- Test with browser dev tools (responsive design mode)
- Check viewport meta tag in HTML `<head>`

**5. GitHub Pages Not Updating**
- Wait 1-2 minutes after push
- Check GitHub Actions tab for deployment status
- Verify pushed to correct branch (`main`)
- Clear browser cache and try incognito mode

---

## Future Considerations

### Potential Migrations (Not Planned Yet)
- **React/Next.js**: If dynamic content or CMS integration needed
- **Build System**: If SASS compilation, minification, or optimization required
- **Contact Form**: If backend integration for form submissions needed
- **Blog Section**: If regular content updates become necessary

**Current Approach is Adequate Because:**
- Static site performs well for portfolio needs
- Manual updates are manageable for infrequent changes
- No build complexity means faster iteration
- GitHub Pages hosting is free and reliable

---

## Quick Reference

### Most Common Edits
1. **Update experience**: [aboutme.html](aboutme.html) - Work Experience section
2. **Add project**: Create `newproject.html` + update [projects.html](projects.html)
3. **Update tech stack**: [aboutme.html](aboutme.html) - Skills section
4. **Fix responsive issues**: [assets/css/main.css](assets/css/main.css) - Media queries
5. **Add images**: Place in [images/](images/) directory

### File Naming Patterns
- Project pages: `projectname.html` (lowercase, no spaces)
- Project images: `projectname1.png`, `projectname2.png`, etc.
- Profile images: Descriptive names (`portrait.jpeg`, `portfolioImage.jpg`)

### Git Workflow
```bash
# After making changes
git status                           # Check what changed
git add .                            # Stage all changes
git commit -m "Updated experience"   # Commit with message
git push origin main                 # Deploy to GitHub Pages
```

---

## Contact & Links

**Portfolio Owner:** Zahran Yahia Khan
**GitHub:** zahran001
**LinkedIn:** [Link in index.html]
**Email:** [Link in index.html]

---

## For Claude Code AI Assistance

When assisting with this project:

1. **Default to editing existing files** rather than creating new ones
2. **Preserve HTML structure** from template (consistent across pages)
3. **Edit CSS directly** in `main.css` (don't try to compile SASS)
4. **Maintain responsive design** when making CSS changes
5. **Test across breakpoints** for mobile/tablet/desktop
6. **Keep jQuery dependencies** intact (don't suggest React refactors unless asked)
7. **Follow existing patterns** for new projects or experience entries
8. **Prioritize performance** (optimize images, minimize dependencies)
9. **Focus on content updates** rather than structural changes (stability matters)
10. **Always provide file paths** as markdown links: [filename.html](path/to/filename.html)

**Most Valuable Assistance:**
- Updating aboutme.html with new experience/education/skills
- Adding new projects (HTML + images + projects.html updates)
- CSS tweaks for responsive design
- Content copywriting improvements
- Accessibility enhancements
- Performance optimization suggestions

---

**Last Updated:** 2025-10-28
**Document Version:** 1.1

---

## Changelog

