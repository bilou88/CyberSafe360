## Requirements

- Python 3.10+
- API key for OpenAI, Anthropic, or other LiteLLM-supported provider

## Installation

```bash
# Clone
git clone https://github.com/GH05TCREW/pentestagent.git
cd pentestagent


.\scripts\setup.ps1   # Windows
./scripts/setup.sh    # Linux/macOS

python -m venv venv
.\venv\Scripts\Activate.ps1  # Windows
source venv/bin/activate     # Linux/macOS
pip install -e ".[all]"
playwright install chromium  # Required for browser tool
```

## Configuration

Créer `.env` dans le project root:

```
ANTHROPIC_API_KEY=sk-ant-...
PENTESTAGENT_MODEL=claude-sonnet-4-20250514
```

Ou avec OpenAI:

```
OPENAI_API_KEY=sk-...
PENTESTAGENT_MODEL=gpt-5
```



## Run

```bash
pentestagent                      
pentestagent -t 192.168.1.1       
pentestagent tui --docker         
```
