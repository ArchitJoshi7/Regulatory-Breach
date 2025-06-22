📊 Regulatory Breach Alert System using Azure ML

A machine learning pipeline that detects potential regulatory breaches from operational risk control data and sends a consolidated alert email for governance or compliance teams. Built entirely on Azure ML's free-tier services.

🎯 Project Objective

To simulate an early-warning system that identifies potential control failures or regulatory breaches within financial operations — aligned with compliance frameworks such as SOX, Basel II/III, and enterprise risk control structures.

🧰 Tech Stack

Azure Machine Learning Studio (Free-tier Compute Instance)

Python 3.10

scikit-learn (Random Forest Classifier)

pandas, matplotlib

Gmail SMTP for alerting (1 email per batch, not per row)


🧪 How It Works

Synthetic Dataset simulates operational risk data (LOBs, controls, ratings).

Data Preprocessing encodes and splits the dataset.

Random Forest Classifier detects breach-prone patterns.

Confusion Matrix visualizes performance.

Batch Inference Notebook scans new data and sends a single HTML email with all predicted breaches.

🚀 Quickstart

Clone this repo:

git clone https://github.com/<your-username>/Regulatory-Breach.git

Upload files to https://ml.azure.com in your free workspace

Run each notebook in order on a free Compute Instance (DS11 or lower)

Replace your_email@gmail.com and your_app_password in the alert script

(Optional) Schedule 03_batch_inference_and_alerting.ipynb to run periodically

🔐 Security Note

Use a Gmail App Password — never use your actual password for SMTP access.

📈 Sample Output

📧 Email shows table of control_id, lob, risk_rating, etc. for all predicted breaches

📊 Confusion matrix image

📌 Highlights

Fully contained in Azure Free Tier

Modular notebooks for clarity

Realistic simulation of regulatory alerting

🏁 Future Ideas

Azure Logic Apps or Power Automate integration

Add ROC curve & model comparison

CI/CD with GitHub Actions for retraining

📬 Contact

Feel free to connect if you'd like to collaborate, improve, or scale this system!
