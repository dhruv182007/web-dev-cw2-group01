# FitZone - Your Ultimate Fitness Destination

A modern, responsive fitness gym website showcasing membership plans, fitness classes, workout programs, and a comprehensive membership registration system.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Pages](#pages)
- [Technologies Used](#technologies-used)
- [Key Features Breakdown](#key-features-breakdown)
- [Browser Compatibility](#browser-compatibility)

## Project Overview

FitZone is a fully responsive website for a modern fitness gym that helps potential members explore membership options, view available fitness classes, learn about workout programs, and register for membership. The site is built with vanilla HTML, CSS, and JavaScript (with jQuery for DOM manipulation).

**Authors:** Dhruv Jaswal, Muhammad Shoaib Khan, Ramesh Budha

## Features

✅ **Responsive Design** - Mobile-first approach, works seamlessly on all devices  
✅ **Multiple Membership Plans** - Basic ($29), Premium ($59), and Elite ($99) options  
✅ **Fitness Classes Gallery** - 6 different class types with hover effects  
✅ **Interactive Workout Programs** - Detailed exercises for 4 muscle groups (Chest, Back, Legs, Shoulders)  
✅ **BMI Calculator** - Calculate body mass index during registration  
✅ **Form Validation** - Client-side validation with error messaging  
✅ **Cookie Consent** - GDPR-compliant cookie consent banner  
✅ **Dark Mode Support** - localStorage-based theme preference  
✅ **Accessibility** - ARIA labels, semantic HTML, skip links  
✅ **Smooth Animations** - Interactive hover effects and transitions  

## File Structure

```
FitZone/
├── index.html              # Home page with pricing and features
├── classes.html            # Fitness classes gallery
├── workouts.html           # Interactive workout programs
├── join.html               # Membership registration form
├── css/
│   ├── styles.css          # Main stylesheet
│   ├── animations.css      # Animation effects
│   ├── workouts.css        # Workout page specific styles
│   └── forms.css           # Form styling
├── js/
│   ├── main.js             # Cookie consent, date/time, utilities
│   ├── validate.js         # Form validation logic
│   ├── workouts.js         # Workout page interactivity
│   └── bmi.js              # BMI calculator
├── images/
│   ├── favicon.png         # Site favicon
│   ├── background.jpg      # Hero background
│   ├── gallery/            # Class images (yoga, spin, hiit, boxing, pilates, crossfit)
│   └── workouts/           # Muscle group images (chest, back, legs, shoulders)
└── README.md               # This file
```

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No server setup required - this is a static site

### Installation

1. **Clone or download the project:**
   ```bash
   git clone <repository-url>
   cd FitZone
   ```

2. **Open in browser:**
   - Double-click `index.html`, or
   - Right-click and select "Open with" your preferred browser, or
   - Use a local server for best results:
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Python 2
     python -m SimpleHTTPServer 8000
     
     # Using Node.js http-server
     npx http-server
     ```

3. **Navigate to:**
   - `http://localhost:8000` (or your server address)

## Pages

### Home Page (index.html)
The landing page featuring:
- **Hero Section** - Compelling tagline and call-to-action
- **Membership Plans** - Three pricing tiers with feature comparison
- **Why Choose Us** - Key differentiators (Expert Trainers, Modern Equipment, Community, Flexible Classes)
- **Navigation** - Easy access to all site sections

### Classes Page (classes.html)
Showcases available fitness classes:
- **Gallery Grid** - 6 fitness class types with images
- **Class Types:**
  - Yoga - Find your inner peace
  - Spin - High-energy cardio workout
  - HIIT - Intense interval training
  - Boxing - Build strength and confidence
  - Pilates - Core strength and flexibility
  - CrossFit - Functional fitness training
- **Class Information** - Details about beginner-friendly approach, schedules, instructors, and community

### Workouts Page (workouts.html)
Interactive workout program guide featuring:
- **Auto-rotating Carousel** - Showcases workout types
- **Muscle Group Selection** - Choose from Chest, Back, Legs, or Shoulders
- **Accordion Exercises** - Expandable exercise details with:
  - Sets and reps
  - Rest periods
  - Step-by-step instructions
- **Cookie Consent Banner** - GDPR compliance notification

### Join Page (join.html)
Comprehensive membership registration form with:
- **Membership Plan Selection** - Radio buttons for Basic, Premium, or Elite
- **Personal Information** - Name, email, phone, date of birth
- **Health & Fitness Information** - Height, weight, BMI calculator, fitness level
- **Medical Information** - Optional field for conditions/injuries
- **Address Information** - Full address with street, city, state, postal code
- **Agreements** - Terms & Conditions and Privacy Policy checkboxes
- **Success Confirmation** - Displays submitted information upon registration

## Technologies Used

### Frontend
- **HTML5** - Semantic markup, form elements, accessibility features
- **CSS3** - Flexbox, Grid, responsive design, animations, transitions
- **JavaScript (ES6)** - DOM manipulation, form handling, local storage
- **jQuery 3.6.0** - Simplified DOM manipulation and animations

### Key Libraries
- jQuery - DOM selection and manipulation
- HTML5 Form API - Native form validation

### Development Tools
- Git - Version control
- VS Code / Text Editor - Development

## Key Features Breakdown

### 1. Responsive Design
- Mobile-first approach using CSS media queries
- Flexbox and Grid layouts
- Touch-friendly buttons and interactive elements

### 2. Form Validation
- Real-time client-side validation
- Custom error messages for each field
- Email, phone, and postal code pattern validation
- Age verification via date of birth
- BMI calculation from height and weight

### 3. Cookie Consent (GDPR Compliance)
- Banner appears after 2 seconds on first visit
- localStorage-based consent tracking
- 365-day cookie persistence
- Accept/Decline options

### 4. Local Storage Features
- Cookie consent preferences
- Dark mode preference (ready to use)
- Last viewed workout tracking
- Form data persistence (optional)

### 5. Accessibility
- Semantic HTML structure
- ARIA labels and descriptions
- Skip links for keyboard navigation
- Form error announcements with aria-live
- Proper heading hierarchy

### 6. Animations & Interactions
- Smooth page transitions
- Hover effects on buttons and cards
- Carousel auto-rotation with manual controls
- Accordion expand/collapse animations
- Gallery overlay effects

## Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome  | ✅ Full |
| Firefox | ✅ Full |
| Safari  | ✅ Full |
| Edge    | ✅ Full |
| IE 11   | ⚠️ Limited |

**Note:** For best experience, use a modern browser with ES6 support.

## Contact

**Email:** info@fitzone.com  
**Phone:** (555) 123-4567

## License

© 2024 FitZone. All rights reserved.

---

## Development Notes

### Common Tasks

**Adding a New Fitness Class:**
1. Add class image to `images/gallery/`
2. Create new gallery-item div in `classes.html`
3. Update styling in `css/styles.css` if needed

**Adding Workout Exercises:**
1. Edit the accordion section in `workouts.html`
2. Update `js/workouts.js` if adding new muscle groups
3. Add corresponding accordion styling

**Form Customization:**
1. Edit form fields in `join.html`
2. Update validation rules in `js/validate.js`
3. Adjust form styling in `css/forms.css`

### Performance Tips
- Images are optimized JFIF format
- CSS and JS are minified for production
- jQuery is loaded from CDN for faster delivery
- Local storage reduces repeated API calls

### Future Enhancement Ideas
- Backend integration for form submission
- Member dashboard/portal
- Booking system for classes
- Email notifications
- Payment processing
- Mobile app

---

**Last Updated:** 2026  
**Version:** 1.0.0
