# SMPRADE

**SMPRADE** is an advanced <b>stock market prediction platform</b> developed as a final year project. It leverages various technologies to offer stock price predictions, up-to-date news, and detailed data visualizations.

## 🚀 Features

- **Stock Price Prediction**: Predict future stock prices using linear regression models.
- **Real-Time News**: Fetch and display the latest stock-related news using news.api.
- **Interactive Charts**: Visualize stock data with interactive charts using Plotly.js.
- **Comprehensive Data**: Integrate data from Alphavantage API and yfinance for accurate analysis.
- **User Signup/Login**: Sign Up your account and use it.
- **Posts Feed/Profile Picture Upload**: User can see post of another users into their feed and upload their profile picture.

## 🛠️ Technologies Used

- **Django**: Framework for building the web application.
- **HTML/CSS/JavaScript**: For frontend development and styling.
- **Alphavantage API**: For fetching stock market data.
- **yfinance**: For additional stock data and historical prices.
- **news.api**: To gather and display stock-related news.
- **NumPy & Pandas**: For data manipulation and analysis.
- **scikit-learn**: For implementing linear regression models.
- **Plotly.js**: For creating interactive charts and visualizations.
- **MySQL**: Default database for storing user data and application information.

## 📦 Installation

To run SMPRADE locally, follow these steps:

**1. Clone the repository**:

git clone https://github.com/Bilal-Ansarii/SMPRADE.git

**2. Navigate to project directory by**:

cd SMPRADE

**3. Create a virtual environment for dependency management:**

python -m venv venv

**4. Activate it:**

On Windows:
venv\Scripts\activate

On macOS/Linux:
source venv/bin/activate

**5. Install Dependencies:**

pip install -r requirements.txt

**6. Configure Database:**

Ensure your settings.py is configured to use MySQL or your chosen database. Update the DATABASES setting in settings.py. You can use DB of your choice.

DATABASES = {
    'default': {<br>
        'ENGINE': 'django.db.backends.mysql',<br>
        'NAME': 'your_db_name',   <----<br>
        'USER': 'your_db_user',   <----<br>
        'PASSWORD': 'your_db_password',<br>
        'HOST': 'localhost',<br>
        'PORT': '3306',<br>
    }
}

**7. Run Migrations:** Apply the migrations to set up your database schema

python manage.py makemigrations

python manage.py migrate

**8. Create Superuser:** Create a superuser account to access the Django admin interface:

python manage.py createsuperuser

**9. Start the development server:**

python manage.py runserver

Access the application in your web browser at http://127.0.0.1:8000/.
