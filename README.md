## Abraham Asimeh

Founder and CTO at Harmonia. I build LLM and computer vision systems and put them
in front of real users.

### What I am working on

Harmonia reads compatibility from three signals: visual taste, personality inferred
from open text, and HLA immune dissimilarity. The first product out of it, Your Eye,
is live at harmoniaengine.com. You rate a set of faces and it describes your own eye
back to you, from your ratings and nothing else. The wider matching platform is still
in build.

Most of my time goes on the scoring. Personality is inferred from free text using
Gemini on Vertex AI, with calibrated per-trait anchors, prompting built to stop the
model clustering its scores around the mean, and a second observer that re-scores when
confidence falls below a threshold. Synthetic scores are flagged and held out of the
production anchor pool, so machine-generated data can be analysed without ever
contaminating live scoring. Visual preference is a fine-tuned vision model over a
research face corpus.

### Stack

Python, FastAPI, PostgreSQL, Alembic, Redis, Docker. Google Cloud Run and Vertex AI
for the platform. Railway for Your Eye, two services deploying straight from GitHub on
push. React, TypeScript and Vite on the front end, plus a fair amount of
dependency-free vanilla JavaScript where a framework would have been noise.

### Why most of my work is not here

The production repositories are private and will stay that way. They hold special
category personal data and research face datasets whose licences do not permit
redistribution. I am happy to walk through the architecture, the schema, the
migrations or the calibration design on request.

### Before this

Google, gTech Ads, Customer Solutions Engineering, October 2024 to March 2026.
Completed a Level 3 Data Technician apprenticeship. Before that, Google YouTube,
creator marketing.
