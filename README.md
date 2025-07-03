# Innovation Blog - Static Frontend with Container Backend

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/Fadil369/static-frontend-container-backend)

<!-- dash-content-start -->

This is a modern static blog web page designed for deployment on Cloudflare Pages. The blog features separate categories for healthcare improvements, technology development, and business innovations. It includes a [Container](https://developers.cloudflare.com/containers/) backend template for API functionality.

<!-- dash-content-end -->

## Blog Features

- **Healthcare Improvements**: Explore innovations in medical technology, patient care, and healthcare systems
- **Tech Development**: Stay updated with software development, emerging technologies, and digital transformation
- **Business Improvements**: Learn about strategic business improvements and operational efficiency
- **Responsive Design**: Fully responsive layout that works on all devices
- **SEO Optimized**: Proper meta tags and structured content for search engine optimization
- **Scalable Architecture**: Easy to add new blog categories and posts

## Blog Structure

```
dist/
├── blog.html              # Main blog homepage
├── categories/
│   ├── healthcare.html    # Healthcare category page
│   ├── tech.html         # Technology category page
│   └── business.html     # Business category page
├── posts/
│   └── ai-powered-diagnostics.html  # Sample blog post
├── styles/
│   └── blog.css          # Blog styling
└── scripts/
    └── navigation.js     # Navigation functionality
```

## Getting Started

First, install dependencies:

```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

Then run the development server:

```bash
npm run dev
```

Open [http://localhost:8787](http://localhost:8787) with your browser to see the result.

- Visit [http://localhost:8787/blog.html](http://localhost:8787/blog.html) to see the blog homepage
- Visit [http://localhost:8787/categories/healthcare.html](http://localhost:8787/categories/healthcare.html) for healthcare posts
- Visit [http://localhost:8787/categories/tech.html](http://localhost:8787/categories/tech.html) for technology posts
- Visit [http://localhost:8787/categories/business.html](http://localhost:8787/categories/business.html) for business posts

You can start editing the blog by modifying files in the `/dist` directory:
- Edit `blog.html` for the main homepage
- Edit category pages in `/dist/categories/`
- Add new blog posts in `/dist/posts/`
- Customize styling in `/dist/styles/blog.css`

## Deployment

### Deploying to Cloudflare Pages

1. **Via Cloudflare Dashboard:**
   - Log into your Cloudflare dashboard
   - Go to Pages and click "Create a project"
   - Connect your GitHub repository
   - Set build settings:
     - Build command: `echo "Static site - no build required"`
     - Build output directory: `dist`
   - Deploy

2. **Via Wrangler CLI:**
   ```bash
   npm run deploy
   ```

### Deploying to Other Static Hosting Providers

The blog is a static site located in the `/dist` directory and can be deployed to any static hosting provider:

- **Netlify**: Drag and drop the `/dist` folder or connect your repository
- **Vercel**: Import your repository and set the output directory to `dist`
- **GitHub Pages**: Enable GitHub Pages and set the source to the `/dist` folder

## Adding New Blog Posts

1. Create a new HTML file in `/dist/posts/`
2. Follow the structure of existing posts like `ai-powered-diagnostics.html`
3. Add the post to the appropriate category page
4. Update the featured posts section on the homepage if desired

## Adding New Categories

1. Create a new category page in `/dist/categories/`
2. Follow the structure of existing category pages
3. Add the category to the navigation menu in all HTML files
4. Add the category card to the homepage
5. Update the footer links

## Customization

- **Colors**: Edit CSS variables in `/dist/styles/blog.css`
- **Fonts**: Update Google Fonts imports in HTML files
- **Layout**: Modify the grid layouts and responsive breakpoints
- **Content**: All content is in HTML files for easy editing

## Container Backend (Optional)

This template also includes a containerized Go backend for API functionality:

- Backend source code: `/container_src/`
- API endpoint: `/api/widgets`
- Container configuration: `Dockerfile`

You can start editing your Worker by modifying `src/index.ts` and your Container backend by editing the content of `container_src`.

## Learn More

To learn more about the technologies used:

- [Cloudflare Pages Documentation](https://developers.cloudflare.com/pages/)
- [Container Documentation](https://developers.cloudflare.com/containers/)
- [Wrangler CLI Documentation](https://developers.cloudflare.com/workers/wrangler/)

Your feedback and contributions are welcome!
