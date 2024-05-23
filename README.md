# Project Nightangle: Email Automation with GPT and Python

Welcome to Project Nightangle, an advanced email automation tool leveraging GPT-3 and Python. This project aims to simplify and automate email management, making it efficient to draft, send, and manage emails with minimal manual intervention.

## Features

- **Automated Email Drafting**: Uses GPT-3 to generate context-aware and personalized email drafts.
- **Intelligent Replies**: Automatically replies to emails based on the context and content of the received email.
- **Inbox Management**: Efficiently reads and processes emails to ensure no important information is missed.
- **Customizable Email Templates**: Allows users to customize email templates for different purposes.
- **Send Emails with Attachments**: Supports sending emails with attachments for richer communication.
- **Scheduled Emails**: Schedule emails to be sent at a later time.
- **Logging and Monitoring**: Keeps logs of sent and received emails for monitoring and auditing.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Git
- An OpenAI API key

### Installation

1. **Clone the Repository**

    ```sh
    git clone https://github.com/Alokbpandey/project_nightangle-email-automation-eith-gpt-and-python-.git
    cd project_nightangle-email-automation-eith-gpt-and-python-
    ```

2. **Set Up Virtual Environment**

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies**

    ```sh
    pip install -r requirements.txt
    ```

4. **Configure Environment Variables**

    Create a `.env` file in the root directory and add the following configuration:

    ```env
    OPENAI_API_KEY=your_openai_api_key
    EMAIL_ADDRESS=your_email@example.com
    EMAIL_PASSWORD=your_email_password
    EMAIL_SMTP_HOST=smtp.your-email-provider.com
    EMAIL_SMTP_PORT=587
    EMAIL_IMAP_SERVER=imap.your-email-provider.com
    ```

### Usage

1. **Running the Script**

    ```sh
    python email_bot.py
    ```

2. **Automated Email Drafting**

    The script will automatically draft replies to unread emails in your inbox. You can review these drafts before they are sent.

3. **Sending Emails**

    Use the script to send emails with custom messages or predefined templates.

    ```python
    from email_bot import send_email

    send_email(to="recipient@example.com", subject="Subject", body="Email body", attachments=["file.txt"])
    ```

### Customization

- **Templates**: Customize the email templates in the `templates` directory to fit your needs.
- **Scheduling**: Modify the scheduling logic in `scheduler.py` to set up email schedules.

### Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Contact

For any questions or suggestions, please open an issue or contact the repository owner.

