<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Securewell LLC - Life Insurance Made Easy</title>
    <!-- Tailwind CSS CDN for styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts for Inter (still included for general page style if needed, though most text is now image) -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8; /* Light background for the page */
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
            box-sizing: border-box;
        }
        .ad-container {
            position: relative; /* Essential for positioning the overlay link */
            max-width: 480px; /* Constrain width for a flyer-like appearance */
            width: 100%; /* Make it responsive */
            border: 2px solid #228B22; /* Green border matching the original flyer */
            border-radius: 12px;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1); /* Softer, larger shadow */
            overflow: hidden; /* Ensures border-radius applies to image edges */
        }
        .full-flyer-image {
            width: 100%;
            height: auto; /* Maintain aspect ratio */
            display: block; /* Remove extra space below image */
            border-radius: 10px; /* Match container border-radius slightly */
        }

        .clickable-overlay {
            position: absolute;
            /* These values are estimates based on the image proportions.
               You might need to fine-tune them after previewing. */
            bottom: 3.5%; /* Adjust this to move the link up/down */
            left: 10%; /* Adjust this to move the link left/right */
            width: 80%; /* Adjust this to make the clickable area wider/narrower */
            height: 5%; /* Adjust this to make the clickable area taller/shorter */
            background-color: rgba(0, 255, 0, 0); /* Invisible background */
            cursor: pointer;
            z-index: 10; /* Ensure it's above the image */
            display: block; /* Make the entire area clickable */
        }

        /* Optional: Add a visual cue on hover for the clickable area */
        .clickable-overlay:hover {
             outline: 2px solid rgba(255, 255, 255, 0.5); /* Subtle white border on hover */
             box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
        }

        /* Responsive adjustments for the overlay if needed, although percentages usually handle this */
        @media (max-width: 600px) {
            .ad-container {
                border-radius: 8px; /* Slightly less rounded corners for smaller screens */
            }
            /* You might need to adjust overlay percentages slightly for different screen sizes if the image scales disproportionately */
        }
    </style>
</head>
<body>

    <div class="ad-container">
        <!-- The entire flyer as a single image -->
        <img src="uploaded:image_bb8681.png-b3f054bf-0b0c-428c-8de2-25d981573407" 
             onerror="this.onerror=null;this.src='https://placehold.co/480x720/E0F2F7/333333?text=Flyer+Image+Not+Found';" 
             alt="Securewell LLC Life Insurance Flyer" 
             class="full-flyer-image">

        <!-- Invisible clickable overlay for the URL -->
        <a href="https://agents.ethoslife.com/invite/b4a05" 
           target="_blank" 
           rel="noopener noreferrer" 
           class="clickable-overlay" 
           aria-label="Visit Ethos Life Website">
        </a>
    </div>

</body>
</html>
