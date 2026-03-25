# CV Portfolio Site

A clean, fast CV/portfolio site built with Astro and deployed to GitHub Pages.

## Quick Start

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Run locally**
   ```bash
   npm run dev
   ```

3. **Build**
   ```bash
   npm run build
   ```

## Deploy to GitHub Pages

### Option 1: User/Organization Site (username.github.io)
1. Create a new repository named `<username>.github.io`
2. Push this code to the `main` branch
3. Enable GitHub Pages in repository settings
4. The site will be available at `https://<username>.github.io`

### Option 2: Project Site (username.github.io/repo)
1. Create any repository name you prefer
2. Update `astro.config.mjs` to include:
   ```js
   export default defineConfig({
     base: '/your-repo-name/'
   });
   ```
3. Push to `main` branch
4. Enable GitHub Pages
5. Site will be at `https://<username>.github.io/your-repo-name`

## Customize Your CV

Edit the `cv` object in `src/pages/index.astro`:

```js
const cv = {
  name: "Your Name",
  title: "Software Engineer",
  email: "you@example.com",
  phone: "+1 234 567 890",
  github: "https://github.com/username",
  linkedin: "https://linkedin.com/in/username",
  summary: "Your professional summary...",
  experience: [
    {
      company: "Company Name",
      position: "Position",
      period: "2022 - Present",
      description: "Your role description..."
    }
  ],
  education: [
    {
      school: "University Name",
      degree: "Degree Name",
      period: "2016 - 2020"
    }
  ],
  skills: ["JavaScript", "React", "Node.js", "TypeScript"]
};
```

## Technologies

- **Astro** - Static site generator
- **Vanilla CSS** - Clean, minimal styling
- **GitHub Actions** - Automatic deployment
- **GitHub Pages** - Free hosting

## License

MIT
