# LeafLine

### A Web-Based Plant Disease Detection System

**BSc (Hons) Computer Science \| University of Wolverhampton**
**Module:** 6CS007 -- Project and Professionalism
**Project status:** Proposal stage / in development

LeafLine is an individual final-year project exploring a
confidence-aware web application that provides an initial indication of
possible plant disease from a leaf photograph. It is intended to support
home gardeners and small-scale growers, not replace professional
agricultural diagnosis.

## Project overview

A user will be able to upload or capture a leaf image and receive a
prediction from a machine-learning model trained as part of this
project. The model is intended to run locally in the browser, with a
confidence indication so that uncertain predictions are not presented as
definitive.

For low-confidence predictions, the application is planned to offer an
optional second opinion through the Gemini API. It will also provide
optional historical weather information as supporting context and allow
signed-in users to review and manage their diagnosis history.

The project investigates whether combining local image inference,
explicit uncertainty communication, selective AI assistance and
contextual weather information can make image-based predictions more
useful and reliable.

## Planned features

- User registration, login and profile management
- Leaf image upload or camera capture, with input validation
- Locally running plant-disease classification model
- Prediction results with confidence scores and uncertainty messaging
- Optional Gemini second opinion for low-confidence predictions
- Optional historical weather context
- Personal diagnosis history, including viewing and deleting records
- Offline local diagnosis after the model has been downloaded
- Short video tutorial explaining image submission and results

The system will focus on a selected set of crops and disease classes
supported by the chosen dataset. It will provide an initial indication
only. It will not claim laboratory-level pathogen identification or
provide pesticide doses.

## Planned technology stack

  Area                      Planned technologies

---

  Frontend                  Next.js, TypeScript, Tailwind CSS
  Backend/API               Node.js, Express
  Database                  PostgreSQL
  Model development         Python, TensorFlow, Keras
  Browser inference         TensorFlow.js
  Optional second opinion   Gemini API
  Historical weather        Open-Meteo Historical Weather API
  Version control           Git and GitHub

These are the technologies proposed in the project plan. The final
implementation may be refined during development and evaluation.

## Research and evaluation

The project will evaluate the model using a held-out test set and
measures including accuracy, per-class precision and recall, macro
F1-score and a confusion matrix. Browser inference time and model size
will also be recorded.

Testing will cover uncertain and unsupported images, invalid uploads,
offline use, Gemini failures, weather-service failures and access
control for diagnosis history. Local-only and hybrid workflows will be
compared. Results and limitations will be documented rather than
assuming that the proposed targets will be achieved.

## Data and responsible use

The initial model work is planned to use public or appropriately
licensed plant-image datasets. Dataset sources, licences and class
selection will be recorded.

Raw leaf photographs will not be stored by default. Location use for
weather context will be optional. AI-generated text and model
predictions will be presented as indicative information, not definitive
agricultural advice. Any usability testing involving people will take
place only after the required ethics review and approval.

## Academic context

This project is being undertaken individually for **6CS007 -- Project
and Professionalism**, as part of the **BSc (Hons) Computer Science**
programme associated with the University of Wolverhampton.

The proposal identifies **Nishant Bhurtel** as the project supervisor.
The project is currently at the proposal stage, so features and
technologies described here are planned rather than completed.

---

*This README will be updated as the project develops.*
