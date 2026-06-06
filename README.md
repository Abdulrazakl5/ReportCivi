# ReportCivi - Anti-Corruption Platform for Nigeria

A comprehensive mobile and web application designed to combat corruption through citizen engagement, transparent reporting, and accountability mechanisms.

## 🎯 Mission

To empower Nigerian citizens with tools to report corruption anonymously, track government accountability, and promote transparency in public services.

## ✨ Key Features

### 1. **Anonymous Reporting System**
- Secure, encrypted corruption incident reporting
- Multiple submission formats (text, images, audio, documents)
- Real-time report tracking and status updates
- Whistleblower protection protocols

### 2. **Transparency Dashboard**
- Government budget tracking and visualization
- Procurement data display
- Project milestone monitoring
- Expenditure vs. allocation comparisons

### 3. **Citizen Scorecard**
- Rate local government services and officials
- Community feedback aggregation
- Performance metrics and rankings
- Accountability feedback loop

### 4. **Investigation Tracking**
- Case status visibility for reported incidents
- Integration with ICPC and EFCC databases
- Secure communication with investigators
- Impact metrics and resolved case showcase

### 5. **Educational Hub**
- Citizen rights and responsibilities
- Anti-corruption laws and regulations
- Safe reporting guidelines
- Success stories and case studies

### 6. **Community Forum**
- Moderated civic discussions
- Resource sharing
- Local anti-corruption initiatives
- Peer support and awareness

## 🛠 Tech Stack

### Backend
- **Runtime:** Python 3.11
- **Framework:** Flask
- **Database:** PostgreSQL with encryption
- **Cache:** Redis
- **Authentication:** JWT with role-based access

### Frontend
- **Web:** React 18 with TypeScript
- **Mobile:** React Native (future)
- **State Management:** Redux
- **UI Framework:** Material-UI

### Security & Infrastructure
- **Encryption:** AES-256 at rest, TLS in transit
- **Hosting:** AWS / Docker
- **CI/CD:** GitHub Actions
- **Monitoring:** Logging & error tracking

## 📁 Project Structure

```
ReportCivi/
├── backend/
│   ├── src/
│   │   ├── api/
│   │   ├── models/
│   │   ├── services/
│   │   └── config/
│   ├── tests/
│   ├── Dockerfile
│   ├── .env.example
│   └── requirements.txt
├── frontend/
│   └── web/
│       ├── src/
│       ├── public/
│       ├── Dockerfile
│       └── package.json
├── docs/
├── docker-compose.yml
├── .github/workflows/
└── LICENSE
```

## 🚀 Quick Start

### Using Docker (Recommended)
```bash
git clone https://github.com/Abdulrazakl5/ReportCivi.git
cd ReportCivi
docker-compose up
```

Access:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000/api
- Health check: http://localhost:5000/api/health

### Local Development

#### Backend
```bash
cd backend
pip install -r requirements.txt
cp .env.example .env
python run.py
```

#### Frontend
```bash
cd frontend/web
npm install
npm start
```

## 📚 Documentation

- [API Documentation](./docs/API_DOCUMENTATION.md) - Complete REST API reference
- [Architecture Guide](./docs/ARCHITECTURE.md) - System design and components
- [Deployment Guide](./docs/DEPLOYMENT.md) - Production deployment
- [Contributing Guidelines](./docs/CONTRIBUTING.md) - How to contribute

## 🔒 Security & Privacy

- ✅ End-to-end encrypted reports
- ✅ Anonymous reporting with no IP logging
- ✅ GDPR and Nigerian data protection compliance
- ✅ Password hashing with bcrypt
- ✅ JWT-based authentication
- ✅ Role-based access control

## 📊 Key Endpoints

### Reports
- `POST /api/reports` - Submit a report
- `GET /api/reports` - List all reports
- `GET /api/reports/<id>` - Get report details
- `PUT /api/reports/<id>` - Update report
- `POST /api/reports/<id>/upvote` - Upvote report

### Authentication
- `POST /api/auth/register` - Create account
- `POST /api/auth/login` - Login user
- `GET /api/auth/profile` - Get user profile
- `PUT /api/auth/profile` - Update profile

### Dashboard
- `GET /api/dashboard/statistics` - Dashboard stats
- `GET /api/dashboard/reports-by-category` - Category breakdown
- `GET /api/dashboard/reports-by-severity` - Severity breakdown
- `GET /api/dashboard/reports-timeline` - Timeline data

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](./docs/CONTRIBUTING.md) for guidelines.

## 📞 Support

- **Issues:** [GitHub Issues](https://github.com/Abdulrazakl5/ReportCivi/issues)
- **Email:** support@reportcivi.ng
- **Docs:** [Full Documentation](./docs)

## 📄 License

MIT License - See [LICENSE](LICENSE) file

## 🙏 Acknowledgments

- UNODC Coding4Integrity Initiative
- Nigeria's ICPC and EFCC
- Civil society organizations
- Community contributors

---

**Let's build a more transparent Nigeria together! 🇳🇬**