# Notes Blog

A simple, clean blog built with Docusaurus and deployed to GitHub Pages. This blog uses a custom `YYYY/MM/DD/post-title.md` structure for organizing posts chronologically.

## Features

- ✅ **Blog as Main Page**: Blog is the homepage at `/notes` (not `/notes/blog`)
- ✅ **Custom Blog Structure**: Posts organized in `YYYY/MM/DD/post-title.md` format
- ✅ **Author Profiles**: Configured author profiles with social links
- ✅ **Tag System**: Organize posts with tags for easy discovery
- ✅ **RSS/Atom Feeds**: Automatic feed generation for subscribers
- ✅ **GitHub Pages Deployment**: Automated deployment via GitHub Actions
- ✅ **Responsive Design**: Works perfectly on desktop and mobile
- ✅ **Dark/Light Mode**: Automatic theme switching based on user preference
- ✅ **SEO Optimized**: Built-in SEO features for better search visibility

## Quick Start

### Prerequisites

- Node.js 20 or higher
- npm or yarn
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/kolsha/notes.git
   cd notes
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## Creating Blog Posts

### Directory Structure

This blog uses a custom directory structure for organizing posts:

```
blog/
├── 2025/
│   ├── 10/
│   │   ├── 19/
│   │   │   └── welcome.md
│   │   └── 20/
│   │       └── my-new-post.md
│   └── 11/
│       └── 01/
│           └── another-post.md
├── authors.yml
└── tags.yml
```

### Creating a New Post

1. **Create the directory structure**
   ```bash
   mkdir -p blog/YYYY/MM/DD
   ```

2. **Create your post file**
   ```bash
   touch blog/YYYY/MM/DD/your-post-title.md
   ```

3. **Add frontmatter to your post**
   ```markdown
   ---
   slug: your-post-title
   title: Your Post Title
   authors: [kolsha]
   tags: [tag1, tag2, tag3]
   ---
   
   # Your Post Title
   
   Your post content goes here...
   ```

### Frontmatter Options

- `slug`: URL-friendly version of your title (optional, auto-generated from filename)
- `title`: The display title of your post
- `authors`: Array of author keys from `blog/authors.yml`
- `tags`: Array of tags for categorizing your post
- `description`: Optional description for SEO
- `image`: Optional featured image for the post

## Deployment

### GitHub Pages Setup

1. **Create a GitHub repository**
   - Create a new repository named `notes` on GitHub
   - Push your code to the `main` branch

2. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: "GitHub Actions"
   - The deployment workflow will automatically deploy your site

3. **Access your site**
   - Your blog will be available at: `https://kolsha.github.io/notes/`
   - The blog is the main page (no `/blog` subdirectory needed)

### Manual Deployment

If you prefer manual deployment:

```bash
# Build the site
npm run build

# Deploy to GitHub Pages
npm run deploy
```

## Configuration

### Site Configuration

Edit `docusaurus.config.ts` to customize:

- Site title and description
- Navigation menu
- Footer links
- Social media links
- Theme colors

### Author Configuration

Edit `blog/authors.yml` to add or modify authors:

```yaml
kolsha:
  name: Kolsha
  title: Blog Author
  url: https://github.com/kolsha
  image_url: https://github.com/kolsha.png
  page: true
  socials:
    github: kolsha
    twitter: your_twitter_handle
    linkedin: your_linkedin_profile
```

### Custom Domain

To use a custom domain:

1. **Add a CNAME file**
   ```bash
   echo "yourdomain.com" > static/CNAME
   ```

2. **Update docusaurus.config.ts**
   ```typescript
   url: 'https://yourdomain.com',
   baseUrl: '/',
   ```

3. **Configure DNS**
   - Add a CNAME record pointing to `kolsha.github.io`

## Development

### Available Scripts

- `npm start`: Start development server
- `npm run build`: Build for production
- `npm run serve`: Serve built site locally
- `npm run deploy`: Deploy to GitHub Pages
- `npm run clear`: Clear Docusaurus cache

### Project Structure

```
├── blog/                    # Blog posts directory
│   ├── YYYY/MM/DD/         # Date-based organization
│   ├── authors.yml         # Author profiles
│   └── tags.yml            # Tag definitions
├── docs/                   # Documentation (optional)
├── src/                    # Source code
│   ├── components/         # React components
│   ├── css/               # Custom styles
│   └── pages/             # Additional pages
├── static/                # Static assets
├── docusaurus.config.ts   # Main configuration
└── package.json          # Dependencies and scripts
```

## Customization

### Styling

- Edit `src/css/custom.css` for custom styles
- Modify theme colors in `docusaurus.config.ts`
- Add custom components in `src/components/`

### Layout

- Customize the homepage in `src/pages/index.tsx`
- Add new pages in `src/pages/`
- Modify navigation in `docusaurus.config.ts`

## Troubleshooting

### Common Issues

1. **Build fails**: Check for syntax errors in markdown files
2. **Images not loading**: Ensure images are in the `static/` directory
3. **Deployment fails**: Verify GitHub Pages settings and repository permissions

### Getting Help

- [Docusaurus Documentation](https://docusaurus.io/docs)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Create an issue](https://github.com/kolsha/notes/issues) for bugs or questions

## License

This project is open source and available under the [MIT License](LICENSE).

---

Built with ❤️ using [Docusaurus](https://docusaurus.io/) and deployed to [GitHub Pages](https://pages.github.com/).