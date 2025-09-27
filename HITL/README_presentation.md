Presentation README
===================

Files created:
- `slides.md` — Enhanced Marp/Markdown slide deck based on the HITL paper with concrete case studies, speaker notes, and actionable guidance.

## What's Included

The presentation covers:
- **Real‑world failures**: Knight Capital ($460M), Dutch childcare scandal (10,000 families), hospital diagnostic errors (30% miss rate)
- **Five failure modes**: Speed mismatch, scale mismatch, overtrust, skill erosion, coordination gaps
- **Domain‑specific analysis**: Financial services, healthcare, transportation with concrete examples
- **Technical solutions**: Discriminator agents, monitoring metrics, audit trails
- **12‑month roadmap**: Practical implementation timeline with specific milestones
- **Speaker notes**: Detailed guidance for each slide (25‑30 minute presentation)

How to render
--------------

Option A — Marp CLI (recommended):

```bash
# install marp-cli (requires Node.js)
npm install -g @marp-team/marp-cli

# render to PDF
marp /Users/ankur/projects/pnp/HITL/slides.md --pdf --allow-local-files

# render to PPTX
marp /Users/ankur/projects/pnp/HITL/slides.md --pptx --allow-local-files
```

Option B — VS Code Marp extension
- Install the 'Marp for VS Code' extension.
- Open `slides.md` in VS Code
- Open Command Palette (Cmd+Shift+P on macOS)
- Type "Marp" and select:
  - `Marp: Export slide deck...` for PDF/PPTX/HTML export
  - `Marp: Show preview to the side` to see live preview
- Choose your export format (PDF, PPTX, HTML, PNG, JPEG)

## Presentation Structure

1. **Opening** (5 min): Hook with dramatic statistics, define the problem
2. **Failure Analysis** (10 min): Five failure modes with real‑world examples  
3. **Domain Deep‑Dives** (8 min): Financial, healthcare, transportation case studies
4. **Solutions** (7 min): Discriminator agents, monitoring, implementation patterns
5. **Roadmap & Close** (5 min): 12‑month timeline, resources, next steps

## Audience Adaptation

**For Technical Audiences:**
- Expand discriminator architecture details
- Deep‑dive on monitoring metrics and thresholds
- Show code examples and API patterns

**For Executive Audiences:**  
- Focus on business impact and compliance requirements
- Emphasize cost of failures and ROI of safeguards
- Stress regulatory implications (EU AI Act, etc.)

Next steps I can take
---------------------
- Create executive summary version (10 slides)
- Add technical appendix with implementation details
- Build branded PPTX template with custom styling
- Generate handout materials with key takeaways

