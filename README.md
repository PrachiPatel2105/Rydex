# Rydex

Rydex is a role-based vehicle rental and ride booking platform built with Next.js, React, and MongoDB.

## Overview

The application supports three main experiences: customer booking, partner operations, and admin review workflows. It includes search, booking, payment, live ride tracking, partner onboarding, video KYC, and real-time communication in a single platform.

## Core Capabilities

- Role-based flows for user, partner, and admin accounts
- Vehicle search, booking, checkout, and ride tracking
- Partner onboarding, vehicle management, and earnings view
- Admin review and approval for partners, vehicles, and video KYC
- Real-time chat and location updates through a separate Socket.io service
- Geospatial vehicle discovery using MongoDB and map-based interfaces

## Tech Stack

| Tech | Purpose |
| --- | --- |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" alt="Next.js" width="18" /> Next.js | App framework and routing |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="React" width="18" /> React | UI layer |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" alt="TypeScript" width="18" /> TypeScript | Type safety |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-original.svg" alt="Tailwind CSS" width="18" /> Tailwind CSS | Styling |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redux/redux-original.svg" alt="Redux Toolkit" width="18" /> Redux Toolkit | Client state |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" alt="MongoDB" width="18" /> MongoDB | Primary database |
| <img src="https://api.iconify.design/mdi:database-outline.svg" alt="Mongoose" width="18" /> Mongoose | Data modeling |
| <img src="https://api.iconify.design/mdi:shield-key-outline.svg" alt="NextAuth" width="18" /> NextAuth | Authentication |
| <img src="https://api.iconify.design/mdi:message-processing-outline.svg" alt="Socket.io" width="18" /> Socket.io | Real-time updates |
| <img src="https://api.iconify.design/mdi:map-outline.svg" alt="Leaflet" width="18" /> Leaflet | Maps and location UI |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" alt="Node.js" width="18" /> Node.js | Runtime |
| <img src="https://api.iconify.design/mdi:credit-card-outline.svg" alt="Razorpay" width="18" /> Razorpay | Payments |
| <img src="https://api.iconify.design/mdi:cloud-upload-outline.svg" alt="Cloudinary" width="18" /> Cloudinary | Media storage |
| <img src="https://api.iconify.design/mdi:email-outline.svg" alt="Nodemailer" width="18" /> Nodemailer | Email delivery |
| <img src="https://api.iconify.design/mdi:robot-outline.svg" alt="Google Gemini" width="18" /> Google Gemini | AI suggestions |
| <img src="https://api.iconify.design/mdi:video-outline.svg" alt="ZegoCloud" width="18" /> ZegoCloud | Video KYC |
| <img src="https://api.iconify.design/mdi:chart-line.svg" alt="Recharts" width="18" /> Recharts | Charts and analytics |

## Getting Started

### Prerequisites

- Node.js 20 or later
- MongoDB database
- npm

### Install and Run

```bash
npm install
npm run dev
```

### Production Build

```bash
npm run build
npm start
```

## Environment Variables

The project expects a `.env.local` file with the main service credentials:

- `MONGODB_URL`
- `AUTH_SECRET`
- `AUTH_GOOGLE_ID`
- `AUTH_GOOGLE_SECRET`
- `NEXT_PUBLIC_SOCKET_SERVER_URL`
- `RAZORPAY_KEY_ID`
- `RAZORPAY_KEY_SECRET`
- `NEXT_PUBLIC_RAZORPAY_KEY_ID`
- `CLOUDINARY_CLOUD_NAME`
- `CLOUDINARY_API_KEY`
- `CLOUDINARY_API_SECRET`
- `NEXT_PUBLIC_GEOAPIFY_API_KEY`
- `NEXT_PUBLIC_ZEGO_APP_ID`
- `NEXT_PUBLIC_ZEGO_SERVER_SECRET`
- `GEMINI_API_URL`
- `EMAIL`
- `PASS`

## Project Notes

- The application uses role-based rendering on the home page.
- Real-time ride updates and chat depend on the Socket.io server configured in `NEXT_PUBLIC_SOCKET_SERVER_URL`.
- Nearby vehicle search relies on geospatial queries in MongoDB.
- The repository includes a separate Socket.io server in `socketServer/`.

## License

Private and proprietary.
