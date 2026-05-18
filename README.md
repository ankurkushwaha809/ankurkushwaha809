<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Highlight Sections</title>
<style>
    /* Styling for the overall section */
    .modern-design-section {
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
        background-color: #f6f8fa; /* Main background color */
        padding: 40px;
        color: #24292e;
    }

    /* Styling for the main heading with emoji */
    .main-heading {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
        font-size: 28px;
        font-weight: bold;
        color: #24292e;
        margin-bottom: 30px;
        border-bottom: 2px solid #e1e4e8;
        padding-bottom: 10px;
    }

    /* Container for the cards to create a grid/flex layout */
    .cards-container {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        justify-content: center;
    }

    /* Styling for individual cards */
    .modern-card {
        background-color: #ffffff;
        border: 1px solid #e1e4e8;
        border-radius: 12px;
        padding: 24px;
        width: calc(50% - 20px); /* Two columns, minus gap */
        box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        transition: transform 0.2s ease, box-shadow 0.2s ease;
        display: flex;
        flex-direction: column;
    }

    /* Small hover effect for modern feel */
    .modern-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 15px rgba(0,0,0,0.1);
        border-color: #0366d6; /* GitHub blue on hover */
    }

    /* Header section inside the card (icon + title) */
    .card-header {
        display: flex;
        align-items: center;
        gap: 12px;
        margin-bottom: 16px;
    }

    /* Large size for emojis */
    .card-icon {
        font-size: 32px;
    }

    /* Individual card title styling */
    .card-title {
        font-size: 20px;
        font-weight: 600;
        margin: 0;
        color: #24292e;
    }

    /* Subtitle styling (job title, dates, client) */
    .card-subtitle {
        color: #586069;
        font-style: italic;
        font-size: 14px;
        margin-bottom: 20px;
        border-bottom: 1px solid #eaecef;
        padding-bottom: 10px;
    }

    /* Styling for main description text */
    .card-body {
        font-size: 15px;
        line-height: 1.6;
        color: #444d56;
        flex-grow: 1; /* Pushes content to the top */
    }

    /* List styling inside "Full Stack Projects" card */
    .project-list {
        margin: 0;
        padding-left: 20px;
        list-style-type: disc;
    }

    .project-list li {
        margin-bottom: 10px;
    }

    /* Make bullet point emojis slightly smaller than head emojis */
    .list-emoji {
        font-size: 1.1em;
        vertical-align: middle;
        margin-right: 5px;
    }

    /* Styling for emphasis within the text (client names) */
    .card-body em {
        color: #24292e;
        font-weight: 600;
        font-style: normal;
    }

</style>
</head>
<body>

<div class="modern-design-section">
    <h1 class="main-heading">
        <span class="card-icon">💼</span> Professional Experience & Featured Work Highlights
    </h1>

    <div class="cards-container">

        <div class="modern-card">
            <div class="card-header">
                <span class="card-icon">🏢</span>
                <h3 class="card-title">Digimees IT Solution</h3>
            </div>
            <div class="card-subtitle">Full Stack Developer | May 2024 - Present</div>
            <div class="card-body">
                <p>Architecting and deploying scalable MERN stack web and mobile applications. Managing secure authentication flows, 3rd-party payment integrations, and automated cloud deployments.</p>
            </div>
        </div>

        <div class="modern-card">
            <div class="card-header">
                <span class="card-icon">📚</span>
                <h3 class="card-title">Training Management System</h3>
            </div>
            <div class="card-subtitle">Client: <em>Lucent Biotech Limited</em></div>
            <div class="card-body">
                <p>Engineered a full-stack platform with JWT Role-Based Access Control. Designed modules for attendance tracking, course management, and scalable REST APIs.</p>
            </div>
        </div>

        <div class="modern-card">
            <div class="card-header">
                <span class="card-icon">🚀</span>
                <h3 class="card-title">Notable Projects</h3>
            </div>
            <div class="card-subtitle">Personal creations and contributions</div>
            <div class="card-body">
                <ul class="project-list">
                    <li>
                        <span class="list-emoji">🚗</span> <strong>Car Parking System:</strong> Real-time slot availability, admin management, and booking APIs.
                    </li>
                    <li>
                        <span class="list-emoji">🍽️</span> <strong>Restaurant Booking:</strong> Online table management and user reservation portal with robust UI.
                    </li>
                </ul>
            </div>
        </div>

    </div>
</div>

</body>
</html>
