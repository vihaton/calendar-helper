# calendar-helper
How do you use your life? How could you use it better? Calendar Helper might help you to answer these questions.

## Quick Start

### Installation

1. Create and activate a virtual environment with Python 3.10+:
```bash
uv venv --python 3.10
source .venv/bin/activate
```

2. Install the package in editable mode:
```bash
uv pip install -e .
```

### Google Calendar API Setup

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project (or select existing)
3. Enable the **Google Calendar API**
4. Configure **OAuth consent screen**:
   - User Type: External
   - Add your email to **Test users** list
5. Go to **Credentials** → **Create Credentials** → **OAuth client ID**
   - Application type: **Desktop app**
6. Download the credentials JSON file
7. Save it as `secrets/credentials.json`

### Running the Notebook

1. Open `notebooks/analyze_calendars.ipynb` and select the `.venv` kernel
2. Run the cells - first run will open a browser for OAuth authorization
3. After authorization, `secrets/token.pickle` is created for future use
