# Gesture-Breaker

Neon‑arcade, webcam‑controlled brick breaker. Steer a glowing paddle with your hand, launch with an open palm, catch with a fist-powered magnet, and score as many points as you can in 60 seconds.

**How to play**
- Move hand left/right to steer the paddle (webcam mirrored like a selfie).
- Open palm to launch the ball.
- Make a fist near the paddle to magnet‑catch and relaunch (has cooldown).
- Goal: score as many points as possible in 60 seconds.

Scoring and items
- ⭐️ Star: +50 points
- 🤩 Bonus star: visually marked “double‑point” star from orange bounty bricks (adds +50 points; visual distinction)
- 💀 Skull: shrinks the paddle temporarily (avoid)
- Orange bricks drop extra stars more often
- 100 points unlocks a second ball; you’ll juggle two balls after that

Rules and feedback
- 3 lives per run; missing the ball loses a life.
- Dynamic bounces based on where the ball hits the paddle.
- Combo sound escalates as you break bricks without touching the paddle.
- Local leaderboard (saved in your browser) ranks your best 60‑second runs.

Run it
- Live (GitHub Pages): https://YOUR_USERNAME.github.io/REPO_NAME
- Locally (needs HTTPS or localhost for camera):
  - With Node: npx http-server . then open http://127.0.0.1:8080
  - Or use any static server/“Live Server” extension
- Allow camera access when prompted. Good lighting improves tracking.

Tech stack
- MediaPipe Hands (gesture + x‑axis hand tracking)
- HTML5 Canvas (rendering, particles)
- Web Audio API (synth SFX)
- Vanilla JavaScript (physics, collisions, game state, localStorage leaderboard)

Notes
- Works best on desktop Chrome/Edge; mobile can work with steady framing and good light.
- No images required; items and UI use emojis with colored glows. If you add sprites later, point index.html to them and redeploy.

License
- Your code license here (MIT recommended). MediaPipe and any third‑party assets follow their respective licenses.
