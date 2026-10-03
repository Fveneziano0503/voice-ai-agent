# Setup guide

## Public demo
Open `demo/index.html`. No installation, keys, or account required. All six views are synthetic.

## Private voice experiment
1. Use your existing Vapi assistant in a private test environment.
2. Review and adapt `prompts/victoria-system-prompt.md`; it is a public starter.
3. Select model, voice, and transcription providers in your account. No provider IDs or credentials are supplied here.
4. Add a structured output using `config/call-record.schema.json` if your current interface supports JSON Schema input. Attach it to the assistant.
5. Run an authorized browser test, end it, and inspect the transcript and structured output.
6. Execute `docs/test-plan.md` scenarios and record actual results.

The schema describes extracted data; it is not a complete assistant-import configuration. Provider interfaces may change. Refer to current provider documentation for exact fields.
