# home-buyer-carousel
A home buyer guide carousel for my real estate landing page.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Buyer Guide Carousel</title>
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css" />
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: #f5f5f5;
        }
        .swiper-container {
            width: 90%;
            max-width: 600px;
            height: 400px;
        }
        .swiper-slide {
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: #fff;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body>
    <div class="swiper-container">
        <div class="swiper-wrapper">
            <div class="swiper-slide">Step 1: Get Pre-Approved for a Mortgage</div>
            <div class="swiper-slide">Step 2: Find the Right Home</div>
            <div class="swiper-slide">Step 3: Make an Offer</div>
            <div class="swiper-slide">Step 4: Home Inspection & Appraisal</div>
            <div class="swiper-slide">Step 5: Closing & Move-In</div>
        </div>
        <div class="swiper-pagination"></div>
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>
    </div>
    <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>
    <script>
        var swiper = new Swiper('.swiper-container', {
            loop: true,
            pagination: { el: '.swiper-pagination', clickable: true },
            navigation: { nextEl: '.swiper-button-next', prevEl: '.swiper-button-prev' }
        });
    </script>
</body>
</html>
