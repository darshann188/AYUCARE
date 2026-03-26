# AYUCARE - Ayurvedic Healthcare Platform

![AYUCARE Logo](Darshan/static/assets/img/ayucare%20logo.png)

AYUCARE is a comprehensive Ayurvedic healthcare platform that combines traditional Ayurvedic medicine with modern machine learning technology to provide personalized health solutions. The platform offers disease prediction, medicine recommendations, treatment center locator, and health tips to promote holistic wellness.

## 🌟 Features

### 🏥 Core Healthcare Services
- **Disease Prediction**: AI-powered symptom analysis for early disease detection
- **Medicine Recommendation**: Personalized Ayurvedic medicine suggestions based on health conditions
- **Treatment Centers**: Interactive map showing Ayurvedic hospitals and clinics in Bangalore
- **Health Tips**: Daily wellness guidance and preventive healthcare advice

### 👤 User Management
- Secure user registration and authentication
- Personalized health dashboard
- User profile management
- Session-based login system

### 📱 User Experience
- Fully responsive design for all devices
- Interactive FAQ section with contact form
- Modern UI with gradient designs and animations
- Touch-friendly mobile interface

## 🛠️ Tech Stack

### Backend
- **Framework**: Flask (Python web framework)
- **Database**: SQLite with SQLAlchemy ORM
- **Authentication**: Flask-Login with Flask-Bcrypt
- **Forms**: Flask-WTF for form handling and validation

### Frontend
- **HTML5**: Semantic markup and accessibility
- **CSS3**: Tailwind CSS for responsive styling
- **JavaScript**: Vanilla JS for interactivity
- **Icons**: Font Awesome for UI elements

### Machine Learning
- **Disease Prediction**: Decision Tree Classifier (Scikit-learn)
- **Medicine Recommendation**: ML-based drug suggestion system
- **Data Processing**: NumPy and Pandas for data manipulation

### Maps & Visualization
- **Interactive Maps**: Leaflet.js for treatment center locator
- **Charts**: Matplotlib for data visualization (if needed)

### Development Tools
- **Version Control**: Git
- **Environment**: Python virtual environment
- **Package Management**: pip
- **IDE**: VS Code recommended

## 📁 Project Structure

```
AYUCARE-main (2)/
├── Darshan/                    # Main Flask Application
│   ├── app.py                 # Main application file
│   ├── database.db           # SQLite database
│   ├── templates/            # HTML templates
│   │   ├── index.html        # Home page
│   │   ├── service.html      # Disease prediction
│   │   ├── med_service.html  # Medicine recommendation
│   │   ├── doc_service.html  # Treatment centers
│   │   ├── health_tips.html  # Health tips
│   │   ├── faq.html          # FAQ and contact
│   │   ├── signin.html       # Login page
│   │   └── register.html     # Registration page
│   └── static/               # Static assets
│       └── assets/
│           └── img/          # Images and logo
├── omkarg/                   # Disease Prediction Model
│   └── Disease_Prediction_Model/
│       ├── DecisionTree-Model.sav  # Trained ML model
│       ├── demo.ipynb        # Demo notebook
│       └── main.ipynb        # Main model notebook
├── Sanket/                   # Medicine Recommendation Model
│   ├── Drug Recommendation Model.ipynb
│   ├── Datasets/            # Training datasets
│   └── drugTree.pkl         # Model pickle file
├── Kiran/                   # Additional components
│   ├── app.py               # Alternative implementation
│   └── Various HTML files
├── requirements.txt         # Python dependencies
└── README.md               # Project documentation
```

## 🚀 Installation & Setup

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)
- Git

### Step-by-Step Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/ayucare.git
   cd ayucare
   ```

2. **Create Virtual Environment**
   ```bash
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Navigate to Main Application**
   ```bash
   cd Darshan
   ```

5. **Run the Application**
   ```bash
   python app.py
   ```

6. **Access the Application**
   Open your browser and go to: `http://127.0.0.1:5000`

## 📖 Usage

### For Users
1. **Register**: Create a new account with your personal details
2. **Login**: Access your personalized dashboard
3. **Disease Prediction**: Input symptoms to get health insights
4. **Medicine Recommendation**: Get personalized Ayurvedic medicine suggestions
5. **Find Treatment Centers**: Use the interactive map to locate nearby Ayurvedic hospitals
6. **Health Tips**: Access daily wellness guidance
7. **Contact Support**: Use the FAQ section to get in touch

### For Developers
- Modify templates in `templates/` directory
- Update styles using Tailwind CSS classes
- Add new routes in `app.py`
- Train new ML models in respective directories

## 🔗 API Endpoints

| Method | Endpoint | Description | Authentication |
|--------|----------|-------------|----------------|
| GET | `/` | Home page | No |
| GET/POST | `/register` | User registration | No |
| GET/POST | `/signin` | User login | No |
| GET | `/logout` | User logout | Yes |
| GET/POST | `/service` | Disease prediction | Yes |
| GET/POST | `/med_service` | Medicine recommendation | Yes |
| GET | `/doc_service` | Treatment centers | Yes |
| GET | `/health_tips` | Health tips | Yes |
| GET/POST | `/faq` | FAQ and contact | No |

## 🤖 Machine Learning Models

### Disease Prediction Model
- **Algorithm**: Decision Tree Classifier
- **Input**: 31 symptom parameters
- **Output**: Disease prediction with confidence score
- **Training Data**: Ayurvedic symptom-disease correlation dataset

### Medicine Recommendation Model
- **Algorithm**: Machine Learning classification model
- **Input**: Disease, age, gender, severity
- **Output**: Personalized medicine recommendations
- **Training Data**: Drug prescription dataset

## 🎨 UI/UX Design

### Design Principles
- **Ayurvedic Theme**: Green and earthy color palette
- **Accessibility**: WCAG compliant design
- **Mobile-First**: Responsive across all devices
- **Intuitive Navigation**: Clear user flow and information hierarchy

### Key Design Elements
- Gradient backgrounds and smooth animations
- Card-based layouts for better content organization
- Interactive elements with hover effects
- Loading states and feedback messages
- Consistent typography and spacing

## 🔧 Development Workflow

### Local Development
1. Create feature branch: `git checkout -b feature/new-feature`
2. Make changes and test locally
3. Commit changes: `git commit -m "Add new feature"`
4. Push to branch: `git push origin feature/new-feature`
5. Create Pull Request

### Code Quality
- Follow PEP 8 Python style guide
- Use meaningful variable and function names
- Add comments for complex logic
- Test all new features before committing

### Deployment
1. Set up production environment
2. Configure environment variables
3. Set up database for production
4. Deploy using Gunicorn or similar WSGI server
5. Configure reverse proxy (nginx recommended)

## 🤝 Contributing

We welcome contributions to AYUCARE! Here's how you can help:

### Ways to Contribute
- **Bug Reports**: Report issues via GitHub Issues
- **Feature Requests**: Suggest new features or improvements
- **Code Contributions**: Submit pull requests with fixes or enhancements
- **Documentation**: Improve documentation and guides
- **Testing**: Help test new features and report bugs

### Contribution Guidelines
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Ensure code follows project standards
6. Submit a pull request with clear description

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Ayurvedic Community**: For preserving traditional healthcare knowledge
- **Open Source Community**: For providing excellent tools and libraries
- **Contributors**: For their valuable contributions to the project
- **Users**: For their feedback and support

## 📞 Support

For support, questions, or feedback:
- **Email**: info@ayucare.com
- **GitHub Issues**: [Create an issue](https://github.com/your-username/ayucare/issues)
- **FAQ**: Visit our FAQ section in the application

## 🔮 Future Enhancements

- [ ] Mobile app development (React Native)
- [ ] Advanced ML models for better predictions
- [ ] Integration with wearable health devices
- [ ] Multi-language support
- [ ] Telemedicine consultation features
- [ ] Health tracking and analytics dashboard
- [ ] Integration with pharmacy systems
- [ ] Offline mode for critical features

---

**AYUCARE** - Bridging Traditional Wisdom with Modern Technology for Holistic Healthcare 🌿⚕️