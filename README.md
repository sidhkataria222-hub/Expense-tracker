# SpendWise AI — Personalized Financial Intelligence

**SpendWise AI** is an institutional-grade personal finance platform unified on a single engine, dynamically personalizing experiences for two primary audiences:
1. **College Students**
2. **Working Professionals**

---

## 🌟 Architecture & Core Personalization

### A. Dynamic User Onboarding
- **Mandatory Persona Selection Screen**:
  - Heading: *"Let's personalize your financial experience."*
  - Question: *"Which best describes you?"* (Options: College Student, Working Professional, Other).
  - Main dashboard is locked until initial personalization is completed.
- **Dynamic Persona-Specific Questionnaire**:
  - **Student**: College name (opt), Course/degree (opt), Academic year, Accommodation type (*Hostel / PG / Home / Rented*), Primary money source (*Pocket money / Family support / Scholarship / Part-time / Multiple*), Monthly allowance (opt), Currency, Primary savings goal (opt).
  - **Professional**: Employment type (*Full-time / Part-time / Freelance / Self-employed*), Company name (opt), Income frequency (*Monthly / Weekly / Irregular*), Primary income source, Monthly income (opt), Currency, Primary financial goals (opt).
  - **Other**: Customizable categories and financial objectives.
- Sensitive financial data disclosure is never forced.

### B. College Student Dashboard (`user_type = STUDENT`)
- **Key Metrics**: Total pocket money received, Total expenses this month, Remaining allowance, Daily average spending, Monthly savings, and category breakdowns.
- **8 Dedicated Student Widgets**:
  1. *Pocket Money Tracker* (Real-time visual allowance consumption)
  2. *Monthly Allowance Planner* (Campus allocation breakdown)
  3. *Remaining Days and Remaining Budget Tracker*
  4. *Daily Spending Limit Calculator* (Remaining budget ÷ Remaining days dynamic pacing)
  5. *Hostel Expense Tracker* (Room rent, mess bills, laundry, leave rebate tips)
  6. *Split Expenses With Friends* (Split shared cafe/hostel bills, track who owes whom, 1-click settlement)
  7. *College Trip Expense Manager* (Budget vacation/hackathon itineraries, track itemized expenses)
  8. *Student Savings Goals* (Pocket money milestones with celebratory confetti upon completion)

### C. Working Professional Dashboard (`user_type = PROFESSIONAL`)
- **Key Metrics**: Monthly income, Total expenses, Available balance, Monthly savings, Savings rate (%), Rent, EMIs, Utility bills, Groceries, Transportation, Investments, and Upcoming recurring payments.
- **8 Dedicated Professional Widgets**:
  1. *Salary Tracker* (Net take-home reconciliation)
  2. *Monthly Cash Flow Waterfall* (Fixed vs Variable vs Investments vs Retained)
  3. *EMI and Loan Tracker* (Tenures, monthly installment dues, interest rate drag)
  4. *Bill Management* (Electricity, broadband, credit cards with 1-click paid status toggles)
  5. *Recurring Subscription Tracker* (Software SaaS, streaming, gym with annual projections)
  6. *Emergency Fund Safety Runway* (Configurable 3/6/9/12 month living cost runway)
  7. *Monthly Savings Planner* (50/30/20 Rule: Needs vs Wants vs Savings)
  8. *Annual Expense Analysis* (Year-to-date monthly trajectory and top spending drivers)

---

## 🚀 Advanced Premium Features

### 1. No-Spend Challenge (`/api/challenges`)
- Create **7-day, 15-day, or 30-day** conscious spending challenges.
- Select target categories to avoid (takeout, shopping, entertainment, etc.).
- Real-time streak tracking and money saved calculations.
- **Essential Spending Protection Guard**: Essential items (healthcare, medicines, hospital bills, college tuition, hostel rent) are automatically protected and never fail challenges.

### 2. Smart Group Expense Manager (`/api/groups`)
- Create groups for roommates, friends, colleagues, or trip squads.
- Add shared expenses with **Equal**, **Custom Amount**, or **Percentage** splits.
- Individual net balance calculations.
- **Simplified Debt Settlement Algorithm**: Minimizes multi-party transactions and calculates exactly who owes whom.
- 1-click settlement recording and itemized group expense history.
- Enforced group membership authorization.

### 3. Financial Calendar (`/api/calendar`)
- Unified chronological timeline of upcoming bills, subscriptions, rent, EMIs, and scheduled salary/allowance inflows.
- Custom reminders with due dates and amounts.
- Monthly commitment KPI metrics (Total committed, Paid, Due).
- 1-click completion toggles.

### 4. What-If Financial Simulator (`/api/simulator`)
- Interactive percentage cutback sliders per category.
- Calculates projected monthly, 1-year, 3-year, and 5-year compound invested wealth potential.
- Compares baseline vs simulated budget.
- Clearly labeled with required regulatory estimate disclaimers.

### 5. Financial Fitness Score (`/api/fitness-score`)
- Explainable 0–100 wellness index derived from 4 transparent pillars:
  - Budget Discipline (30% weight)
  - Savings Consistency (30% weight)
  - Debt & Leverage Exposure (20% weight)
  - Resilience Buffer & Goals (20% weight)
- Actionable steps for resilience enhancement.
- Prominent statutory notice clarifying it is NOT a credit bureau score or formal credit assessment.

### 6. Student Deals and Savings Hub (`/api/deals`)
- Curated directory of verified educational discounts: GitHub Student Developer Pack, Spotify Student, Apple Education, Notion, Amazon Prime Student, Canva for Education, Adobe Creative Cloud, and JetBrains.
- Category filtering (*Tech & Dev, Streaming & Music, Productivity & Study, Lifestyle & Retail*).
- Clear eligibility and validity guidelines. Direct verified official links.

### 7. Personalized Spending Comparison (`/api/comparison`)
- Historical month-over-month category shift analysis.
- Flags significant surges or decreases (>10%).
- Evidence-based explanations backed by actual transaction records.
- 100% private: scoped exclusively to user's authenticated ledger.

### 8. Achievement & Gamification System (`/api/gamification`)
- Milestone badges for savings consistency, no-spend challenge completions, goal milestones, and cash flow surpluses.
- 1-click automated ledger evaluation.
- Promotes financial wellness while strictly discouraging unhealthy spending deprivation.

---

## 🧪 Testing & Quick Start

```powershell
# Run the 11-suite integration test
npm test

# Start Dev Mode (Backend on 5000 + Vite Frontend on 5173)
npm run dev

# Production Build and Run
npm run build
npm start
```

### Instant Demo Credentials

| Persona | Email | Password | Pre-seeded Features |
|---|---|---|---|
| **College Student** | `student@spendwise.ai` | `password123` | Pocket money, canteen food, hostel split, Manali trip manager, 15-day fast food challenge, Roommates Smart Group |
| **Working Professional** | `pro@spendwise.ai` | `password123` | Salary credit, apartment rent, car EMI, bills, 30-day shopping challenge, Flatmates Smart Group, emergency runway |
