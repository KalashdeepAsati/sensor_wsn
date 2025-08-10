# Urban Breath — (Crowd Missions, Gamified Sensing)

**What this is:** A professional, pink–white themed WSN prototype that looks nothing like SirenNet. It adds **Crowd Missions** (named geofences), **gamified progress + points**, and a polished dashboard.

## Run (fast)
1. Open `laptop.html` in Chrome (HTTPS origin recommended for mic/cam permissions).
2. On each phone, open `phone.html` in Chrome.
3. Phone → **Grant Mic • Cam • GPS** → **Create Offer** → copy JSON to laptop.
4. Laptop → **Accept Offer** → copy Answer JSON back to phone → **Set Answer**.
5. On the laptop map, **click** to add mission centers (edit name & radius in the list).
6. Click **Send to Phones** — missions broadcast to all connected phones.
7. Phones only sample **when inside an active mission**; progress bar + points update.
8. Watch **Noise (pink heat)** and **Haze (lavender heat)** fill the map. Export data as CSV.

## Notes
- Phones show mission list; tap to activate/deactivate your mission.
- Data flows P2P over WebRTC DataChannel; no server after pairing.
- Haze index is a heuristic from camera frame (saturation, contrast, blue ratio).
