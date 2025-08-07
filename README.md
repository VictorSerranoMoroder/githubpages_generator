# Github Pages Generator

## Step 1: Setup hexo and dependencies

```
hexo init my-page
cd my-page
npm install
```

## Step 2: Install Icarus Theme
From your blog root directory:
```
git clone https://github.com/ppoffice/hexo-theme-icarus themes/icarus
```
Then, update _config.yml to use the Icarus theme:
```
theme: icarus
```

Now install the theme dependencies (probably you will need more...):
```
npm install --save hexo-generator-feed hexo-generator-sitemap hexo-generator-archive
```
You can customize the theme via themes/icarus/_config.yml.

## Step 3: Customize blog
Edit these files:
`_config.yml`: Site-wide config (title, URL, deployment)
`themes/icarus/_config.yml`: Theme-specific config
`source/_posts/`: Add .md files here for new blog posts

Example post:

```
hexo new "My First Post"
```

## Step 4: Deploy to Github Pages
1. Create a new GitHub repository called yourusername.github.io.
2. Install Hexo deployer:

```
npm install --save hexo-deployer-git
```

3. Generate and deploy:
```
hexo clean
hexo generate
hexo deploy
```
💡 Make sure the main branch contains only the generated public/ folder.

**Optional tips**
- Local preview:
```
hexo serve
```