# lumina-care-app-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lumicare | AI-Powered Premium Skincare</title>
    <!-- Fonts & Firebase SDKs included -->
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Auth & Navigation -->
    <header>...</header>

    <main>
        <!-- Hero Section -->
        <section id="home">...</section>

        <!-- AI Analysis Section -->
        <section id="analysis">
            <div id="scanner-container">
                <video id="video" style="display: none;"></video>
                <div id="scan-overlay"></div>
            </div>
        </section>

        <!-- Dynamic Shop & Consult Sections -->
        <section id="shop">...</section>
    </main>

    <script src="script.js"></script>
</body>
</html>

:root {
    --color-primary: #8DAA91;      /* Sage Green */
    --color-background: #FBFAF8;   /* Pearl White */
    --color-text: #2D3436;         /* Deep Charcoal */
    --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.glass-card {
    background: rgba(255, 255, 255, 0.7);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255, 255, 255, 0.3);
    box-shadow: var(--shadow-md);
}

/* Scanning Animation */
@keyframes scan {
    0% { top: 0; }
    50% { top: 100%; }
    100% { top: 0; }
}

// Example: Analysis Logic
const generateDetailedAnalysis = () => {
    const types = [
        {
            type: "Dry / Dehydrated",
            summary: "Your skin shows significant dehydration...",
            scores: { hydration: 34, texture: 72, clarity: 88 }
        },
        // ... more skin profiles
    ];
    return types[Math.floor(Math.random() * types.length)];
};


it is app which scan the face , tries to know problems , deliver proper solution , suggest consultation 
