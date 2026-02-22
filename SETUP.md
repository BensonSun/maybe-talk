# Maybe She'd Like to Talk — Setup Guide

## Cal.com Booking System Setup

### Step 1: Create Cal.com Account
1. Go to https://cal.com and sign up (free plan is enough to start)
2. Complete your profile

### Step 2: Create Event Type
1. Go to "Event Types" in the sidebar
2. Click "New Event Type"
3. Settings:
   - **Title**: `聊聊 / Talk Session`
   - **Duration**: 45 minutes
   - **Location**: Zoom (you'll connect Zoom in the next step)
   - **Description**: 一對一的線上聊聊，45 分鐘。/ A 1:1 online talk session, 45 minutes.

### Step 3: Connect Zoom
1. Go to "Apps" in the sidebar
2. Search for "Zoom"
3. Click "Install" and authorize with your Zoom account
4. Now every booking will auto-generate a Zoom link

### Step 4: Set Availability
1. Go to "Availability" in the sidebar
2. Set your available time slots (e.g., Mon-Fri 10am-6pm)
3. Set your timezone

### Step 5: Update Website Code
1. Open `index.html`
2. Find the line that says `calLink: "YOUR_USERNAME/YOUR_EVENT"`
3. Replace it with your actual Cal.com link, e.g., `calLink: "annie/talk-session"`
4. The booking calendar will now show up on the website

### Step 6: First Session Free
Option A (Simple): Just don't set a price — all bookings are free by default
Option B (Future paid): Enable "Payments" in Cal.com, set a price, and create a separate free event type for first-timers

## Deploying the Website

### Option A: Vercel (Recommended)
1. Create a GitHub repo and push the code
2. Go to https://vercel.com and import the repo
3. It deploys automatically

### Option B: Netlify
1. Go to https://netlify.com
2. Drag and drop the project folder
3. Done

### Domain
Once you decide on the domain name (e.g., maybeshedliketotalk.com), you can connect it in Vercel/Netlify settings.

## File Structure
```
maybe-talk/
├── index.html          — Main website (single page)
├── illustrations/       — AI-generated illustrations
│   ├── 01-meditation-v2.png
│   ├── 02-talking-v2.png
│   └── 03-sleep-v2.png
├── screenshots/         — Development screenshots
└── SETUP.md            — This file
```
