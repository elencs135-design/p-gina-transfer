<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Credit Card Debt Sucks - Transfer Your Balance & Regain Your Freedom</title>
    <style>
        /* Basic Reset & Global Styles */
        * { box-sizing: border-box; margin: 0; padding: 0; }
        html { scroll-behavior: smooth; }
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
            line-height: 1.6;
            color: #333;
            background-color: #f8f8f8;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
        .container { max-width: 1200px; margin: 0 auto; padding: 20px; }
        h1, h2, h3 { color: #0066CC; margin-bottom: 20px; line-height: 1.2; }
        h1 { font-size: 2.5em; text-align: center; }
        h2 { font-size: 2em; text-align: center; }
        p { margin-bottom: 15px; }
        .btn {
            display: inline-block;
            background-color: #0066CC;
            color: #fff;
            padding: 12px 25px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s ease, transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            border: none;
            cursor: pointer;
            font-size: 1em;
        }
        .btn:hover { background-color: #0056b3; transform: translateY(-2px); box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3); }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #0066CC 0%, #0056b3 100%);
            color: #fff;
            padding: 80px 20px;
            text-align: center;
            position: relative;
            overflow: hidden;
            border-bottom-left-radius: 20px;
            border-bottom-right-radius: 20px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }
        .hero h1 { font-size: 3em; margin-bottom: 15px; color: #fff; }
        .hero h2 { font-size: 1.5em; margin-bottom: 30px; color: #eee; font-weight: normal; }

        /* Section styles */
        section { padding: 60px 20px; text-align: center; }
        section:nth-of-type(even) { background-color: #f0f0f0; }

        /* Cards Section */
        .cards-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            margin-top: 40px;
        }
        .card {
            background-color: #fff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
            text-align: left;
            max-width: 300px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid #eee;
        }
        .card:hover { transform: translateY(-10px); box-shadow: 0 12px 24px rgba(0, 0, 0, 0.2); }
        .card h3 { color: #0066CC; margin-bottom: 15px; font-size: 1.5em; }
        .card p { color: #555; font-size: 1em; }

        /* Table Section */
        .table-container { overflow-x: auto; margin-top: 40px; }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 0 auto;
            max-width: 800px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            overflow: hidden; /* Ensures rounded corners apply to children */
        }
        th, td { padding: 15px; border: 1px solid #ddd; text-align: left; }
        th { background-color: #0066CC; color: #fff; font-weight: bold; }
        tr:nth-child(even) { background-color: #f9f9f9; }
        tr:hover { background-color: #f1f1f1; }
        .highlight-success { color: #28a745; font-weight: bold; }
        .highlight-danger { color: #dc3545; font-weight: bold; }

        /* Video Section */
        .video-section { background-color: #f8f8f8; padding: 60px 20px; }
        .video-wrapper {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            height: 0;
            overflow: hidden;
            max-width: 800px;
            margin: 40px auto;
            background-color: #000;
            border-radius: 10px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }
        .video-wrapper video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }
        .video-controls {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            background: linear-gradient(to top, rgba(0,0,0,0.8) 0%, rgba(0,0,0,0) 100%);
            color: #fff;
            padding: 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            font-size: 0.9em;
            transition: opacity 0.3s ease;
            opacity: 0;
            pointer-events: none; /* Allow clicks to pass through when hidden */
        }
        .video-wrapper:hover .video-controls, .video-controls.active { opacity: 1; pointer-events: all; }
        .video-controls button {
            background: none;
            border: none;
            color: #fff;
            font-size: 1.2em;
            cursor: pointer;
            padding: 5px 10px;
            transition: color 0.2s ease;
        }
        .video-controls button:hover { color: #0066CC; }
        .video-controls input[type="range"] {
            flex-grow: 1;
            margin: 0 10px;
            -webkit-appearance: none;
            appearance: none;
            height: 5px;
            background: #555;
            border-radius: 5px;
            outline: none;
            cursor: pointer;
        }
        .video-controls input[type="range"]::-webkit-slider-thumb {
            -webkit-appearance: none;
            appearance: none;
            width: 15px;
            height: 15px;
            background: #0066CC;
            border-radius: 50%;
            cursor: pointer;
            box-shadow: 0 0 2px rgba(0,0,0,0.5);
        }
        .video-controls input[type="range"]::-moz-range-thumb {
            width: 15px;
            height: 15px;
            background: #0066CC;
            border-radius: 50%;
            cursor: pointer;
            box-shadow: 0 0 2px rgba(0,0,0,0.5);
        }
        .video-progress-bar { height: 5px; background: #0066CC; width: 0%; border-radius: 5px; position: absolute; top: 0; left: 0; }
        .video-time { margin: 0 10px; color: #ccc; }
        .speed-selector {
            background-color: rgba(0, 0, 0, 0.5);
            color: #fff;
            border: none;
            padding: 5px;
            border-radius: 3px;
            cursor: pointer;
            margin-left: 10px;
        }
        .video-overlay-cta {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            color: #fff;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.3s ease, visibility 0.3s ease;
            border-radius: 10px;
            padding: 20px;
        }
        .video-overlay-cta.active { opacity: 1; visibility: visible; }
        .video-overlay-cta h3 { color: #fff; margin-bottom: 20px; font-size: 1.8em; }

        /* Gallery Section */
        .gallery-section { padding: 60px 20px; }
        .image-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }
        .image-gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
            background-color: #e0e0e0; /* Placeholder background */
        }
        .image-gallery img:hover { transform: scale(1.05); }

        /* Final CTA Section */
        .final-cta-section {
            background: linear-gradient(135deg, #0066CC 0%, #28a745 100%);
            color: #fff;
            padding: 60px 20px;
            border-top-left-radius: 20px;
            border-top-right-radius: 20px;
            box-shadow: 0 -8px 16px rgba(0, 0, 0, 0.2);
        }
        .final-cta-section h2 { color: #fff; margin-bottom: 30px; }
        .final-cta-section .btn { background-color: #fff; color: #0066CC; }
        .final-cta-section .btn:hover { background-color: #eee; transform: translateY(-2px); box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3); }

        /* Footer */
        footer { background-color: #333; color: #fff; text-align: center; padding: 20px; font-size: 0.9em; }

        /* Animations */
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        @keyframes slideUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
        .animate-on-scroll { opacity: 0; transform: translateY(20px); transition: opacity 0.6s ease-out, transform 0.6s ease-out; }
        .animate-on-scroll.is-visible { opacity: 1; transform: translateY(0); }

        /* Responsive adjustments */
        @media (min-width: 768px) {
            h1 { font-size: 3.5em; }
            h2 { font-size: 2.5em; }
            .hero { padding: 100px 20px; }
            .cards-container { grid-template-columns: repeat(2, 1fr); }
            .card { max-width: none; }
            .image-gallery { grid-template-columns: repeat(4, 1fr); }
        }
        @media (min-width: 1024px) {
            h1 { font-size: 4em; }
            h2 { font-size: 3em; }
            .cards-container { grid-template-columns: repeat(3, 1fr); }
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <header class="hero">
        <div class="container animate-on-scroll">
            <h1>Credit Card Debt Sucks</h1>
            <h2>Transfer Your Balance & Regain Your Freedom</h2>
            <a href="https://pay.hotmart.com/V102947506D" class="btn">Get Started Now</a>
        </div>
    </header>

    <!-- Why Transfer Your Balance? Section -->
    <section class="animate-on-scroll">
        <div class="container">
            <h2>Why Transfer Your Balance?</h2>
            <div class="cards-container">
                <div class="card animate-on-scroll">
                    <h3>Save Money</h3>
                    <p>Lower interest rates mean less money wasted on interest payments, allowing you to pay down your principal faster.</p>
                </div>
                <div class="card animate-on-scroll">
                    <h3>Simplify Payments</h3>
                    <p>Consolidate multiple high-interest credit card debts into one manageable payment, making budgeting easier.</p>
                </div>
                <div class="card animate-on-scroll">
                    <h3>Improve Credit Score</h3>
                    <p>By paying down your debt more efficiently, you can positively impact your credit utilization and overall credit score.</p>
                </div>
                <div class="card animate-on-scroll">
                    <h3>Reduce Stress</h3>
                    <p>Take control of your finances, eliminate the burden of high interest, and gain invaluable peace of mind.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Comparative Table Section -->
    <section class="animate-on-scroll">
        <div class="container">
            <h2>Compare Your Options</h2>
            <div class="table-container">
                <table>
                    <thead>
                        <tr>
                            <th>Feature</th>
                            <th>Current Credit Card Debt</th>
                            <th>Balance Transfer Offer</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td><strong>Interest Rate</strong></td>
                            <td class="highlight-danger">18% - 25% APR</td>
                            <td class="highlight-success">0% - 5% APR (Intro)</td>
                        </tr>
                        <tr>
                            <td><strong>Monthly Payment</strong></td>
                            <td>High, interest-heavy</td>
                            <td>Lower, principal-focused</td>
                        </tr>
                        <tr>
                            <td><strong>Debt Payoff</strong></td>
                            <td>Slow, difficult</td>
                            <td>Faster, achievable</td>
                        </tr>
                        <tr>
                            <td><strong>Stress Level</strong></td>
                            <td class="highlight-danger">High</td>
                            <td class="highlight-success">Low</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </section>

    <!-- Video Section -->
    <section class="video-section animate-on-scroll">
        <div class="container">
            <h2>Tired of Being a Slave to Your Credit Card?</h2>
            <div class="video-wrapper" id="customVideoPlayer">
                <!--
                    INSTRUCTIONS: Replace "seu-video.mp4" with the actual path to your video file.
                    Ensure the video file is hosted and accessible.
                    Example: <source src="https://yourdomain.com/videos/my-debt-solution.mp4" type="video/mp4">
                -->
                <video preload="metadata" playsinline>
                 <source src="https://seu-dominio.com/seu-video.mp4" type="video/mp4">
                 Your browser does not support the video tag.
                </video>
                <div class="video-controls">
                    <button class="play-pause-btn">&#9658;</button> <!-- Play icon -->
                    <div style="position:relative; flex-grow:1; height:5px;">
                        <input type="range" class="progress-range" min="0" max="100" value="0" step="0.1">
                        <div class="video-progress-bar"></div>
                    </div>
                    <span class="video-time current-time">00:00</span> / <span class="video-time duration">00:00</span>
                    <button class="volume-btn">&#128266;</button> <!-- Volume icon -->
                    <input type="range" class="volume-range" min="0" max="1" value="1" step="0.01" style="width: 60px;">
                    <select class="speed-selector">
                        <option value="0.5">0.5x</option>
                        <option value="1" selected>1x</option>
                        <option value="1.5">1.5x</option>
                        <option value="2">2x</option>
                    </select>
                    <button class="fullscreen-btn">&#x26F6;</button> <!-- Fullscreen icon -->
                </div>
                <div class="video-overlay-cta">
                    <h3>Ready to Break Free from Debt?</h3>
                    <a href="https://pay.hotmart.com/V102947506D" class="btn">Get Started Now</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Image Gallery Section -->
    <section class="gallery-section animate-on-scroll">
        <div class="container">
            <h2>Your Path to Financial Freedom</h2>
            <div class="image-gallery">
                <img class="lazy" data-src="https://via.placeholder.com/400x200?text=Freedom+1" alt="Financial Freedom Image 1">
                <img class="lazy" data-src="https://via.placeholder.com/400x200?text=Freedom+2" alt="Financial Freedom Image 2">
                <img class="lazy" data-src="https://via.placeholder.com/400x200?text=Freedom+3" alt="Financial Freedom Image 3">
                <img class="lazy" data-src="https://via.placeholder.com/400x200?text=Freedom+4" alt="Financial Freedom Image 4">
            </div>
        </div>
    </section>

    <!-- Final Call to Action Section -->
    <section class="final-cta-section animate-on-scroll">
        <div class="container">
            <h2>Don't Let Debt Control Your Life Any Longer.</h2>
            <a href="https://pay.hotmart.com/V102947506D" class="btn">Get Started Today</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2023 Your Company Name. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // INSTRUCTIONS:
        // To deploy this page:
        // 1. Save this entire code as an HTML file (e.g., index.html).
        // 2. Replace "seu-video.mp4" in the <video> tag with the actual URL or path to your video file.
        //    Make sure your video file is hosted and accessible.
        // 3. Upload the index.html file (and your video file) to your web server or hosting service (e.g., Vercel, Netlify, cPanel).

        // Lazy loading for images
        document.addEventListener("DOMContentLoaded", function() {
            var lazyImages = [].slice.call(document.querySelectorAll("img.lazy"));
            if ("IntersectionObserver" in window) {
                let lazyImageObserver = new IntersectionObserver(function(entries, observer) {
                    entries.forEach(function(entry) {
                        if (entry.isIntersecting) {
                            let lazyImage = entry.target;
                            lazyImage.src = lazyImage.dataset.src;
                            lazyImage.classList.remove("lazy");
                            lazyImageObserver.unobserve(lazyImage);
                        }
                    });
                }, { rootMargin: "0px 0px -50px 0px" }); // Load 50px before entering viewport
                lazyImages.forEach(function(lazyImage) {
                    lazyImageObserver.observe(lazyImage);
                });
            } else {
                // Fallback for browsers without Intersection Observer
                lazyImages.forEach(function(lazyImage) {
                    lazyImage.src = lazyImage.dataset.src;
                    lazyImage.classList.remove("lazy");
                });
            }
        });

        // Scroll animations
        document.addEventListener("DOMContentLoaded", function() {
            const animateElements = document.querySelectorAll(".animate-on-scroll");
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add("is-visible");
                    }
                });
            }, { threshold: 0.1 }); // Trigger when 10% of the element is visible

            animateElements.forEach(element => {
                observer.observe(element);
            });
        });

        // Video Player Logic
        document.addEventListener("DOMContentLoaded", function() {
            const videoPlayer = document.getElementById('customVideoPlayer');
            const video = videoPlayer.querySelector('video');
            const playPauseBtn = videoPlayer.querySelector('.play-pause-btn');
            const progressBar = videoPlayer.querySelector('.progress-bar');
            const progressRange = videoPlayer.querySelector('.progress-range');
            const currentTimeElem = videoPlayer.querySelector('.current-time');
            const durationElem = videoPlayer.querySelector('.duration');
            const volumeRange = videoPlayer.querySelector('.volume-range');
            const volumeBtn = videoPlayer.querySelector('.volume-btn');
            const speedSelector = videoPlayer.querySelector('.speed-selector');
            const fullscreenBtn = videoPlayer.querySelector('.fullscreen-btn');
            const controls = videoPlayer.querySelector('.video-controls');
            const videoOverlayCta = videoPlayer.querySelector('.video-overlay-cta');

            let isPlaying = false;
            let volumeBeforeMute = video.volume; // Store initial volume

            // Play/Pause
            function togglePlayPause() {
                if (video.paused || video.ended) {
                    video.play();
                    playPauseBtn.innerHTML = '&#10074;&#10074;'; // Pause icon
                    isPlaying = true;
                } else {
                    video.pause();
                    playPauseBtn.innerHTML = '&#9658;'; // Play icon
                    isPlaying = false;
                }
            }
            playPauseBtn.addEventListener('click', togglePlayPause);
            video.addEventListener('click', togglePlayPause); // Click video to play/pause
            video.addEventListener('play', () => {
                playPauseBtn.innerHTML = '&#10074;&#10074;';
                isPlaying = true;
                videoOverlayCta.classList.remove('active');
                controls.classList.remove('active'); // Hide controls on play
            });
            video.addEventListener('pause', () => {
                playPauseBtn.innerHTML = '&#9658;';
                isPlaying = false;
                controls.classList.add('active'); // Show controls on pause
            });
            video.addEventListener('ended', () => {
                playPauseBtn.innerHTML = '&#9658;';
                isPlaying = false;
                videoOverlayCta.classList.add('active'); // Show CTA when video ends
                controls.classList.add('active'); // Keep controls visible
            });

            // Update progress bar
            video.addEventListener('timeupdate', () => {
                const progress = (video.currentTime / video.duration) * 100;
                progressBar.style.width = `${progress}%`;
                progressRange.value = progress;
                updateTime();
            });

            // Seek video
            progressRange.addEventListener('input', () => {
                const seekTime = (progressRange.value / 100) * video.duration;
                video.currentTime = seekTime;
            });

            // Clickable progress bar (more precise)
            progressRange.addEventListener('click', (e) => {
                const clickPosition = e.offsetX / progressRange.offsetWidth;
                video.currentTime = clickPosition * video.duration;
            });

            // Update time display
            function formatTime(time) {
                const minutes = Math.floor(time / 60);
                const seconds = Math.floor(time % 60);
                return `${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
            }
            function updateTime() {
                currentTimeElem.textContent = formatTime(video.currentTime);
                if (!isNaN(video.duration)) {
                    durationElem.textContent = formatTime(video.duration);
                }
            }
            video.addEventListener('loadedmetadata', updateTime);

            // Volume control
            volumeRange.addEventListener('input', () => {
                video.volume = volumeRange.value;
                if (video.volume === 0) {
                    volumeBtn.innerHTML = '&#128263;'; // Mute icon
                } else {
                    volumeBtn.innerHTML = '&#128266;'; // Volume icon
                }
            });
            volumeBtn.addEventListener('click', () => {
                if (video.volume === 0) {
                    video.volume = volumeBeforeMute > 0 ? volumeBeforeMute : 0.5; // Restore previous volume or default to 0.5
                    volumeRange.value = video.volume;
                    volumeBtn.innerHTML = '&#128266;';
                } else {
                    volumeBeforeMute = video.volume; // Save current volume
                    video.volume = 0;
                    volumeRange.value = 0;
                    volumeBtn.innerHTML = '&#128263;';
                }
            });

            // Playback speed
            speedSelector.addEventListener('change', () => {
                video.playbackRate = parseFloat(speedSelector.value);
            });

            // Fullscreen
            fullscreenBtn.addEventListener('click', () => {
                if (videoPlayer.requestFullscreen) {
                    videoPlayer.requestFullscreen();
                } else if (videoPlayer.mozRequestFullScreen) { /* Firefox */
                    videoPlayer.mozRequestFullScreen();
                } else if (videoPlayer.webkitRequestFullscreen) { /* Chrome, Safari & Opera */
                    videoPlayer.webkitRequestFullscreen();
                } else if (videoPlayer.msRequestFullscreen) { /* IE/Edge */
                    videoPlayer.msRequestFullscreen();
                }
            });

            // Show controls on mouse move
            let controlsTimeout;
            videoPlayer.addEventListener('mousemove', () => {
                controls.classList.add('active');
                clearTimeout(controlsTimeout);
                controlsTimeout = setTimeout(() => {
                    if (!video.paused) {
                        controls.classList.remove('active');
                    }
                }, 3000); // Hide controls after 3 seconds of inactivity
            });
            videoPlayer.addEventListener('mouseleave', () => {
                if (!video.paused) {
                    controls.classList.remove('active');
                }
            });

            // Engagement tracking (simple example: log progress at intervals)
            let lastLoggedProgress = 0;
            video.addEventListener('timeupdate', () => {
                const currentProgress = Math.floor((video.currentTime / video.duration) * 100);a
                if (currentProgress >= lastLoggedProgress + 25) { // Log every 25%
                    // console.log(`Video watched: ${currentProgress}%`); // For debugging
                    lastLoggedProgress = currentProgress;
                }
            });
        });
    </script>
</body>
</html>
