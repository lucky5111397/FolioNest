# FolioNest — Developer Portfolio Template

A modern, dark-themed developer portfolio template built with **React 19, Vite, Tailwind CSS, and Framer Motion**.

FolioNest helps developers create their own professional portfolio without starting from scratch. Customize your personal information, skills, projects, experience, education, resume, and social links to make the portfolio your own.

## Features

- **Modern UI:** Responsive dark-mode design with reusable components.
- **Animated Background:** Trace-network visuals with connected nodes and lines.
- **Smooth Animations:** Scroll reveals, page-load animations, and hover interactions.
- **Custom Cursor:** Interactive cursor effects with support for touch devices and smaller screens.
- **Skills Showcase:** Highlight your technical skills, frameworks, and tools.
- **Projects Showcase:** Present projects with descriptions, technologies, repository links, and live demos.
- **Experience & Education:** Showcase your professional experience, education, and certifications.
- **Resume Integration:** Add links to view or download your resume.
- **GitHub Statistics:** Contribution graph and statistics section that can be connected to live data.
- **Contact Section:** Contact form structure ready for email service integration.
- **Responsive Design:** Layout designed for desktop, tablet, and mobile devices.
- **Accessibility:** Keyboard focus states, skip-to-content navigation, and reduced-motion support.
- **SEO & Social Sharing:** Customizable page metadata, favicon, and social preview image.

> Some integrations, including live GitHub statistics and contact form delivery, require additional configuration.

## Tech Stack

| Technology | Purpose |
|---|---|
| React 19 | Component-based UI development |
| Vite | Development server and production builds |
| Tailwind CSS 3 | Styling and design customization |
| Framer Motion | Animations and transitions |
| GSAP | Additional animation capabilities |
| React Icons | Icon library |
| React Scroll | Scroll navigation utilities |

## Getting Started

### Prerequisites

Install the following tools:

- [Node.js](https://nodejs.org/)
- npm, included with Node.js
- Git, for cloning the repository

Verify your installation:

```bash
node -v
npm -v
git --version
```

### 1. Clone the Repository

```bash
git clone https://github.com/lucky5111397/FolioNest.git
cd FolioNest
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Start the Development Server

```bash
npm run dev
```

Open the local URL displayed in your terminal, usually `http://localhost:5173`.

### 4. Build for Production

```bash
npm run build
```

Vite generates the production-ready files in the `dist/` directory.

### 5. Preview the Production Build

```bash
npm run preview
```

Use the URL displayed in your terminal to inspect the production build locally.

## Customization Guide

### 1. Personal Information

Update your name, professional title, introduction, and About section using the relevant files in the project.

If the portfolio data is centralized, edit:

```text
src/data/portfolioData.js
```

Follow the existing data structure to avoid breaking components that consume it.

### 2. Resume

Add your own resume PDF to the `public/` directory.

For example:

```text
public/resume/YourNameResume.pdf
```

Update the corresponding references in the navigation and hero components if the filename or path changes.

### 3. Projects

Add your projects with relevant information, including:

- Project name and description
- Technologies used
- Key features and technical highlights
- GitHub repository URL
- Live demo URL, if available
- Project images, where supported

Replace sample entries with your own work. Do not present placeholder projects as completed projects.

### 4. Skills, Experience & Education

Customize the skills, work experience, education, and certifications sections to reflect your own background.

Remove any sections you do not need while preserving the component structure and references used by the application.

### 5. Social Links

Update your GitHub, LinkedIn, email, and other social links in the relevant configuration or data file.

Remove unused links and test all external URLs before deployment.

### 6. Contact Form

The contact section can be configured for an email service such as EmailJS.

Before using it in production:

1. Configure the required email service and template.
2. Add the required configuration values.
3. Implement appropriate form validation and error handling.
4. Test successful and unsuccessful submissions.

The form should not be assumed to send messages until the integration has been configured and tested. Never expose private credentials in frontend code.

### 7. GitHub Statistics

The GitHub statistics section may use placeholder data until connected to a live source.

To display real statistics, integrate an appropriate GitHub API or statistics service. Handle API errors and rate limits, and never expose a private GitHub token in client-side code.

### 8. Branding & Design

Customize the portfolio's colors, typography, layout, animations, and other visual elements using the relevant project files.

Update these assets as needed:

```text
public/favicon.svg
public/og-image.png
index.html
```

Make sure the favicon, page title, metadata, and Open Graph image reflect your own portfolio.

## Project Structure

```text
FolioNest/
├── public/
│   ├── resume/
│   ├── favicon.svg
│   └── og-image.png
├── src/
│   ├── components/
│   ├── sections/
│   ├── hooks/
│   ├── data/
│   │   └── portfolioData.js
│   ├── App.jsx
│   └── main.jsx
├── index.html
├── package.json
├── tailwind.config.js
└── vite.config.js
```

This is a representative structure. Actual files and directories may vary depending on the version of the project.

## Deployment

FolioNest can be deployed to a static hosting provider that supports Vite applications.

### Vercel

1. Push your repository to GitHub.
2. Import the repository into [Vercel](https://vercel.com/).
3. Configure the following build settings:

   - **Build command:** `npm run build`
   - **Output directory:** `dist`

4. Deploy the application and verify the live website.

### Netlify

1. Import the repository into [Netlify](https://www.netlify.com/).
2. Configure the following build settings:

   - **Build command:** `npm run build`
   - **Publish directory:** `dist`

3. Deploy and test the website.

## Accessibility & Performance

The project incorporates accessibility and performance considerations, including:

- Support for `prefers-reduced-motion`
- Visible keyboard focus states
- Skip-to-content navigation
- Responsive interactions for touch devices
- Opportunities for lazy loading and code splitting

Test these features after making changes. Verify keyboard navigation, mobile layouts, and browser console output before publishing.

## Before Publishing

Use this checklist before deploying your customized portfolio:

- [ ] Replace all sample personal information.
- [ ] Add your own resume and verify its links.
- [ ] Replace placeholder projects with real projects.
- [ ] Update and test social links.
- [ ] Configure and test the contact form.
- [ ] Connect real GitHub statistics or identify placeholder data.
- [ ] Update favicon, page metadata, and social preview image.
- [ ] Test responsive layouts and keyboard accessibility.
- [ ] Run `npm run build` and resolve build errors.
- [ ] Verify the production deployment.

---

**FolioNest — Start with a template. Build your identity. Showcase your work.**
