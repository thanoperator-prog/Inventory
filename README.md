Inventory & Equipment Monitor App

Isang modern at single-file web application para sa pamamahala ng imbentaryo, pagsubaybay sa lokasyon ng kagamitan, at pag-monitor ng status. Ito ay gumagamit ng Firebase Firestore para sa real-time na database.

🚀 Features

Dashboard: Real-time statistics ng total items, assigned assets, at room occupancy.

Inventory Management: Pag-add, edit, at pag-delete ng items. May "undo" functionality para sa accidental deletions.

Location Management: Pamamahala ng Floors, Rooms, at Boxes.

Activity Logs: Detalyadong history ng bawat galaw sa system.

Data Import/Export: Kakayahang mag-export at mag-import ng data gamit ang CSV.

PDF Reports: Pag-generate ng professional PDF reports para sa inventory at status.

Mobile Responsive: Gumagana sa desktop, tablet, at mobile devices.

🛠️ Setup & Configuration

Ang app na ito ay dinisenyo upang tumakbo bilang isang standalone na index.html file.

1. Firebase Setup

Para gumana ang database, kailangan mong ikonekta ito sa iyong sariling Firebase project:

Pumunta sa Firebase Console.

Gumawa ng bagong project.

I-enable ang Firestore Database (Start in Test Mode para sa mabilisang setup).

I-enable ang Authentication at piliin ang Anonymous sign-in provider.

Pumunta sa Project Settings at kopyahin ang firebaseConfig.

2. Update Code

Buksan ang index.html at hanapin ang customConfig variable. I-paste ang iyong API keys doon:

const customConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT.firebaseapp.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT.appspot.com",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID"
};


🌐 Deployment

Maaari mong i-host ang app na ito kahit saan na sumusuporta sa static websites:

GitHub Pages: I-upload ang index.html at i-enable ang Pages sa Settings.

Firebase Hosting: Gamitin ang firebase deploy.

Local: Buksan lang ang index.html sa iyong browser.

📄 Libraries Used

Tailwind CSS - Styling

Lucide Icons - Icons

Firebase SDK - Backend/Database

Chart.js - Dashboard Charts

jsPDF & AutoTable - PDF Generation

PapaParse - CSV Processing

Created with Gemini Canvas
