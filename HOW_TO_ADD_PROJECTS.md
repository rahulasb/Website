# 📝 Quick Guide: How to Add a New Project

## Step-by-Step Instructions

### Step 1: Open `index.html`
Open the file `/Users/rahuladhinisatheeshbabu/Desktop/CAREER/PORTWeb/index.html` in your text editor.

### Step 2: Find the Projects Section
Scroll down to around **line 107** where you'll see:
```html
<!-- Project Card 1 -->
<div class="project-card">
```

### Step 3: Copy a Project Card Template
Copy **everything** from one of the existing project cards. For example, copy from **line 107 to line 140** (the entire first project card):

```html
<!-- Project Card 1 -->
<div class="project-card">
    <div class="project-header">
        <div class="project-icon">🔧</div>
        <!-- EDIT THIS: Project name -->
        <h3 class="project-title">Project Name Here</h3>
    </div>
    <!-- EDIT THIS: Project description -->
    <p class="project-description">
        Brief description of your project. Explain what it does, what problem it solves, 
        and what technologies you used. Keep it concise but informative.
    </p>
    <div class="project-tags">
        <!-- EDIT THIS: Add/remove tags as needed -->
        <span class="tag">Python</span>
        <span class="tag">Arduino</span>
        <span class="tag">IoT</span>
    </div>
    <div class="project-links">
        <!-- EDIT THIS: Add your project links (GitHub, demo, etc.) -->
        <a href="https://github.com/yourusername/project" class="project-link" target="_blank">
            <span>GitHub</span>
            <svg width="16" height="16" viewBox="0 0 16 16" fill="none">
                <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z" fill="currentColor"/>
            </svg>
        </a>
        <a href="#" class="project-link" target="_blank">
            <span>Live Demo</span>
            <svg width="16" height="16" viewBox="0 0 16 16" fill="none">
                <path d="M14 9v5H2V2h5M10 2h4v4M6 10l8-8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
            </svg>
        </a>
    </div>
</div>
```

### Step 4: Find Where to Paste
Scroll down to find the comment that says:
```html
<!-- ADD NEW PROJECTS ABOVE THIS LINE -->
```

This is around **line 206**.

### Step 5: Paste Above That Line
**Paste your copied project card ABOVE that comment line.**

### Step 6: Edit Your New Project
Now customize the pasted code:

1. **Change the comment number** (optional):
   ```html
   <!-- Project Card 4 -->
   ```

2. **Change the icon** (line with `project-icon`):
   ```html
   <div class="project-icon">🚀</div>  <!-- Pick any emoji! -->
   ```

3. **Edit the project title**:
   ```html
   <h3 class="project-title">My Awesome Robot</h3>
   ```

4. **Write your description**:
   ```html
   <p class="project-description">
       Built an autonomous robot using Raspberry Pi that can navigate 
       obstacles and follow a line. Implemented computer vision and 
       motor control algorithms.
   </p>
   ```

5. **Update the technology tags**:
   ```html
   <div class="project-tags">
       <span class="tag">Raspberry Pi</span>
       <span class="tag">Python</span>
       <span class="tag">OpenCV</span>
   </div>
   ```

6. **Add your links**:
   ```html
   <a href="https://github.com/YOUR-USERNAME/robot-project" class="project-link" target="_blank">
       <span>GitHub</span>
       ...
   </a>
   ```

### Step 7: Save and Refresh
1. Save the `index.html` file
2. Refresh your browser at `http://localhost:8000`
3. Your new project should appear!

---

## 🎨 Example: Adding a 4th Project

Here's what your code should look like after adding a new project:

```html
</div>  <!-- End of Project Card 3 -->

<!-- Project Card 4 -->
<div class="project-card">
    <div class="project-header">
        <div class="project-icon">🤖</div>
        <h3 class="project-title">Autonomous Line Following Robot</h3>
    </div>
    <p class="project-description">
        Designed and built an autonomous robot using Raspberry Pi that can 
        follow a colored line and avoid obstacles using computer vision.
    </p>
    <div class="project-tags">
        <span class="tag">Raspberry Pi</span>
        <span class="tag">Python</span>
        <span class="tag">OpenCV</span>
        <span class="tag">Motor Control</span>
    </div>
    <div class="project-links">
        <a href="https://github.com/yourusername/robot-project" class="project-link" target="_blank">
            <span>GitHub</span>
            <svg width="16" height="16" viewBox="0 0 16 16" fill="none">
                <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z" fill="currentColor"/>
            </svg>
        </a>
        <a href="https://youtu.be/demo-video" class="project-link" target="_blank">
            <span>Video Demo</span>
            <svg width="16" height="16" viewBox="0 0 16 16" fill="none">
                <path d="M14 9v5H2V2h5M10 2h4v4M6 10l8-8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
            </svg>
        </a>
    </div>
</div>

<!-- ADD NEW PROJECTS ABOVE THIS LINE -->
```

---

## 💡 Tips

### Choosing Emojis for Icons
You can use any emoji! Here are some good ones for engineering projects:
- 🔧 Tools/Hardware
- 💻 Software/Web
- 🤖 Robotics/AI
- ⚙️ Systems/Backend
- 🎮 Games
- 📊 Data/Analytics
- 🌐 Networking
- 📱 Mobile Apps
- 🔐 Security
- 🚀 Innovation

### Adding/Removing Tags
You can add as many technology tags as you want:
```html
<div class="project-tags">
    <span class="tag">Python</span>
    <span class="tag">C++</span>
    <span class="tag">Arduino</span>
    <span class="tag">TensorFlow</span>
    <!-- Add more tags here -->
</div>
```

### Removing a Link
If you don't have a live demo link, just delete that entire `<a>...</a>` block.

### Adding More Links
Want to add a YouTube video or documentation? Copy one of the existing link blocks and change the text:
```html
<a href="https://youtu.be/your-video" class="project-link" target="_blank">
    <span>Video Demo</span>
    <svg width="16" height="16" viewBox="0 0 16 16" fill="none">
        <path d="M14 9v5H2V2h5M10 2h4v4M6 10l8-8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
    </svg>
</a>
```

---

## ❓ Common Issues

**Q: I don't see my new project on the page**
- Make sure you saved the file
- Refresh your browser (Cmd+R or Ctrl+R)
- Check that you pasted it ABOVE the "ADD NEW PROJECTS" comment

**Q: The layout looks broken**
- Make sure you copied the entire `<div class="project-card">...</div>` block
- Check that all opening tags have matching closing tags

**Q: How do I delete a project?**
- Simply delete the entire project card block (from `<!-- Project Card X -->` to the closing `</div>`)

---

## 📚 Same Process for Courses!

The exact same steps work for adding courses:
1. Find a course card (around line 234)
2. Copy the entire block
3. Paste it above the `<!-- ADD NEW COURSES ABOVE THIS LINE -->` comment (around line 354)
4. Edit the course code, title, description, and skills

---

Need more help? Check the [README.md](file:///Users/rahuladhinisatheeshbabu/Desktop/CAREER/PORTWeb/README.md) file for detailed instructions!
