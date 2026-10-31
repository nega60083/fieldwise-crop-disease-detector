# FieldWise Website Starter
Features: leaf upload, model integration point, confidence warning, Tamil/English text guidance, weather risk notice, session scan history and CSV export.

## Run on Windows
1. Install Python 3.10 or 3.11.
2. Extract this folder and open Terminal inside it.
3. Run `python -m venv .venv`
4. Activate: `.venv\\Scripts\\activate`
5. Install: `python -m pip install -r requirements.txt`
6. Start: `streamlit run app.py`

## Connect your trained AI model
Add `model/disease_model.keras` and `model/class_names.json`. Example labels:
`["Tomato_Healthy", "Tomato_Early_Blight", "Tomato_Late_Blight"]`
Labels must be in exactly the same order as the model outputs. The starter assumes RGB 224x224 input scaled to 0..1; change preprocessing if your training pipeline differs. No trained model is included.

Weather needs internet. History is session-only. Voice playback and IoT hardware are future extensions. AI results are not confirmed diagnoses; do not make pesticide decisions from predictions alone.
