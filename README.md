# Zizi Wallpaper

Zizi Wallpaper is an interactive wallpaper platform built around a simple idea: find a wallpaper that matches what you want to feel or do.

Instead of browsing images only by appearance, visitors can choose a question such as **“Do you want to get things done?”** and explore wallpapers connected to that intention. They can also search, browse categories, save favorites, download images, and talk about wallpapers through comments and replies.

**Live website:** [Explore Zizi Wallpaper](https://ziziwallpaper.vercel.app)

---

## Discover a wallpaper

- Explore wallpapers through visual questions about a goal or feeling.
- Search by title or keyword and browse categories.
- Open a wallpaper to view its images, description, and related suggestions.
- Save favorites to a personal collection.
- Download wallpapers and join conversations through comments and replies.
- Browse on desktop or mobile.

The main gallery loads wallpapers in smaller batches as the visitor scrolls, helping the page handle a growing collection.

---

## Tools and what they do

- **Next.js, React, and TypeScript** — build the pages and interactive features.
- **Tailwind CSS** — create the responsive interface.
- **Firebase Authentication and Firestore** — manage accounts, wallpapers, questions, categories, favorites, and comments.
- **Cloudinary** — store images and deliver versions suited to the gallery, thumbnails, and detail pages.
- **React Hook Form and Zod** — organize and validate content forms in the admin area.
- **Swiper** — navigate between images on a wallpaper detail page.

---

## Image quality and performance

A wallpaper platform needs images to look good without making every page unnecessarily heavy. I learned to deliver different image sizes for different uses: smaller thumbnails, gallery images, and larger detail images.

Cloudinary delivery uses automatic format and quality settings so the displayed image can be more efficient while retaining a good visual result. The download action can use the original image rather than the smaller version shown in the feed.

---

## Content management and protection

The admin area supports managing wallpapers, categories, and question cards. Admins can add and edit content, while the user management area is limited to a super admin.

Image uploads pass through a server API route that checks the admin role and validates image type and size before uploading to Cloudinary. The Cloudinary credentials stay on the server.

Published Firestore security rules separate public and private actions: visitors can view published wallpapers, signed-in users can manage their own favorites and comments, and content management is reserved for admins.

---

## Project screenshots

### 01 — Homepage: Discover Wallpapers

<!-- Add a screenshot of the main wallpaper feed here -->

### 02 — Questions: Choose an Intention

<!-- Add a screenshot of the visual question cards here -->

### 03 — Question Results: Wallpapers for Your Goal

<!-- Add a screenshot of a question result page, such as "Do you want to get things done?" -->

### 04 — Search & Categories: Find a Wallpaper

<!-- Add a screenshot showing search and category navigation here -->

### 05 — Wallpaper Details: View & Download

<!-- Add a screenshot of the image gallery and download action here -->

### 06 — Comments & Replies: Share Thoughts

<!-- Add a screenshot with sample comments and replies here -->

### 07 — Favorites: A Personal Collection

<!-- Add a screenshot of a populated favorites page here -->

### 08 — Admin: Content Overview

<!-- Add a screenshot of the admin homepage here -->

### 09 — Admin: Create or Edit a Wallpaper

<!-- Add a screenshot of the wallpaper form and image controls here -->

### 10 — Admin: Manage Questions & Categories

<!-- Add screenshots of question and category management here -->

### 11 — Mobile Experience

<!-- Add a narrow-screen screenshot of the feed and navigation here -->

---

## My contribution

I developed Zizi Wallpaper as more than an image gallery. I shaped the discovery experience around what a visitor wants from a wallpaper, connecting question cards to relevant images alongside search and categories.

I worked on the interactive experience around each wallpaper, including image viewing, downloads, favorites, and conversations. I also built content management workflows and connected the platform to Firebase and Cloudinary.

---

## What I learned

- **Designing discovery:** How questions, categories, and search offer different ways to find the right image.
- **Image optimization:** How to balance image size and visual quality for feeds and detail pages while preserving the original for downloads.
- **Loading growing collections:** Why paginated wallpaper and comment lists are better than loading everything at once.
- **Community features:** How accounts, favorites, comments, and replies add interaction to a content platform.
- **Access and security:** How to separate public content, user-owned actions, admin tools, and protected image uploads.
