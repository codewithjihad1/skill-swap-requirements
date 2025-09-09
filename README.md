# Skill Swap Marketplace

**Description:** A platform where users can trade skills (e.g., "I’ll teach you coding if you teach me guitar") instead of paying money.

This document outlines the project requirements and the plan for dividing the work among a team of six.

---

## Project Requirements

### Functional Requirements

#### 1. User Management
-   **User Registration & Login:** Secure account creation and login with email and password.
-   **User Profile:** Profiles must display a username, bio, profile picture, a list of "Skills I Can Teach," and a list of "Skills I Want to Learn."

#### 2. Skill Management
-   **Add/Edit Skills:** Users can add, edit, and remove skills from their profile.
-   **Skill Details:** Each skill includes a name, category, description, and proficiency level.

#### 3. Marketplace & Search
-   **Browse & Search:** A central marketplace to browse and search for skills.
-   **Filtering:** Filter skills by category and proficiency level.

#### 4. Trading System
-   **Propose Trade:** Users can propose a trade by offering one of their skills.
-   **Manage Proposals:** Users can accept or decline trade proposals.
-   **Trade Status:** View the status of all trades (Pending, Accepted, Declined).

#### 5. Communication
-   **Private Messaging:** A private messaging channel is created between users once a trade is accepted.

#### 6. Reputation System
-   **Ratings & Reviews:** Users can rate and review each other after a completed skill swap.
-   **Public Feedback:** Reviews are visible on user profiles to build community trust.

### Non-Functional Requirements

-   **Usability:** The interface must be intuitive, clean, and mobile-friendly.
-   **Performance:** The application must be fast and responsive.
-   **Security:** User data must be protected, with encrypted communication (HTTPS) and hashed passwords.
-   **Scalability:** The architecture should support a growing user base.

---

## Team Roles & Responsibilities

-   **Member 1 (Lead Frontend & User Onboarding):** Focus on UI/UX for registration, login, and profile pages.
-   **Member 2 (Backend Lead & User Authentication):** Build the core backend, database schema for users, and authentication APIs.
-   **Member 3 (Frontend - Marketplace):** Develop the marketplace, search, and filtering UI.
-   **Member 4 (Backend - Skill & Marketplace Logic):** Implement the backend APIs for creating, managing, and searching for skills.
-   **Member 5 (Full-Stack - Trading System):** Handle the end-to-end trade proposal and management system (frontend and backend).
-   **Member 6 (Full-Stack - Communication & Reputation):** Build the private messaging and user rating systems (frontend and backend).
