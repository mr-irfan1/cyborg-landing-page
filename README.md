# 🏛️ Techfest, IIT Bombay - An Aetherial Renaissance
> **30th Edition // Asia's Largest Science & Technology Festival**  
> *Indian Institute of Technology Bombay, Powai, Mumbai*

[![Techfest](https://img.shields.io/badge/Techfest-30th%20Edition-ffd269?style=for-the-badge&logo=react&logoColor=black)](https://techfest.org)
[![Theme](https://img.shields.io/badge/Theme-An%20Aetherial%20Renaissance-4de8ff?style=for-the-badge)](https://techfest.org)
[![Author](https://img.shields.io/badge/Author-Mohammad%20Irfan-ff4655?style=for-the-badge&logo=github)](https://github.com/devirfan)

---

## 🌌 Overview

An ultra-immersive, futuristic fantasy-meets-sci-fi web application inspired by the **IIT Bombay Techfest 30th Edition - "An Aetherial Renaissance"**. 

Built with rich Game UI / HUD design aesthetics, chiseled gold-flame metallic typography, chamfered metallic navigation frames, custom 16:9 atmospheric backdrops, interactive Three.js 3D fire & ember physics, and a full-screen view-switching architecture.

---

## 🎥 Full Video Walkthrough

A high-definition video walkthrough showcasing all 10 full-screen views, 3D lava fire, and interactive systems is available in the assets folder:
- **Video File**: `assets/techfest_full_walkthrough.webp` (Native high-frame animated walkthrough)

---

## ✨ Key Features & Architecture

### 1. 🏰 10 Immersive Full-Screen Views
Rather than small generic popups, every core department of the festival is rendered as a cinematic full-page view with its own dedicated high-resolution atmosphere, radial dark vignettes, and breadcrumb navigation:

| View | Identifier | Atmosphere Backdrop | Focus Area |
| :--- | :--- | :--- | :--- |
| **Citadel Home** | `main-site-view` | `techfest_hero_bg.mp4` | Hero video, 3 Golden Citadel cards, live festival countdown timer, and featured arenas |
| **Official Profile** | `profile-page-view` | `profile_fire_ring_bg.jpg` | Delegate badge, spirit animal element tuning, and real-time registered event tracker |
| **Events & Schedule** | `events-page-view` | `events_celestial_bg.jpg` | Interactive Day 1, 2, and 3 festival itinerary timeline with reminder toasts |
| **CES Quantum Expo** | `ces-page-view` | `ces_quantum_bg.jpg` | Asia's biggest science expo, quantum booths, and delegate pass booking |
| **Contact Secretariat** | `contact-page-view` | `contact_cyber_bg.jpg` | Interactive transmission dispatch form, SAC coordinates, and direct helpline info |
| **About 30th Legacy** | `about-page-view` | `about_renaissance_bg.jpg` | 30-year legacy timeline, UNESCO & UNICEF patronages, and festival milestones |
| **Accommodation** | `accommodation-page-view` | `accommodation_pavilion_bg.jpg` | Lakeside hostel living pavilions, tariff details, and instant reservation booking |
| **Workshops Lab** | `workshops-page-view` | `workshops_lab_bg.jpg` | Renaissance robotics lab, category filters (`Robotics`, `AI`, `Aerospace`, `Cyber`), and 1-click enrollment |
| **Competitions Arena** | `competitions-page-view` | `competitions_arena_bg.jpg` | Robowars colosseum, ₹45L+ prize pool badges, and 6 championship squad registrations |
| **Ignite Venture Summit** | `ignite-page-view` | `ignite_summit_bg.jpg` | Startup pitch amphitheater, 3 strategic pillars (VC Arena, SINE Incubation), and deck application |

---

### 2. 🔥 Three.js 3D Balanced Roaring Lava Fire Engine
- Interactive 3D WebGL fire mesh simulation with simplex noise deformation and custom vertex/fragment shader color-ramping.
- Ascending buoyant ember particle field emitting warm radial lighting onto surrounding elements.
- Perfectly balanced intensity tailored for clean visual readability and high performance (60 FPS).

### 3. 🧭 Seamless Game HUD Navigation
- **Chamfered Top Header**: Fast view-switching buttons (`ACCOMMODATION`, `WORKSHOPS`, `COMPETITIONS`, `IGNITE`, `MOHAMMAD`).
- **Floating Left Dock**: Quick icon launcher for Home, Events, CES Expo, Contact, and About.
- **Floating Socials Dock**: Quick links to developer socials (Instagram, X, LinkedIn, Facebook, Discord).
- **Citadel Quick Hub**: Floating radial coral launcher providing instant access to all 10 views from anywhere.
- **Return to Citadel Breadcrumb**: Back navigation button on all views returning smoothly to the home viewpoint.

### 4. ⚡ Live Reactive State & Feedback
- **Celebration Confetti**: Dynamic particle bursts upon workshop enrollment, competition squad registration, and hostel booking.
- **HUD Toast Dispatcher**: Animated bottom telemetry toasts confirming user actions.
- **Profile Dashboard Sync**: Any workshop or competition registered anywhere across the site instantly reflects in the user's Profile dashboard.

---

## 📁 Clean Folder Structure

```text
/
├── index.html                  # Core application (HTML5, Tailwind, Three.js, GSAP/Canvas logic)
├── favicon.ico                 # Official Techfest IIT Bombay favicon
├── README.md                   # Project documentation
│
└── assets/                     # 16 Active High-Definition Assets
    ├── techfest_logo.png       # Official TF™ Logo
    ├── techfest_hero_bg.mp4    # 1080p Atmospheric Loop Video for Hero Section
    ├── techfest_hero_bg.jpg    # Video Poster Fallback
    ├── techfest_portal_bg.jpg  # Citadel Portal Section Background
    ├── profile_fire_ring_bg.jpg# Profile View Background
    ├── spirit_animal_fire.jpg  # Spirit Animal Fire Kitsune Asset
    ├── events_celestial_bg.jpg # Events & Timeline View Background
    ├── ces_quantum_bg.jpg      # CES Quantum Expo View Background
    ├── contact_cyber_bg.jpg    # Contact Secretariat View Background
    ├── about_renaissance_bg.jpg# About Us 30th Legacy View Background
    ├── accommodation_pavilion_bg.jpg # Accommodation View Background
    ├── workshops_lab_bg.jpg    # Workshops Lab View Background
    ├── competitions_arena_bg.jpg # Competitions Arena View Background
    ├── ignite_summit_bg.jpg    # Ignite Venture Summit View Background
    ├── workshops_thumb.jpg     # Card 2 Workshop Thumbnail
    └── hackathon_thumb.jpg     # Card 2 Competition Thumbnail
```

---

## 🚀 How to Run Locally

### Option 1: Direct Browser Launch
Simply double click `index.html` or open it directly in any modern web browser (Google Chrome, Safari, Edge, Firefox, Brave).

### Option 2: Local HTTP Server (Recommended)
Running through a local web server ensures optimal video decoding and Three.js shader compilation:

```bash
# Using Python 3
python3 -m http.server 3000

# OR using Node.js / npx
npx serve .
```

Then visit:
```
http://localhost:3000/
```

---

## 🛠️ Tech Stack & Libraries

- **HTML5 & Vanilla JavaScript**: Modular zero-dependency architecture.
- **Tailwind CSS (CDN)**: Modern utility classes, glassmorphism, and responsive grid layouts.
- **Three.js (r128)**: 3D procedural fire mesh, vertex noise shaders, and particle motes.
- **Canvas Confetti**: Lightweight particle celebration engine.
- **FontAwesome 6**: Crisp cybernetic and renaissance iconography.
- **Google Fonts**: `Cinzel Decorative`, `Cinzel`, `Space Grotesk`, `Rajdhani`.

---

## 👨‍💻 Author & Credits

- **Developer**: [Mohammad Irfan](https://github.com/devirfan)
  - Instagram: [@devirfan](https://www.instagram.com/devirfan/)
  - Email: [mohammadirfan9403@gmail.com](mailto:mohammadirfan9403@gmail.com)
- **Inspiration**: [Techfest, IIT Bombay](https://techfest.org) - *Asia's Largest Science and Technology Festival*.
