Asteria Chart high-precision ephemeris setup

This is optional. The app works without it.

Files:
- asteria-chart-v69-full-audit-clean-optimized.html
- asteria_ephemeris_server.py

Run the optional backend:
1. Install dependency:
   pip install pyswisseph

2. Start the server:
   python asteria_ephemeris_server.py

3. Open Asteria Chart and connect it in the browser console:
   window.ASTERIA_EPHEMERIS_ENDPOINT = "http://127.0.0.1:8765/api/ephemeris"

   Or save it permanently:
   localStorage.setItem("ASTERIA_EPHEMERIS_ENDPOINT", "http://127.0.0.1:8765/api/ephemeris")

The frontend automatically uses its built-in chart engine if the backend is not reachable.
