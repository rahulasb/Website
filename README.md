# Portfolio Website Customization Guide

## 📍 Where to Edit Your Information

This guide shows you exactly where to customize your portfolio website. All editable sections are marked with `<!-- EDIT THIS: -->` comments in the HTML.

---

## 🏠 **Home Section** (`index.html`)

### Your Name and Title
**Lines 20-21**: Replace with your name
```html
<a href="#home">YourName</a>
```

**Lines 39-40**: Replace with your major/specialization
```html
<span class="circuit-icon">⚡</span>
Computer Engineering Student
```

**Lines 43-44**: Add your full name
```html
<h1 class="hero-title">
    Hi, I'm <span class="gradient-text">Your Name</span>
</h1>
```

### Introduction Paragraph
**Lines 47-51**: Write your personal introduction
```html
<p class="hero-description">
    I am a passionate Computer Engineering student specializing in [Your Specialization]...
</p>
```

### Statistics
**Lines 54-66**: Update your project count, years of experience, and courses
```html
<div class="stat-number">10+</div>  <!-- Number of projects -->
<div class="stat-number">3+</div>   <!-- Years of experience -->
<div class="stat-number">20+</div>  <!-- Number of courses -->
```

---

## 💼 **Projects Section** (`index.html`)

### Finding the Projects Section
Projects start around **line 95** and are contained in individual project cards.

### Editing a Project Card

Each project card has this structure:
```html
<div class="project-card">
    <div class="project-header">
        <div class="project-icon">🔧</div>  <!-- EDIT: Change emoji -->
        <h3 class="project-title">Project Name Here</h3>  <!-- EDIT: Project name -->
    </div>
    <p class="project-description">
        Brief description of your project...  <!-- EDIT: Description -->
    </p>
    <div class="project-tags">
        <!-- EDIT: Add/remove/change tags -->
        <span class="tag">Python</span>
        <span class="tag">Arduino</span>
    </div>
    <div class="project-links">
        <!-- EDIT: Update links -->
        <a href="https://github.com/yourusername/project" ...>
    </div>
</div>
```

### Adding a New Project

1. **Find the template comment** (around line 180):
   ```html
   <!-- TO ADD MORE PROJECTS: ... -->
   ```

2. **Copy an entire project card** (from `<div class="project-card">` to its closing `</div>`)

3. **Paste it before the comment**

4. **Edit the new card**:
   - Change the icon emoji
   - Update the project title
   - Write your project description
   - Modify tags to match your technologies
   - Update GitHub/demo links

---

## 📚 **Courses Section** (`index.html`)

### Finding the Courses Section
Courses start around **line 190**.

### Editing a Course Card

Each course card has this structure:
```html
<div class="course-card">
    <div class="course-code">
        CSE 101  <!-- EDIT: Course code -->
    </div>
    <h3 class="course-title">Introduction to Programming</h3>  <!-- EDIT: Course name -->
    <p class="course-description">
        Brief description of the course...  <!-- EDIT: Description -->
    </p>
    <div class="course-highlights">
        <h4 class="highlights-title">Key Projects & Work:</h4>
        <ul class="highlights-list">
            <!-- EDIT: Add your projects/work -->
            <li>Developed a [project name] that [what it does]</li>
            <li>Implemented [algorithm/system] using [technology]</li>
        </ul>
    </div>
    <div class="course-skills">
        <!-- EDIT: Add/remove skills -->
        <span class="skill-tag">Python</span>
    </div>
</div>
```

### Adding a New Course

1. **Find the template comment** (around line 330):
   ```html
   <!-- TO ADD MORE COURSES: ... -->
   ```

2. **Copy an entire course card** (from `<div class="course-card">` to its closing `</div>`)

3. **Paste it before the comment**

4. **Edit the new card**:
   - Update the course code
   - Change the course title
   - Write the course description
   - Add your key projects/work as list items
   - Update skill tags

---

## 📧 **Contact Section** (`index.html`)

### Finding the Contact Section
Contact information starts around **line 340**.

### Updating Contact Information

```html
<div class="contact-item">
    <div class="contact-icon">📧</div>
    <div>
        <h3>Email</h3>
        <a href="mailto:your.email@example.com">your.email@example.com</a>  <!-- EDIT -->
    </div>
</div>

<div class="contact-item">
    <div class="contact-icon">💼</div>
    <div>
        <h3>LinkedIn</h3>
        <a href="https://linkedin.com/in/yourprofile">linkedin.com/in/yourprofile</a>  <!-- EDIT -->
    </div>
</div>

<div class="contact-item">
    <div class="contact-icon">🔗</div>
    <div>
        <h3>GitHub</h3>
        <a href="https://github.com/yourusername">github.com/yourusername</a>  <!-- EDIT -->
    </div>
</div>
```

### Adding More Contact Methods

Copy a contact item block and change:
- The emoji icon
- The heading (h3)
- The link and text

---

## 🎨 **Customizing Colors** (`styles.css`)

If you want to change the color scheme, edit the CSS variables at the top of `styles.css` (lines 5-20):

```css
:root {
    /* Primary Colors - Electric Blue & Circuit Green */
    --primary: #00d4ff;        /* Main accent color */
    --accent: #00ff88;          /* Secondary accent */
    
    /* Background Colors */
    --bg-primary: #0a0e27;      /* Main background */
    --bg-card: #1a2042;         /* Card backgrounds */
    
    /* Text Colors */
    --text-primary: #ffffff;    /* Main text */
    --text-secondary: #b8c1ec;  /* Secondary text */
}
```

---

## 🚀 **Testing Locally**

1. Open Terminal in the project folder
2. Run: `python3 -m http.server 8000`
3. Open browser to: `http://localhost:8000`

---

## 📤 **Publishing to GitHub Pages**

1. Create a new repository on GitHub
2. Name it: `your-username.github.io`
3. Push these files to the repository:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio website"
   git branch -M main
   git remote add origin https://github.com/your-username/your-username.github.io.git
   git push -u origin main
   ```
4. Go to repository Settings > Pages
5. Set source to "main" branch
6. Your site will be live at: `https://your-username.github.io`

---

## 🔍 **Quick Reference: What to Edit**

| Section | What to Change | Where (approx. line) |
|---------|---------------|---------------------|
| Name | Navigation logo & hero title | Lines 20, 43 |
| Introduction | About you paragraph | Lines 47-51 |
| Stats | Project count, years, courses | Lines 54-66 |
| Projects | Title, description, tags, links | Lines 95-180 |
| Courses | Code, name, description, work | Lines 190-330 |
| Contact | Email, LinkedIn, GitHub | Lines 340-370 |
| Footer | Copyright year & name | Line 385 |

---

## ✨ **Tips for Best Results**

1. **Keep descriptions concise** - 2-3 sentences per project/course
2. **Use specific technologies** - Mention exact tools, languages, frameworks
3. **Add real links** - Replace placeholder URLs with actual project links
4. **Use professional language** - This is showcasing your work
5. **Test on mobile** - The site is responsive, check it on different devices
6. **Update regularly** - Add new projects and courses as you complete them

---

## 🆘 **Need Help?**

- All editable sections have `<!-- EDIT THIS: -->` comments
- Follow the structure of existing cards when adding new ones
- Don't delete structural div tags, only edit content inside them
- Keep opening and closing tags balanced
