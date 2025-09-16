SkillShareHub/
├── README.md
├── .env.local
├── .env.example
├── .gitignore
├── next.config.js
├── tailwind.config.js
├── tsconfig.json
├── package.json
├── yarn.lock / package-lock.json
├── middleware.ts
│
├── public/
│   ├── images/
│   ├── icons/
│   ├── favicon.ico
│   └── manifest.json
│
├── src/
│   ├── app/
│   │   ├── globals.css
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── loading.tsx
│   │   ├── error.tsx
│   │   ├── not-found.tsx
│   │   │
│   │   ├── (auth)/
│   │   │   ├── login/
│   │   │   │   └── page.tsx
│   │   │   ├── register/
│   │   │   │   └── page.tsx
│   │   │   └── layout.tsx
│   │   │
│   │   ├── dashboard/
│   │   │   ├── page.tsx
│   │   │   ├── profile/
│   │   │   │   └── page.tsx
│   │   │   ├── skills/
│   │   │   │   ├── page.tsx
│   │   │   │   ├── add/
│   │   │   │   │   └── page.tsx
│   │   │   │   └── [id]/
│   │   │   │       └── page.tsx
│   │   │   ├── swaps/
│   │   │   │   ├── page.tsx
│   │   │   │   ├── requests/
│   │   │   │   │   └── page.tsx
│   │   │   │   └── [id]/
│   │   │   │       └── page.tsx
│   │   │   ├── messages/
│   │   │   │   ├── page.tsx
│   │   │   │   └── [conversationId]/
│   │   │   │       └── page.tsx
│   │   │   └── layout.tsx
│   │   │
│   │   ├── explore/
│   │   │   ├── page.tsx
│   │   │   ├── skills/
│   │   │   │   ├── page.tsx
│   │   │   │   └── [category]/
│   │   │   │       └── page.tsx
│   │   │   └── users/
│   │   │       ├── page.tsx
│   │   │       └── [id]/
│   │   │           └── page.tsx
│   │   │
│   │   ├── admin/
│   │   │   ├── page.tsx
│   │   │   ├── users/
│   │   │   │   └── page.tsx
│   │   │   ├── skills/
│   │   │   │   └── page.tsx
│   │   │   ├── reports/
│   │   │   │   └── page.tsx
│   │   │   └── layout.tsx
│   │   │
│   │   └── api/
│   │       ├── auth/
│   │       │   ├── login/
│   │       │   │   └── route.ts
│   │       │   ├── register/
│   │       │   │   └── route.ts
│   │       │   ├── logout/
│   │       │   │   └── route.ts
│   │       │   └── verify/
│   │       │       └── route.ts
│   │       │
│   │       ├── users/
│   │       │   ├── route.ts
│   │       │   ├── [id]/
│   │       │   │   └── route.ts
│   │       │   ├── profile/
│   │       │   │   └── route.ts
│   │       │   └── search/
│   │       │       └── route.ts
│   │       │
│   │       ├── skills/
│   │       │   ├── route.ts
│   │       │   ├── [id]/
│   │       │   │   └── route.ts
│   │       │   ├── categories/
│   │       │   │   └── route.ts
│   │       │   └── search/
│   │       │       └── route.ts
│   │       │
│   │       ├── swaps/
│   │       │   ├── route.ts
│   │       │   ├── [id]/
│   │       │   │   └── route.ts
│   │       │   ├── requests/
│   │       │   │   └── route.ts
│   │       │   └── matches/
│   │       │       └── route.ts
│   │       │
│   │       ├── messages/
│   │       │   ├── route.ts
│   │       │   ├── [conversationId]/
│   │       │   │   └── route.ts
│   │       │   └── conversations/
│   │       │       └── route.ts
│   │       │
│   │       ├── reviews/
│   │       │   ├── route.ts
│   │       │   └── [id]/
│   │       │       └── route.ts
│   │       │
│   │       ├── calendar/
│   │       │   ├── route.ts
│   │       │   ├── events/
│   │       │   │   └── route.ts
│   │       │   └── availability/
│   │       │       └── route.ts
│   │       │
│   │       └── admin/
│   │           ├── users/
│   │           │   └── route.ts
│   │           ├── skills/
│   │           │   └── route.ts
│   │           └── reports/
│   │               └── route.ts
│   │
│   ├── components/
│   │   ├── ui/
│   │   │   ├── Button.tsx
│   │   │   ├── Input.tsx
│   │   │   ├── Modal.tsx
│   │   │   ├── Card.tsx
│   │   │   ├── Badge.tsx
│   │   │   ├── Avatar.tsx
│   │   │   ├── Dropdown.tsx
│   │   │   ├── Tabs.tsx
│   │   │   ├── Toast.tsx
│   │   │   ├── Loader.tsx
│   │   │   └── index.ts
│   │   │
│   │   ├── layout/
│   │   │   ├── Header.tsx
│   │   │   ├── Footer.tsx
│   │   │   ├── Sidebar.tsx
│   │   │   ├── Navigation.tsx
│   │   │   └── MobileMenu.tsx
│   │   │
│   │   ├── auth/
│   │   │   ├── LoginForm.tsx
│   │   │   ├── RegisterForm.tsx
│   │   │   ├── ForgotPasswordForm.tsx
│   │   │   └── ProtectedRoute.tsx
│   │   │
│   │   ├── profile/
│   │   │   ├── ProfileCard.tsx
│   │   │   ├── ProfileForm.tsx
│   │   │   ├── SkillsList.tsx
│   │   │   ├── BadgesList.tsx
│   │   │   └── ProfileStats.tsx
│   │   │
│   │   ├── skills/
│   │   │   ├── SkillCard.tsx
│   │   │   ├── SkillForm.tsx
│   │   │   ├── SkillSearch.tsx
│   │   │   ├── SkillFilters.tsx
│   │   │   ├── CategoryList.tsx
│   │   │   └── SkillGrid.tsx
│   │   │
│   │   ├── swaps/
│   │   │   ├── SwapCard.tsx
│   │   │   ├── SwapRequestForm.tsx
│   │   │   ├── SwapsList.tsx
│   │   │   ├── MatchSuggestions.tsx
│   │   │   └── SwapDetails.tsx
│   │   │
│   │   ├── messaging/
│   │   │   ├── ChatWindow.tsx
│   │   │   ├── MessageList.tsx
│   │   │   ├── MessageInput.tsx
│   │   │   ├── ConversationList.tsx
│   │   │   └── MessageBubble.tsx
│   │   │
│   │   ├── calendar/
│   │   │   ├── Calendar.tsx
│   │   │   ├── EventForm.tsx
│   │   │   ├── EventCard.tsx
│   │   │   ├── TimeSlotPicker.tsx
│   │   │   └── AvailabilityForm.tsx
│   │   │
│   │   ├── reviews/
│   │   │   ├── ReviewCard.tsx
│   │   │   ├── ReviewForm.tsx
│   │   │   ├── RatingStars.tsx
│   │   │   └── ReviewsList.tsx
│   │   │
│   │   ├── search/
│   │   │   ├── SearchBar.tsx
│   │   │   ├── SearchResults.tsx
│   │   │   ├── SearchFilters.tsx
│   │   │   └── SearchSuggestions.tsx
│   │   │
│   │   └── admin/
│   │       ├── UserManagement.tsx
│   │       ├── SkillModeration.tsx
│   │       ├── ReportsPanel.tsx
│   │       └── Analytics.tsx
│   │
│   ├── lib/
│   │   ├── db/
│   │   │   ├── mongodb.ts
│   │   │   ├── models/
│   │   │   │   ├── User.ts
│   │   │   │   ├── Skill.ts
│   │   │   │   ├── Swap.ts
│   │   │   │   ├── Message.ts
│   │   │   │   ├── Review.ts
│   │   │   │   ├── Calendar.ts
│   │   │   │   └── index.ts
│   │   │   └── seeders/
│   │   │       ├── users.ts
│   │   │       ├── skills.ts
│   │   │       └── categories.ts
│   │   │
│   │   ├── auth/
│   │   │   ├── jwt.ts
│   │   │   ├── bcrypt.ts
│   │   │   ├── middleware.ts
│   │   │   └── config.ts
│   │   │
│   │   ├── validations/
│   │   │   ├── auth.ts
│   │   │   ├── user.ts
│   │   │   ├── skill.ts
│   │   │   ├── swap.ts
│   │   │   └── message.ts
│   │   │
│   │   ├── utils/
│   │   │   ├── api.ts
│   │   │   ├── constants.ts
│   │   │   ├── helpers.ts
│   │   │   ├── formatters.ts
│   │   │   ├── email.ts
│   │   │   ├── upload.ts
│   │   │   └── matchmaking.ts
│   │   │
│   │   └── providers/
│   │       ├── AuthProvider.tsx
│   │       ├── ThemeProvider.tsx
│   │       ├── QueryProvider.tsx
│   │       └── ToastProvider.tsx
│   │
│   ├── hooks/
│   │   ├── useAuth.ts
│   │   ├── useApi.ts
│   │   ├── useLocalStorage.ts
│   │   ├── useDebounce.ts
│   │   ├── useSocket.ts
│   │   ├── useInfiniteScroll.ts
│   │   ├── useSkills.ts
│   │   ├── useSwaps.ts
│   │   ├── useMessages.ts
│   │   ├── useCalendar.ts
│   │   └── useSearch.ts
│   │
│   ├── types/
│   │   ├── auth.ts
│   │   ├── user.ts
│   │   ├── skill.ts
│   │   ├── swap.ts
│   │   ├── message.ts
│   │   ├── review.ts
│   │   ├── calendar.ts
│   │   ├── api.ts
│   │   └── index.ts
│   │
│   ├── styles/
│   │   ├── globals.css
│   │   ├── components.css
│   │   └── utilities.css
│   │
│   └── config/
│       ├── database.ts
│       ├── env.ts
│       ├── constants.ts
│       └── features.ts
│
├── docs/
│   ├── API.md
│   ├── SETUP.md
│   ├── CONTRIBUTING.md
│   └── DEPLOYMENT.md
│
├── tests/
│   ├── __mocks__/
│   ├── components/
│   ├── api/
│   ├── utils/
│   ├── setup.ts
│   └── jest.config.js
│
└── scripts/
    ├── build.sh
    ├── deploy.sh
    ├── seed-db.ts
    └── migration.ts