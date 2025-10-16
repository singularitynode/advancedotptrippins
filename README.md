Advanced OTP Login - Quantum Glass Authentication
A modern OTP verification interface featuring advanced glassmorphism design with quantum particle effects and 3D interactions.

Features
Visual Design
Realistic glassmorphism effects with multi-layer depth

Quantum particle background animation

Dark/light theme toggle with local storage

Smooth animations and transitions

Interactive Elements
Draggable container with physics-based movement

3D transform effects on hover and drag

Auto-focus input management

Paste support for OTP codes

Security & UX
Input validation (numbers only)

Resend protection with countdown timer

Accessibility features (ARIA labels, keyboard nav)

Error state handling

Quick Start
Direct Usage
Open the HTML file in any modern browser. No build process or dependencies required.

Integration
Copy the HTML structure into your existing project.

Usage
Enter OTP Code

Type the 4-digit code received on your mobile

Inputs auto-advance as you type

Paste full code supported

Theme Toggle

Click the sun/moon icon in top-right corner

Preferences saved in local storage

Move Container

Click and drag the glass panel to reposition

Container has boundary limits

Resend Code

Available after 60-second countdown

Visual confirmation on resend

Technical Features
CSS
Advanced glassmorphism with backdrop-filter

3D transform effects and perspective

CSS custom properties for theming

Responsive design

JavaScript
Quantum particle animation system

Draggable container with physics

Smart input management and validation

Local storage for theme preferences

Customization
Colors & Themes
Modify CSS variables in :root and [data-theme="light"]:

css
--accent-glow: #00d4ff;
--bg-primary: #0c0c0c;
--text-primary: #fff;
OTP Length
Add more input fields to change from 4 to 6 digits.

Browser Compatibility
Chrome 90+ (full support)

Firefox 88+ (full support)

Safari 14+ (full support)

Edge 90+ (full support)

Responsive Design
Desktop: Full 3D effects

Tablet: Optimized touch interactions

Mobile: Streamlined for mobile usage

Integration
With Backend API
Replace the verification handler with your API endpoint:

javascript
verifyBtn.addEventListener('click', async () => {
  const code = getOTPCode();
  const response = await fetch('/api/verify-otp', {
    method: 'POST',
    body: JSON.stringify({ code, userId })
  });
  // Handle response
});
Performance
Single HTML file, no external dependencies

Optimized 60fps animations

Progressive enhancement (works without JavaScript)

License
MIT-Attribution License (Modified)

Copyright (c) 2025 singularitynode

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, subject to the following conditions:

Attribution must be given to the original author:
"Created by singularitynode (https://github.com/singularitynode)"

This notice and the above copyright attribution must be included in all copies
or substantial portions of the Software.

The Software may not be misrepresented as the work of another author or organization.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Contributing
Contributions welcome for:

Additional theme variants

Enhanced accessibility features

Browser compatibility improvements

Known Issues
Mobile Safari: Minor backdrop-filter performance

High-DPI screens: Ensure crisp rendering

Built with modern web technologies and focus on user experience.
