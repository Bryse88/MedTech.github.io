# Disability Rehabilitation Website

A modern, responsive website for Disability Rehabilitation, featuring a device to help partially able individuals exercise in supine, sitting, and standing positions.

## Features

- Responsive, modern design with vertical scrolling layout
- Contact form with email functionality
- Flask backend for easy deployment and form handling
- Blue and white health-focused color scheme

## Project Structure

```
disability-rehabilitation/
├── app.py                  # Flask application
├── .env                    # Environment variables (excluded from git)
├── requirements.txt        # Python dependencies
├── static/                 # Static assets
│   ├── css/
│   │   └── style.css       # Main stylesheet
│   ├── js/
│   │   └── main.js         # Client-side JavaScript
│   └── images/             # Image assets
│       └── device-placeholder.jpg
└── templates/              # Flask templates
    └── index.html          # Main template file
```

## Setup Instructions

1. Clone the repository
   ```
   git clone https://github.com/your-username/disability-rehabilitation.git
   cd disability-rehabilitation
   ```

2. Create a virtual environment
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies
   ```
   pip install -r requirements.txt
   ```

4. Set up environment variables
   ```
   # Copy the example .env file and modify with your values
   cp .env.example .env
   ```

5. Run the application
   ```
   python app.py
   ```

6. Open your browser and navigate to `http://127.0.0.1:5000`

## Email Setup

To enable the contact form functionality:

1. Create a Gmail account or use an existing one
2. Enable 2-Factor Authentication
3. Generate an App Password (Google Account → Security → App Passwords)
4. Update the `.env` file with your email credentials:
   ```
   EMAIL_ADDRESS=your-email@gmail.com
   EMAIL_PASSWORD=your-app-password
   RECEIVER_EMAIL=where-to-receive-messages@example.com
   ```

## Deployment

### Heroku

1. Create a `Procfile` with:
   ```
   web: gunicorn app:app
   ```

2. Deploy to Heroku:
   ```
   heroku create disability-rehabilitation
   git push heroku main
   ```

3. Set environment variables on Heroku:
   ```
   heroku config:set SECRET_KEY=your-secret-key
   heroku config:set EMAIL_ADDRESS=your-email@gmail.com
   heroku config:set EMAIL_PASSWORD=your-app-password
   heroku config:set RECEIVER_EMAIL=recipient@example.com
   ```

### GitHub Pages (Frontend only)

Since GitHub Pages only supports static sites, you'll need a third-party form handling service like Formspree.

## License

[MIT License](LICENSE)

## Contact

For any inquiries, please reach out to us at info@disabilityrehab.org.