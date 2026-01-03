# Legal AI Governance Tool

**Live Demo:** https://ashleysally00.github.io/legal-ai-governance-tool/

A lightweight governance and evaluation harness for testing how AI systems behave when answering questions about legal documents.

<br>
<p align="center">
  <img src="images/evaluation-example.png" alt="Evaluation example" width="600">
</p>
<p align="center"><em>Governance check showing document input, question, and evaluated response</em></p>


## What this demonstrates

This tool evaluates whether AI responses:
- Stay grounded in the provided document
- Correctly refuse when information is missing
- Avoid hallucinating unsupported claims
- Respect strict document-boundary constraints

Example scenarios:
- Grounded question resulting in an accurate, document-based response
- Out-of-scope question resulting in a correct refusal
- Hallucination trap detected and blocked
- Vague prompt resulting in a safe refusal with redirection

The focus is on evaluation and boundary enforcement, not on generating legal guidance.

---
## Public demo mode

The GitHub Pages site runs in Demo Mode using simulated responses.

Why this repository uses a demo configuration:

- A live model would require an API key
- In a public, client-side site that key would be exposed
- Therefore the public version is a demo

The purpose of this repository is to demonstrate evaluation and governance logic without calling external services.

In a production setting, model access would be handled server-side.

