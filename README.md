# SkillShare Hub - Skill Swap Marketplace

**A Peer-to-Peer Skill Swap Platform** built with React.js, TypeScript, and Tailwind CSS.

**Description:** A platform where users can trade skills (e.g., "I'll teach you coding if you teach me guitar") instead of paying money. SkillShare Hub connects people who want to exchange skills without monetary transactions through an intuitive web application.

---

## 🚀 Quick Start

### Prerequisites
- Node.js (v16.0.0 or higher)
- npm or yarn package manager

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/codewithjihad1/skill-swap-requirements.git
   cd skill-swap-requirements
   ```

2. **Install dependencies:**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up Tailwind CSS:**
   ```bash
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init -p
   ```

4. **Start the development server:**
   ```bash
   npm start
   # or
   yarn start
   ```

5. **Open your browser and visit:** `http://localhost:3000`

---

## 📁 Project Structure

The project follows a feature-based architecture with TypeScript and follows React best practices:

```
skillshare-hub/
├── public/                     # Static files
│   ├── index.html
│   ├── favicon.ico
│   └── manifest.json
├── src/
│   ├── components/             # Reusable UI components
│   │   ├── ui/                # Basic UI components (Button, Input, Modal, etc.)
│   │   │   ├── Button/
│   │   │   │   ├── Button.tsx
│   │   │   │   ├── Button.types.ts
│   │   │   │   └── index.ts
│   │   │   ├── Input/
│   │   │   ├── Modal/
│   │   │   ├── Card/
│   │   │   └── index.ts
│   │   ├── layout/            # Layout components (Header, Footer, Sidebar)
│   │   │   ├── Header/
│   │   │   ├── Footer/
│   │   │   ├── Sidebar/
│   │   │   └── Layout.tsx
│   │   └── common/            # Common components (Loading, ErrorBoundary)
│   │       ├── Loading/
│   │       ├── ErrorBoundary/
│   │       └── ProtectedRoute/
│   ├── features/              # Feature-based modules
│   │   ├── auth/              # Authentication feature
│   │   │   ├── components/    # Auth-specific components
│   │   │   ├── hooks/         # Auth-related custom hooks
│   │   │   ├── services/      # Auth API services
│   │   │   ├── store/         # Auth state management
│   │   │   ├── types/         # Auth TypeScript types
│   │   │   └── index.ts
│   │   ├── profile/           # User profile management
│   │   ├── skills/            # Skills posting & browsing
│   │   ├── matching/          # Matchmaking system
│   │   ├── messaging/         # In-app messaging
│   │   ├── swapRequests/      # Skill swap request system
│   │   ├── scheduling/        # Calendar & scheduling
│   │   ├── reviews/           # Ratings & reviews
│   │   ├── dashboard/         # User & admin dashboards
│   │   └── admin/             # Admin panel features
│   ├── pages/                 # Page components for routing
│   │   ├── HomePage.tsx
│   │   ├── LoginPage.tsx
│   │   ├── SignupPage.tsx
│   │   ├── ProfilePage.tsx
│   │   ├── SkillsPage.tsx
│   │   ├── DashboardPage.tsx
│   │   ├── MessagingPage.tsx
│   │   ├── SwapRequestsPage.tsx
│   │   ├── SchedulingPage.tsx
│   │   ├── ReviewsPage.tsx
│   │   ├── AdminPage.tsx
│   │   └── NotFoundPage.tsx
│   ├── hooks/                 # Global custom hooks
│   │   ├── useLocalStorage.ts
│   │   ├── useDebounce.ts
│   │   ├── useApi.ts
│   │   └── index.ts
│   ├── services/              # API services
│   │   ├── api/
│   │   │   ├── client.ts      # Axios instance configuration
│   │   │   ├── endpoints.ts   # API endpoints
│   │   │   └── index.ts
│   │   ├── auth.service.ts
│   │   ├── user.service.ts
│   │   ├── skills.service.ts
│   │   └── index.ts
│   ├── store/                 # Redux store configuration
│   │   ├── index.ts
│   │   ├── rootReducer.ts
│   │   └── middleware.ts
│   ├── types/                 # Global TypeScript types
│   │   ├── api.types.ts
│   │   ├── common.types.ts
│   │   ├── user.types.ts
│   │   └── index.ts
│   ├── utils/                 # Utility functions
│   │   ├── constants.ts
│   │   ├── helpers.ts
│   │   ├── validation.ts
│   │   ├── formatters.ts
│   │   └── index.ts
│   ├── styles/                # Global styles
│   │   ├── globals.css
│   │   ├── components.css
│   │   └── utilities.css
│   ├── assets/                # Static assets
│   │   ├── images/
│   │   ├── icons/
│   │   └── fonts/
│   ├── config/                # Configuration files
│   │   ├── env.ts
│   │   ├── routes.ts
│   │   └── constants.ts
│   ├── App.tsx
│   ├── App.css
│   ├── index.tsx
│   ├── index.css
│   └── react-app-env.d.ts
├── package.json
├── tsconfig.json
├── tailwind.config.js
├── postcss.config.js
└── README.md
```

---

## ✨ Core Features

### 🔐 1. User Profile Management
- Secure registration and login system
- Comprehensive profiles with skills offered and requested
- Profile customization with bio and profile picture

### 🎯 2. Skill Posting & Browsing
- Post skill listings with detailed descriptions
- Browse and search skills with advanced filters
- Category-based skill organization

### 🤝 3. AI-Powered Matchmaking System
- Intelligent matching based on complementary skills
- Automated suggestions for potential skill swaps
- Match compatibility scoring

### 📨 4. Skill Swap Request System
- Send and receive skill exchange proposals
- Request management with acceptance/decline options
- Trade status tracking

### 📅 5. Scheduling & Calendar Integration
- Built-in session scheduler
- Google Calendar integration
- Time slot management for learning sessions

### ⭐ 6. Ratings & Reviews System
- Post-session feedback and ratings
- Community trust building through reviews
- Reputation-based matching improvements

### 💬 7. In-App Messaging System
- Secure chat functionality between matched users
- Real-time communication for coordination
- Message history and notifications

### 🏆 8. Gamification & Achievements
- Earn badges for active participation
- Achievement system to encourage engagement
- Reputation levels and progress tracking

### 🏷️ 9. Advanced Skill Categories & Tagging
- Structured skill categorization
- Tag-based skill discovery
- Custom skill tags for better matching

### 👤 10. Comprehensive Dashboards
- **User Dashboard:** Personal activity overview
- **Admin Dashboard:** Platform management and monitoring

---

## 🛠️ Technology Stack

### Frontend
- **React.js** - UI library
- **TypeScript** - Type safety and better developer experience
- **Tailwind CSS** - Utility-first CSS framework
- **React Router** - Client-side routing
- **Redux Toolkit** - State management
- **React Hook Form** - Form handling
- **Axios** - HTTP client

### Development Tools
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **Husky** - Git hooks
- **Jest** - Testing framework

---

## 📋 Project Requirements

### Functional Requirements

#### 1. User Management
- **User Registration & Login:** Secure account creation and login with email and password
- **User Profile:** Profiles displaying username, bio, profile picture, "Skills I Can Teach," and "Skills I Want to Learn"

#### 2. Skill Management
- **Add/Edit Skills:** Users can add, edit, and remove skills from their profile
- **Skill Details:** Each skill includes name, category, description, and proficiency level

#### 3. Marketplace & Search
- **Browse & Search:** Central marketplace to browse and search for skills
- **Filtering:** Filter skills by category and proficiency level

#### 4. Trading System
- **Propose Trade:** Users can propose trades by offering their skills
- **Manage Proposals:** Accept or decline trade proposals
- **Trade Status:** View status of all trades (Pending, Accepted, Declined)

#### 5. Communication
- **Private Messaging:** Private messaging channels between users after trade acceptance

#### 6. Reputation System
- **Ratings & Reviews:** Rate and review users after completed skill swaps
- **Public Feedback:** Reviews visible on user profiles for community trust

### Non-Functional Requirements
- **Usability:** Intuitive, clean, and mobile-friendly interface
- **Performance:** Fast and responsive application
- **Security:** Protected user data with HTTPS and hashed passwords
- **Scalability:** Architecture supporting growing user base

---

## 👥 Team Structure & Development Workflow

### Team Roles (6 Members)
- **Member 1 (Lead Frontend & User Onboarding):** UI/UX for registration, login, and profile pages
- **Member 2 (Backend Lead & User Authentication):** Core backend, database schema, and authentication APIs
- **Member 3 (Frontend - Marketplace):** Marketplace, search, and filtering UI
- **Member 4 (Backend - Skill & Marketplace Logic):** Backend APIs for skill creation, management, and search
- **Member 5 (Full-Stack - Trading System):** End-to-end trade proposal and management system
- **Member 6 (Full-Stack - Communication & Reputation):** Private messaging and user rating systems

---

## 🚦 Development Guidelines

### Code Quality Standards
- **TypeScript:** Use strict type checking for all components
- **Component Structure:** Follow the established folder structure for consistency
- **Naming Conventions:** Use PascalCase for components, camelCase for functions and variables
- **CSS Classes:** Use Tailwind utility classes, create custom components when needed

### Git Workflow
- **Branching:** Create feature branches from `main` (`feature/component-name`)
- **Commits:** Use conventional commit messages (`feat:`, `fix:`, `docs:`, etc.)
- **Pull Requests:** Require code review before merging
- **Testing:** Ensure all tests pass before merging

### File Organization
- **Components:** Each component should have its own folder with `.tsx`, `.types.ts`, and `index.ts` files
- **Imports:** Use absolute imports with proper index files
- **Types:** Define TypeScript interfaces in separate `.types.ts` files
- **Styles:** Use Tailwind classes, create utility classes in global CSS when needed

---

## 📱 Responsive Design

The application is built with a mobile-first approach using Tailwind CSS responsive utilities:
- **Mobile:** 320px - 768px
- **Tablet:** 768px - 1024px  
- **Desktop:** 1024px and above

---

## 🔒 Security Considerations

- **Authentication:** JWT-based authentication with secure token storage
- **Data Protection:** Input validation and sanitization
- **HTTPS:** All communications encrypted
- **Privacy:** User data protection and privacy controls

---

## 🚀 Deployment

### Build for Production
```bash
npm run build
# or
yarn build
```

### Environment Variables
Create a `.env` file in the root directory:
```
REACT_APP_API_URL=your_api_url
REACT_APP_ENVIRONMENT=production
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and development process.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

## 📞 Support

If you have any questions or need help with the project:
- Create an issue in the repository
- Contact the development team
- Check the documentation in the `/docs` folder

---

**Happy Coding! 🚀**

*Built with ❤️ by the SkillShare Hub Team*