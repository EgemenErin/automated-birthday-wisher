# Birthday Wisher

This script sends an automatic birthday wish email to people whose birthdays are listed in a CSV file. The email content is randomly selected from three letter templates.

## Prerequisites

- Python 3.x
- Required Python packages: `pandas`, `smtplib`

## Setup

1. Clone the repository or download the script files.

2. Install the required Python packages if you don't have them already:

    ```sh
    pip install pandas
    ```

3. Prepare the CSV file named `birthdays.csv` in the following format:

    ```csv
    name,email,year,month,day
    John Doe,johndoe@example.com,1990,5,18
    Jane Smith,janesmith@example.com,1985,12,25
    ```

5. Replace the placeholders `YOUR EMAIL`, `YOUR PASSWORD`, and `YOUR EMAIL PROVIDER SMTP SERVER ADDRESS` in the script with your actual email credentials and SMTP server address.

## Usage

1. Run the script:

    ```sh
    python birthday_wisher.py
    ```

2. The script will check if today is anyone's birthday as per the `birthdays.csv` file. If yes, it will send an email to the birthday person with a randomly selected letter template.

## Important Notes

- Ensure that you have allowed less secure apps to access your email account if you are using Gmail. You can enable this in your Google account settings.
- Be cautious with your email credentials. Consider using environment variables or a configuration file to store sensitive information.

## License

This project is licensed under the MIT License.
