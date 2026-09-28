# Zizi Wallpaper

Zizi Wallpaper is an interactive wallpaper platform where people can discover images, explore collections, save favorites, download wallpapers, and share their thoughts.

I wanted the experience to feel like more than a static image gallery: visitors can search and browse, open a wallpaper for a closer look, and interact around the content.

<!-- Add the live website link here when ready -->

---

## Explore and interact

- Browse published wallpapers and explore categories.
- Search wallpapers by title or keywords.
- Discover content through visual question prompts.
- Open a wallpaper to view its images, description, and related suggestions.
- Download a wallpaper or save it to a personal favorites page.
- Read comments and take part in conversations with replies.
- Use the experience across desktop and mobile screens.

The gallery loads wallpapers in smaller batches as visitors scroll, instead of requesting the entire collection at once.

---

## Tools and what they do

- **Next.js, React, and TypeScript** — build the pages and interactive experience.
- **Tailwind CSS** — style the responsive interface.
- **Firebase Authentication and Firestore** — manage accounts, wallpapers, categories, favorites, questions, and comments.
- **Cloudinary** — store and deliver wallpaper images in sizes suited to different parts of the interface.
- **React Hook Form and Zod** — support structured forms and input validation in the content management interface.
- **Swiper** — provide image navigation on wallpaper detail pages.

---

## Content management and access

The admin area brings together wallpaper, category, and question management. An admin can add and edit content, while access to the admin area is checked on the server.

Image uploads go through a protected API route that checks the admin role and validates the file type and size before sending it to Cloudinary. This keeps the upload credentials on the server.

A separate user management area is reserved for the super admin.

---

## Project screenshots

### 01 — Homepage: Discover Wallpapers

<!-- Add a screenshot of the main wallpaper feed here -->

### 02 — Search & Categories: Find a Style

<!-- Add a screenshot showing search and category navigation here -->

### 03 — Question Prompts: Explore by an Idea

<!-- Add a screenshot of the visual question selection and result page here -->

### 04 — Wallpaper Details: Gallery & Download

<!-- Add a screenshot of a wallpaper detail page here -->

### 05 — Comments & Replies: Community Interaction

<!-- Add a screenshot with sample comments and replies here -->

### 06 — Favorites: Saved Wallpapers

<!-- Add a screenshot of a populated favorites page here -->

### 07 — Profile: Personal Space

<!-- Add a screenshot of the user profile here -->

### 08 — Admin: Content Overview

<!-- Add a screenshot of the admin homepage here -->

### 09 — Admin: Add or Edit a Wallpaper

<!-- Add a screenshot of the wallpaper form and image controls here -->

### 10 — Admin: Categories & Questions

<!-- Add screenshots of category and question management here -->

### 11 — Mobile Experience

<!-- Add a narrow-screen screenshot of the feed and navigation here -->

---

## My contribution

I worked on Zizi Wallpaper as an interactive content platform rather than a simple gallery. The project connects a responsive browsing experience with accounts, favorites, downloads, and conversations around individual wallpapers.

I also worked on the tools behind the public experience: organizing wallpapers with categories and questions, managing content through an admin interface, and handling image uploads and delivery with Cloudinary.

---

## What I learned

- **Content discovery:** How search, categories, visual prompts, and related wallpapers help people explore a growing collection.
- **User interaction:** How favorites, comments, and replies change a gallery into a more participatory experience.
- **Managing larger collections:** Why loading wallpapers and comments in pages matters for usability and data usage.
- **Image handling:** How to upload images through a protected server route and deliver suitable versions for cards and detail views.
- **Access control:** How customer features, admin tools, and super-admin tools need different permissions.
