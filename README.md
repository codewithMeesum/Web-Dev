# Web-Dev
For u ! 


index.htm : 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Hover Card</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <!-- Card 1 -->
        <div class="card">
            <div class="card-overlay">
                <h2 class="card-title">Deep Thoughts</h2>
                <p class="card-description">
                    When you're trying to understand your assignment but the instructions are more confusing than the task itself. Sometimes we all need a moment to think!
                </p>
                <a href="#" class="card-button">Learn More</a>
            </div>
        </div>

        <!-- Card 2 -->
        <div class="card card-2">
            <div class="card-overlay">
                <h2 class="card-title">Beach Paradise</h2>
                <p class="card-description">
                    Relax on pristine beaches with crystal clear waters. The perfect getaway for those seeking peace and tranquility by the ocean.
                </p>
                <a href="#" class="card-button">Discover Now</a>
            </div>
        </div>

        <!-- Card 3 -->
        <div class="card card-3">
            <div class="card-overlay">
                <h2 class="card-title">Night Sky</h2>
                <p class="card-description">
                    Witness the magic of starlit nights and celestial wonders. An unforgettable experience for astronomy enthusiasts and dreamers.
                </p>
                <a href="#" class="card-button">Learn More</a>
            </div>
        </div>
    </div>
</body>
</html>


style.css : 
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background: linear-gradient(to bottom, #2c3e50, #3498db);
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
}

.container {
    max-width: 1200px;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 30px;
}

.card {
    width: 350px;
    height: 450px;
    background-image: url('https://gptimage.ai/wp-content/uploads/gptimage/2025/08/A-monkey-standing-in-front-of-a-harbor-looking-up-thoughtfully-with-one-finger-in-its-mouth-as-if-deep-in-thought-768x768.png');
    background-size: cover;
    background-position: center;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    transition: transform 0.4s ease, box-shadow 0.4s ease;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
}

.card:hover {
    transform: scale(1.05);
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5);
}

.card-overlay {
    background: linear-gradient(to top, rgba(0, 0, 0, 0.8), transparent);
    padding: 30px;
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.card-title {
    color: white;
    font-size: 2rem;
    font-weight: bold;
    margin-bottom: 10px;
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 0.5s ease, transform 0.5s ease;
}

.card:hover .card-title {
    opacity: 1;
    transform: translateY(0);
}

.card-description {
    color: white;
    font-size: 1rem;
    line-height: 1.6;
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 0.5s ease, transform 0.5s ease;
}

.card:hover .card-description {
    opacity: 1;
    transform: translateY(0);
}

.card-button {
    display: inline-block;
    background-color: #3498db;
    color: white;
    padding: 12px 25px;
    border-radius: 25px;
    text-decoration: none;
    text-align: center;
    font-weight: bold;
    opacity: 0;
    transform: translateY(20px) scale(0.8);
    transition: opacity 0.6s ease, transform 0.6s ease, background-color 0.3s ease;
    align-self: flex-start;
}

.card:hover .card-button {
    opacity: 1;
    transform: translateY(0) scale(1);
}

.card-button:hover {
    background-color: #2980b9;
}

/* Second Card with Different Image */
.card-2 {
    background-image: url('https://tse4.mm.bing.net/th/id/OIP.YLKVMIdd_jplbcizqr4h8gHaHa?pid=Api&P=0&h=220');
}

/* Third Card with Different Image */
.card-3 {
    background-image: url('https://images.unsplash.com/photo-1519681393784-d120267933ba?w=800&h=1000&fit=crop');
}

/* Tablet View (768px and below) */
@media screen and (max-width: 768px) {
    .container {
        gap: 20px;
    }

    .card {
        width: 100%;
        max-width: 400px;
        height: 400px;
    }

    .card-title {
        font-size: 1.8rem;
    }

    .card-description {
        font-size: 0.95rem;
    }

    .card-overlay {
        padding: 25px;
    }

    .card-button {
        padding: 10px 20px;
        font-size: 0.9rem;
    }
}

/* Mobile View (480px and below) */
@media screen and (max-width: 480px) {
    body {
        padding: 15px;
    }

    .card {
        height: 350px;
    }

    .card-title {
        font-size: 1.5rem;
        margin-bottom: 8px;
    }

    .card-description {
        font-size: 0.85rem;
        line-height: 1.5;
    }

    .card-overlay {
        padding: 20px;
        gap: 10px;
    }

    .card-button {
        padding: 8px 18px;
        font-size: 0.85rem;
    }

    .card:hover {
        transform: scale(1.02);
    }
}

/* Large Desktop View (1200px and above) */
@media screen and (min-width: 1200px) {
    .card {
        width: 380px;
        height: 500px;
    }

    .card-title {
        font-size: 2.2rem;
    }

    .card-description {
        font-size: 1.05rem;
    }

    .card-overlay {
        padding: 35px;
    }
}

-------------------------------------------------------------------------------
## 📂 Folder Structure:
```
project-folder/
│
├── index.html
└── style.css
