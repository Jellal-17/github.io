# Personal Portfolio Website

A responsive, multi-page personal portfolio website built with HTML, CSS, and JavaScript. Showcases an introduction hero, about section, educational background, skills, projects, Master's thesis, and a contact form powered by Formspree. Includes mobile-friendly navigation with a hamburger menu, card-based project grid, and GSAP page-enter animations.

## Features
- **Multi-page Layout**: Separate pages for Home, About, Projects, Thesis, and Contact.
- **Responsive Design**: Mobile-first navigation with a hamburger menu; grid-based layouts adapt to various screen sizes.
- **Interactive Nav**: Work dropdown grouping Projects & Thesis links; active-link highlighting.
- **Hero Animations**: Full-screen GSAP overlays on the homepage that animate off on load.
- **Projects Grid**: Card-based layout with hover-to-reveal detailed descriptions, images, and video embeds.
- **Contact Form**: Integrated with [Formspree](https://formspree.io/) for email submissions; includes nmae, email, and message fields.
- **Clean Codebase**: Organised folder structure

## Setup & Local Deployment
1. **Clone the Repository**
   ```
   git clone https://github.com/Jellal-17/github.io.git
   cd github.io
   ```
2. **Install Dependencies**
   - This is a static site; no build tools required.
3. **Run Locally**
   - Simply open `index.html` in your browser, or use a simple HTTP Server:
   ```
   # Python 3
   python3 -m http.server 8000

   # Node.js (http-server)
   npx http-server . -p 8000
   ```
   - Then navigate to `http://localhost:8000`.
4. **Configure Contact Form**
   - Sign up on [Formspree](https://formspree.io/) and replace `action` URL in `contact.html`:
   ```
   <form action="https://formspree.io/f/yourFormId" method="POST" class="contact-form">
   ```

## Customization
- **Theme Colours**: Edit CSS variables in `style.css` under the `:root` selector.
- **Typography**: Uses Poppins from Google Fonts, adjust in the `@import` at the top of `style.css`.
- **Nav Links**: Update `<nav>` in each HTML file to add or remove pages.
- **Projects**: Add, remove, or modify `.card` blocks in `projects.html` to showcase new work.

## Deployment
- **GitHub pages**: Push to `main` branch and enable pages in repository settings.
- **Other Hosts**: Upload the repository folder to any static hosting.

## License
