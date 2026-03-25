Email Phishing Detector

A beginner-friendly machine learning project that detects phishing emails by analyzing their content, URLs, and suspicious patterns.

What It Does

This tool analyzes email content and tells you whether it's a phishing attempt or a safe email. It looks for:
- Suspicious keywords (urgent, verify, account, etc.)
- URL patterns (IP addresses, unusual domains)
- Requests for personal information
- Urgent language designed to pressure you
- Other red flags commonly found in phishing emails

Why It Matters

Phishing attacks are one of the most common cybersecurity threats. This tool helps:
- Protect yourself from email scams
- Learn how machine learning can detect patterns
- Understand what makes an email suspicious

How It Works

1. Feature Extraction: The email is analyzed for 11 different features
2. Machine Learning: A Random Forest classifier is trained on example emails
3. Prediction: New emails are classified as "Safe" or "Phishing" with confidence scores

Tech Stack

- Python 3.7+
- scikit-learn (Machine Learning)
- pandas (Data handling)
- joblib (Model persistence)

 Setup Instructions

1. Clone or Download the Project

bash
git clone https://github.com/yourusername/email-phishing-detector.git
cd email-phishing-detector
pip install -r requirements.txt
python src/detect_phishing.py --file emails.txt
URGENT: Your PayPal account has been limited. Click here to verify: http://paypal-verify.com
🚨 PHISHING EMAIL DETECTED
Confidence: 95.3%
Threat Level: HIGH

Suspicious Features Found:
  • Contains 3 suspicious keywords
  • Contains urgent/emergency language
  • Requests personal information
  • Contains URLs
Customization
phishing_emails.append("Your custom phishing email here")
safe_emails.append("Your custom safe email here")
Adding new features
def extract_your_feature(email_text):
    Add your feature extraction logic
    return feature_value
    🚨 Detect phishing emails before they fool you! This project uses machine learning (Random Forest classifier) to analyze email content and identify phishing attempts. Perfect for beginners learning ML, cybersecurity, or Python development.

🔍 Features:
• Analyzes email text for suspicious keywords and patterns
• Detects malicious URLs and IP-based links
• Identifies urgent language and personal info requests
• Provides confidence scores for predictions
• Interactive CLI for testing emails

📚 Educational Value:
Learn how ML can be applied to real-world security problems, understand phishing detection techniques, and build a complete Python project from scratch.

How to run:

def check_phishing(email):
    suspicious_words = ["urgent", "click now", "verify", "password", "limited time"]

    score = 0

    for word in suspicious_words:
        if word in email.lower():
            score += 1

    if score >= 2:
        return "⚠️ Phishing Email"
    else:
        return "✅ Safe Email"

email = input("Enter email content: ")
print(check_phishing(email))
