# Weather Predictor — Run Instructions

This repo contains two ways to run the Weather Predictor UI:

1) Streamlit app (interactive, Python-powered)

- Start the app:
  - Open PowerShell in the project folder and run:
    ```powershell
    streamlit run "weather_predictor_app (1).py"
    ```
  - Once started, open Chrome and visit: `http://localhost:8501`
    - Or open Chrome from PowerShell: `start chrome http://localhost:8501`
  - To change the port: `streamlit run "weather_predictor_app (1).py" --server.port 8502`

2) Static HTML demo (no server required — open locally in Chrome)

- Open `weather_predictor_static.html` directly in Chrome (File → Open File), or from PowerShell:
  ```powershell
  start chrome "file:///d:/Rithul VIT/Software Config Mgmt/Project/Weather-Prediction/weather_predictor_static.html"
  ```
- This static version uses a simple exported linear regression model and a nearest-neighbor lookup to predict a weather condition, so it runs entirely in your browser.

Notes:
- The static demo is intentionally simple; it is designed to work offline and to run purely in the browser. If you'd like a full-featured web app (HTML frontend + Flask/FastAPI backend) that runs locally and uses the trained models, I can scaffold that next.
