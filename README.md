🏟️ VenueSpot
VenueSpot is a modern, AI-powered real-time event management platform designed to connect event organizers with the perfect venues. Built with a focus on speed, real-time interactivity, and high-level security.
🚀 The Modern Tech Stack
Moving beyond the traditional MERN stack, VenueSpot utilizes a high-performance "Modern Trio" for better developer experience and user performance:
 * Frontend: React.js & Tailwind CSS
 * Backend & Database: Convex (Reactive, Real-time Backend-as-a-Service)
 * Authentication: Clerk (Identity & User Management)
 * UI Components: shadcn/ui (Radix UI + Tailwind)
 * Type Safety: TypeScript
✨ Key Features
1. Real-time Venue Syncing (Powered by Convex)
Unlike standard REST APIs, VenueSpot uses Convex’s reactive queries. This means any update to a venue's availability or pricing is pushed instantly to all users without a page refresh or manual polling.
2. Secure, Multi-tenant Auth (Powered by Clerk)
We use Clerk to handle complex authentication flows, including:
 * Social Logins (Google, GitHub, etc.).
 * Role-Based Access Control (Organizers vs. Venue Owners).
 * Seamless JWT-based synchronization with the Convex backend.
3. Accessible & Premium UI (Powered by shadcn/ui)
The interface is built using shadcn/ui, ensuring that every component is:
 * Fully accessible (WAI-ARIA compliant).
 * Highly performant.
 * Custom-tailored to VenueSpot’s branding.
4. AI-Driven Discovery (In-Progress)
Integrating AI to analyze user preferences and logistics to recommend the most suitable venues automatically.
🏗️ Architecture Overview
graph TD
    A[User/Browser] -->|Auth| B(Clerk)
    A -->|Reactive UI| C(React + shadcn/ui)
    C -->|Real-time Subscriptions| D(Convex Backend)
    B -->|JWT Verification| D
    D -->|Persistent Data| E[(Convex Database)]

🛠️ Getting Started
Prerequisites
 * Node.js (v18+)
 * A Convex account
 * A Clerk account
Installation
 * Clone the repository:
   git clone
cd venuespot

 * Install dependencies:
   npm install

 * Set up Environment Variables:
   Create a .env.local file and add your Clerk and Convex keys:
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_key
CLERK_SECRET_KEY=your_key
CONVEX_DEPLOYMENT_URL=your_url
NEXT_PUBLIC_CONVEX_URL=your_url

 * Run the development server:
   npm run dev

📈 Roadmap
 * [x] Initial Project Setup (React + TypeScript)
 * [x] Clerk Auth Integration
 * [x] Convex Real-time Schema Design
 * [ ] AI-Powered Recommendation Engine
 * [ ] Booking & Payment Gateway Integration
 * [ ] Mobile App (React Native + Expo)
🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
📄 License
Distributed under the MIT License. See LICENSE for more information.
Developed with ❤️ by Teja Yeshamoni

