# AR-Interior-Design-App
It's a complete AR based app using for interior design.

Project Overview:
DesignAR is an AR-based Interior Design Mobile Application built with Next.js. It allows users to visualize furniture in their rooms using Augmented Reality, browse a furniture catalog, save designs, and manage their profile — all from a web-based platform.

App Features:
Splash Screen: Animated logo with loading indicator Auto-redirects to Landing or Dashboard based on login status.
Landing Page: Hero section with AR room visualization image Feature highlights (AR Visualization, Furniture Catalog, Room Design, Save & Share) Call-to-action buttons (Get Started / Sign In) App version badge in footer.
Signup Page: Full name, email, password fields Form validation Animated transitions
Login Page: Email and password authentication Local storage based auth Redirect to Dashboard on success.
Dashboard: Welcome greeting with user's first name Quick actions (Start AR Design, Browse Catalog, My Designs, Settings) Recent saved designs carousel Design tips section App version badge in header.
AR Camera View: Room selector — Living Room, Bedroom, Kitchen, Office Real room images as background Furniture placement — drag, rotate, scale items 3D View toggle for perspective Save design functionality Bottom navigation bar.
Furniture Catalog: categories: Living Room, Bedroom, Kitchen, Office, Decor 100+ furniture items with emojis and descriptions Search and filter functionality Category tabs with icons Add items to AR view directly.
Saved Designs: View all saved room designs Design cards with room type badge Item count per design Delete designs Load designs back into AR view 9.: Profile Page User avatar with initials Full name and email display Member since date Stats: Designs, Items Placed, Room Types Menu: Settings, My Designs, Browse Catalog, Contact Support Logout button App version badge.
Settings Page: Appearance: Light / Dark / System theme Notifications: Design Saved, New Features, Design Tips toggles Language: English, Spanish, French, German, Chinese, Japanese AR Settings: Show Grid, Snap to Grid, Measurement Units (cm/inches) Contact Support: Email, Phone, Website, Address (with copy buttons) 
Legal: Privacy Policy, Terms & Conditions links Learn: Design Tips link.
About: App Version (v2.0.0), App Name, Release Date, Platform.
Privacy Policy Page: Full privacy policy content Data collection, usage, and protection details
Terms & Conditions Page: Complete terms of service User responsibilities and app usage terms
Design Tips Page: Expandable tip cards Categories: Color Theory, Lighting, Furniture Layout, etc. Professional interior design advice
Dark Mode: Full dark mode support across all pages System preference detection Manual toggle available.

How to Run on VS Code (Windows) Prerequisites:
Node.js 18+ installed — Download from https://nodejs.org VS Code installed — Download from https://code.visualstudio.com Steps:
Extract ZIP Extract DesignAR-App.zip to any folder (e.g., Desktop)
Open in VS Code Open VS Code File → Open Folder → Select the extracted folder
Install Dependencies:
Open Terminal (Ctrl + ~) and run:
npm install 
Wait for installation to complete (1-2 minutes).
Run Development Server:
npm run dev
Open in Browser Go to: http://localhost:3000
Build for Production:
npm run build
Run Production Build: 
npm start

Key Technical Details:
State Management (Zustand):
app-store: Page navigation, current page tracking
auth-store:
User login/signup, session persistence (localStorage)
design-store: 
Saved designs, AR settings, current furniture items 
AR View Implementation: 
Room images serve as backgrounds ( tags for reliability) Furniture items rendered as overlay elements Drag: Uses useRef for performance (not useState) 
Rotate: 90-degree rotation on tap 
Scale: Pinch-to-zoom gesture support 
Room Switching: 4 rooms available 
Data Persistence: All data stored in localStorage User sessions persist across browser refreshes Saved designs include room type, furniture items, and positions 
PWA Support: Service Worker for offline caching Web App Manifest for home screen installation All icon sizes generated (72px to 512px)

Author

DesignAR Team: University Project — AR-Based Interior Design Mobile Application 
📄 License: This project is for educational purposes. All rights reserved
