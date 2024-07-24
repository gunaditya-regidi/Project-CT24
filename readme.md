\# Clinical Trials Topic Modeling and Tracking Project

\## Introduction

This project provides a system for tracking and visualizing topics in
clinical trials data using DeBERTa for topic modeling and lexical chains
for topic tracking. The final output is visualized through a Flask web
application.

\## Directory Layout

\`\`\` project/ \|\-- app/ \| \|\-- static/ \| \| \|\-- css/ \| \| \|\--
style.css \| \|\-- templates/ \| \| \|\-- index.html \| \| \|\--
results.html \| \|\-- app.py \| \|\-- data/ \| \|\-- clinical_trials.csv
\| \|\-- preprocessed_clinical_trials.csv \| \|\--
topic_modeled_trials.csv \| \|\-- tracked_trials.csv \| \|\-- script/ \|
\|\-- preprocess.py \| \|\-- topic_modeling.py \| \|\--
topic_tracking.py \| \|\-- scoring.py \| \|\-- requirements.txt \| \|\--
README.md \`\`\`

\## Installation

\### Prerequisites

\- Python 3.7+ - pip (Python package installer)

\### Steps

1\. Clone the repository: \`\`\`sh git clone
https://github.com/your-username/project.git cd project \`\`\`

2\. Create and activate a virtual environment (optional but
recommended): \`\`\`sh python -m venv venv source venv/bin/activate \#
On Windows use \`venv\\Scripts\\activate\` \`\`\`

3\. Install the required packages: \`\`\`sh pip install -r
requirements.txt \`\`\`

\## Usage

\### Preprocessing Data

Run the preprocessing script to clean the clinical trials data:

\`\`\`sh python script/preprocess.py \`\`\`

\### Topic Modeling

Run the topic modeling script to encode the text and assign topics:

\`\`\`sh python script/topic_modeling.py \`\`\`

\### Topic Tracking

Run the topic tracking script to build lexical chains and track topics:

\`\`\`sh python script/topic_tracking.py \`\`\`

\### Running the Flask App

Start the Flask application to visualize the data:

\`\`\`sh python app/app.py \`\`\`

\### Access the Web Application

Open your web browser and navigate to \`http://127.0.0.1:5000/\`. Enter
a condition or drug name to visualize the tracked topics.

\## Code Overview

\### Preprocessing Script (preprocess.py)

This script cleans and preprocesses the clinical trials data.

\### Topic Modeling Script (topic_modeling.py)

This script encodes the text using DeBERTa and assigns topics using
KMeans clustering.

\### Topic Tracking Script (topic_tracking.py)

This script builds lexical chains to track topics related to specific
conditions or drugs.

\### Flask Application (app.py)

This script sets up a Flask web application to visualize the tracked
topics.

\## Running the Project

1\. \*\*Setup the Environment:\*\*  - Ensure you have Python 3.7+
installed.  - Install the required packages:

\`\`\`sh pip install -r requirements.txt \`\`\`

2\. \*\*Preprocess the Data:\*\*  - Run the preprocessing script to
clean the clinical trials data:

\`\`\`sh python script/preprocess.py \`\`\`

3\. \*\*Topic Modeling:\*\*  - Run the topic modeling script to encode
the text and assign topics:

\`\`\`sh python script/topic_modeling.py \`\`\`

4\. \*\*Topic Tracking:\*\*  - Run the topic tracking script to build
lexical chains and track topics:

\`\`\`sh python script/topic_tracking.py \`\`\`

5\. \*\*Run the Flask App:\*\*  - Start the Flask application to
visualize the data:

\`\`\`sh python app/app.py \`\`\`

6\. \*\*Access the Web Application:\*\*  - Open your web browser and
navigate to \`http://127.0.0.1:5000/\`.  - Enter a condition or drug
name to visualize the tracked topics.

\## References

\- \*\*DeBERTa Model:\*\* \[DeBERTa: Decoding-enhanced BERT with
Disentangled Attention\](https://arxiv.org/abs/2006.03654) - \*\*Flask
Documentation:\*\* \[Flask - A micro web framework for
Python\](https://flask.palletsprojects.com/) - \*\*KMeans
Clustering:\*\* \[KMeans Clustering -
scikit-learn\](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) -
\*\*Pandas Documentation:\*\* \[Pandas - Python Data Analysis
Library\](https://pandas.pydata.org/)

\## Relevant Researches

1\. \*\*Transformers for NLP:\*\* Vaswani, A., Shazeer, N., Parmar, N.,
Uszkoreit, J., Jones, L., Gomez, A. N., \... & Polosukhin, I. (2017).
Attention is all you need. Advances in neural information processing
systems, 30. 2. \*\*Text Mining and Clinical Trials:\*\* Nadkarni, P.
M., Ohno-Machado, L., & Chapman, W. W. (2011). Natural language
processing: an introduction. Journal of the American Medical Informatics
Association, 18(5), 544-551. 3. \*\*Applications of Lexical Chains:\*\*
Barzilay, R., & Elhadad, M. (1999). Using lexical chains for text
summarization. Advances in automatic text summarization, 111, 10-17.
