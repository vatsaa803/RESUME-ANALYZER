# RESUME-ANALYZER

A simple AI-powered resume analyzer that compares a resume to a job description and gives:
- Match score (0-100)
- Strengths and gaps
- Missing keywords
- Suggested resume bullets
- ATS optimization tips

## Quick start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
```

If you add `OPENAI_API_KEY` in `.env`, the app uses OpenAI for deeper analysis.
If no key is present (or API fails), it falls back to local heuristic analysis.

## Run

```bash
python analyzer.py --resume-file sample_resume.txt --job-file sample_job.txt
```

## Input format

Use plain text files (`.txt`) for both resume and job description.
You can convert PDF/DOCX to text before running.

## Next improvements

- Add PDF/DOCX ingestion
- Add web UI (Streamlit)
- Export polished, tailored resume suggestions
