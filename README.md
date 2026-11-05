# APSRTC-Smart-Yatra-Assistant
An accessibility-first multimodal transit platform designed to enhance the daily commuting experience across AP. It bridges the gap between traditional bus scheduling, real-time GPS tracking, passenger emergency safety, multimodal alternative mobility, and proactive with complete hands-free voice assistance for visually impaired .
🚀 All Features Offered (Short Bulletin Points)
1. 🎨 Visual Identity & Inclusive Design
Authentic APSRTC Branding: Professional UI styled in official APSRTC Emerald Green (#006837) and RTC Telugu Gold (#FDB813).
Prominent Native Language Selector: Top-level switcher supporting 6 languages with native typography:
🇬🇧 English, 🇮🇳 తెలుగు, 🇮🇳 हिंदी, 🇮🇳 தமிழ், 🇮🇳 ಕನ್ನಡ, 🇮🇳 മലയാളം.
High-Contrast Dark Mode: One-click high-contrast mode with bold borders and optimized readability for low-vision passengers.
Dynamic 3-Tier Font Resizing: Quick cycling (A-, A, A+) across all screen interfaces.
2. 🗺️ Live GPS Bus Radar & Transit Dataset
Simulated Real-Time Moving Fleet: 6+ active buses moving across AP highways with dynamic GPS interpolation.
Live Vehicle Telemetry: Real-time speedometer (km/h), heading compass, seat occupancy gauge (%), and next stop ETA.
24+ Comprehensive AP Bus Stations: Major transit hubs (Vijayawada PNBS, Visakhapatnam DBS, Tirupati Central, Guntur NTR, Kurnool, etc.) with platform numbers (e.g. PNBS 78 platforms) and amenities.
Nearest Stop Locator: Geolocation-based distance calculation with walking duration estimates.
One-Click Regional City Hub Jumps: Direct map centering for Vijayawada, Vizag, Guntur, Tirupati, Rajahmundry, and Kurnool.
3. 🛡️ Emergency Safety Dead-Man Switch
Automated Trip Arming: Commuter inputs emergency contact (name & phone number) and expected arrival time.
Arrival Check-In Verification: When ETA is reached, the system issues an arrival confirmation prompt: "Have you safely arrived at your destination?"
Dead-Man Escalation: If unconfirmed within the grace period (1-hour standard or 10-second rapid demo test), system automatically activates emergency protocol.
Rich SOS Dispatch: Packages live GPS coordinates, Google Maps pin link, bus service number, and trip itinerary.
One-Click Instant WhatsApp SOS & Direct SMS: Direct pre-filled communication links to emergency contacts and local helplines.
4. 🤖 AI Commuter Assistant & Multi-Modal Recovery
Hybrid AI Architecture: Google Gemini integration paired with offline fallback logic for 100% service uptime.
Missed Bus Recovery Protocol:
Automatically assesses travel urgency and calculates remaining highway distance.
Recommends fastest alternative mobility: Rapido bike taxi (fare ₹160–₹240, 40–50 mins), Ola/Uber cabs, auto rickshaws, and connecting train schedules.
Pre-fills next bus options with filtered departure times.
Proactive Budget Planning Interview:
Agent proactively interviews the commuter regarding weekly commute frequency and budget limits.
Automatically advises on concessions: Student passes, Senior Citizen 25% discount, Divyangjan free transit, and Navasaka passes.
Contextual Reminders & Expense Tracker: Schedules departure/boarding alerts and logs transit expenditures.
5. 🎙️ Full Voice Assistance for Visually Impaired Commuters
Hands-Free Web Speech Engine: Integrated speech recognition and natural text-to-speech synthesis.
Audio Screen Narration: "Read screen" command provides audio summaries of any open page, route option, or alert.
Voice Navigation Commands: Commuters can speak their way through the whole app:
"Go to Planner", "Open Map", "Ask Assistant", "Emergency Alert", "Switch to Telugu/Hindi", "Stop".
6. 🏛️ Official Grievance Redressal & Helpline Dispatch
Direct Helplines Directory:
24/7 APSRTC Customer Care: 1800-200-2000
Official Grievance Email: customercare@apsrtc.gov.in
Women Safety Helplines: 1091 / 112
Regional Depot Managers (Vijayawada, Vizag, Tirupati, Guntur, Kurnool).
Automated Formal Letter Generator: Formats official complaint letters with incident timestamps and unique reference IDs.
One-Click Dispatch: Direct mailto: integration to APSRTC care email and WhatsApp grievance desk.
7. 🕹️ APSRTC Operations, Telemetry & Simulation Hub (/demo)
System Health Monitor: Live telemetry for Backend API, GPS Fleet Radar, Safety Dead-Man Switch, and Web Speech Engine.
Interactive Fleet Telemetry Controller: Adjust live vehicle cruising speed, inject highway congestion (+15m), or trigger mechanical breakdown protocols.
5-Second Rapid Safety Test: Live visual simulation of the dead-man switch workflow with countdown bar and SOS preview.
Regional Depot Command Board: Real-time platform occupancy, on-time departure rates (e.g. PNBS 96.2%), and highway weather advisories.
🏗️ Technical Architecture
Frontend: React 18, TypeScript, Tailwind CSS, Leaflet & React-Leaflet, Zustand (with LocalStorage state persistence), Lucide Icons, Vite.
Backend: Python 3.12, FastAPI, Pydantic v2, SlowAPI rate limiting, Structlog, Pytest (13/13 passing tests).
Speech Engine: Web Speech API (SpeechRecognition & SpeechSynthesisUtterance).
Telemetry Engine: Real-time GPS path interpolation over Andhra Pradesh highway vectors.
🔮 Future Scope & Project Roadmap
Phase	Milestone	Description
Phase 1	Direct APSRTC VTS / OBD-II API Sync	Integrate directly with APSRTC's live Vehicle Tracking System (VTS) and depot IoT GPS transponders.
Phase 2	Automated Server-Side SMS Gateway	Integrate Twilio or Government SMS Gateway (CDAC) for automatic zero-click SMS dispatch if phone is offline or battery dies.
Phase 3	Offline Progressive Web App (PWA)	Offline caching with Service Workers for seamless usage along low-signal rural Andhra Pradesh ghat roads and villages.
Phase 4	UPI-Integrated Digital Ticketing	In-app UPI QR code booking (PhonePe, Google Pay, Paytm) and instant digital bus pass renewals inside the AI chat.
Phase 5	Crowdsourced Occupancy & Seat Availability	Real-time passenger reports on bus crowdedness, AC temperature, and seat availability at upcoming stops.
Phase 6	Dialect-Specific Telugu Speech Recognition	Custom acoustic models fine-tuned for regional Telugu dialects (Godavari, Rayalaseema, Uttarandhra, Krishna).
Phase 7	Depot Computer Vision & Beacon Wayfinding	BLE Beacons & smartphone camera assistance to guide visually impaired passengers directly from the bus station gate to their designated platform.
