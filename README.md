

## 🗓️ 4-Week Plan: Build a Blog with **Next.js + Tailwind CSS + TypeScript**

### **Week 1 — Setup & Core Concepts**

**Goal:** Understand Next.js structure, set up Tailwind & TypeScript, and build the skeleton.

#### 🧭 Day 1: Project Setup

* [ ] Install Node.js (LTS) and VS Code
* [ ] Create a new Next.js + TS project

  ```bash
  npx create-next-app@latest my-blog --typescript
  cd my-blog
  npm run dev
  ```
* [ ] Explore the project structure: `/app` or `/pages`, `/public`, `/components`, `/styles`

#### 🧭 Day 2: Add Tailwind CSS

* [ ] Install Tailwind:

  ```bash
  npm install -D tailwindcss postcss autoprefixer
  npx tailwindcss init -p
  ```
* [ ] Configure `tailwind.config.js`:

  ```js
  content: ["./app/**/*.{js,ts,jsx,tsx}", "./pages/**/*.{js,ts,jsx,tsx}", "./components/**/*.{js,ts,jsx,tsx}"]
  ```
* [ ] Add base Tailwind imports in `globals.css`
* [ ] Test with a styled button

#### 🧭 Day 3: Layout Components

* [ ] Create `components/Header.tsx` and `components/Footer.tsx`
* [ ] Add navigation links using `next/link`
* [ ] Wrap pages with a consistent layout (`_app.tsx` or Layout component)

#### 🧭 Day 4: Pages & Routing

* [ ] Create basic pages: `/`, `/about`, `/blog`
* [ ] Learn **file-based routing** and **dynamic routes**
* [ ] Add navigation between them with `<Link>`

#### 🧭 Day 5: Styling & Responsiveness

* [ ] Use Tailwind for a clean responsive layout
* [ ] Set color palette and typography in `tailwind.config.js`
* [ ] Make the header sticky and responsive

---

### **Week 2 — Blog Content & Dynamic Pages**

**Goal:** Display and render Markdown posts dynamically with Next.js SSG.

#### 🧭 Day 6: Markdown Setup

* [ ] Create a `/posts` folder with Markdown files (e.g. `my-first-post.md`)
* [ ] Install dependencies:

  ```bash
  npm install gray-matter remark remark-html
  ```
* [ ] Learn to parse Markdown and frontmatter using `gray-matter`

#### 🧭 Day 7: Dynamic Routing

* [ ] Create `[slug].tsx` inside `/pages/blog`
* [ ] Use `getStaticPaths` + `getStaticProps` to generate pages for each post
* [ ] Render Markdown as HTML

#### 🧭 Day 8: Blog Index Page

* [ ] Use `getStaticProps` to read all Markdown posts
* [ ] Display titles, dates, and excerpts on `/blog`
* [ ] Add links to each post page

#### 🧭 Day 9: SEO & Metadata

* [ ] Add `<Head>` component from `next/head` for each page
* [ ] Include meta title, description, and OpenGraph tags

#### 🧭 Day 10: Polish & Styling

* [ ] Add Tailwind typography plugin:

  ```bash
  npm install @tailwindcss/typography
  ```
* [ ] Style blog post content with `prose` classes
* [ ] Add hover animations for links

---

### **Week 3 — Enhancements & Data Fetching**

**Goal:** Add interactivity, APIs, and structure for scalability.

#### 🧭 Day 11: API Routes

* [ ] Create `/pages/api/posts.ts`
* [ ] Return mock data from API
* [ ] Fetch it on client side with `fetch` and TypeScript interfaces

#### 🧭 Day 12: Client-Side Fetching

* [ ] Use `useEffect` and `useState` for client-side data
* [ ] Compare SSR vs SSG vs CSR in Next.js

#### 🧭 Day 13: TypeScript Improvements

* [ ] Define types for `Post`, `FrontMatter`, and component props
* [ ] Learn how to handle `getStaticProps` types

#### 🧭 Day 14: Category or Tag Filtering

* [ ] Add category/tag fields in Markdown frontmatter
* [ ] Filter posts by category in `/blog`

#### 🧭 Day 15: Styling & Layout Refinement

* [ ] Add grid layout for posts
* [ ] Polish responsiveness & dark mode (optional with Tailwind)

---

### **Week 4 — Deployment & Extras**

**Goal:** Make it production-ready, deploy, and add polish.

#### 🧭 Day 16: Comments (Optional)

* [ ] Add a static comment section (mock or real)
* [ ] Create a controlled form with React hooks

#### 🧭 Day 17: Author & About Section

* [ ] Create author bio component
* [ ] Add `/about` page content

#### 🧭 Day 18: Performance & Accessibility

* [ ] Use `next/image` for optimized images
* [ ] Test with Lighthouse (in Chrome DevTools)

#### 🧭 Day 19: Deployment

* [ ] Push to GitHub
* [ ] Deploy to **Vercel**:

  ```bash
  vercel
  ```
* [ ] Test live site on mobile

#### 🧭 Day 20: Wrap-Up & Next Steps

* [ ] Review code and refactor
* [ ] Optional upgrades:

  * Add a CMS (e.g. Contentlayer, Sanity, or Notion API)
  * Add RSS feed or sitemap
  * Enable analytics

---

### ✅ Final Result

A **responsive, SEO-friendly blog** with:

* Next.js (TypeScript)
* Tailwind CSS styling
* Markdown-based posts
* Static generation (SSG)
* Deployed on Vercel

