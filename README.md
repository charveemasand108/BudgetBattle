# 💸 BudgetBattle

> **Turn saving money into a competition you actually want to win.**

BudgetBattle is an iOS app that gamifies personal finance. Track your expenses, take on spending challenges, and battle your bad habits — all with a clean, native SwiftUI interface.

---

## 🎯 Concept

Most budgeting apps make you feel guilty. BudgetBattle makes you feel like a winner. Set spending limits, take on daily and weekly challenges, and watch your financial health bar rise as you beat your own records.

---

## ✨ Features

- 💰 **Expense Tracking** — log and categorise your spending on the go
- 🏆 **Budget Challenges** — take on preset or custom challenges (no coffee for a week, eat in every day, etc.)
- 📊 **Dashboard** — visual overview of your budget health, spending trends, and active battles
- 🎨 **Theme Manager** — personalise the app's look and feel
- 🃏 **Challenge Cards** — swipeable cards for discovering and starting new budget challenges

---
<p>
  <img src="https://github.com/charveemasand108/BudgetBattle/blob/47885f8b43b7f6d515c9535311ef15b8d2b606d2/simulator_screenshot_759F8404-2AF3-4CE9-9EFB-51A13051E8BA.png?raw=true" width="220" />
  &nbsp;&nbsp;&nbsp;
  <img src="https://github.com/charveemasand108/BudgetBattle/blob/47885f8b43b7f6d515c9535311ef15b8d2b606d2/simulator_screenshot_70ADE0B9-8C83-4057-A175-A0A036723380.png?raw=true" width="220" />
  &nbsp;&nbsp;&nbsp;
  <img src="https://github.com/charveemasand108/BudgetBattle/blob/47885f8b43b7f6d515c9535311ef15b8d2b606d2/simulator_screenshot_81535E6F-7BAE-4984-B692-AEEABD0A75DE.png?raw=true" width="220" />
  &nbsp;&nbsp;&nbsp;
  <img src="https://github.com/charveemasand108/BudgetBattle/blob/47885f8b43b7f6d515c9535311ef15b8d2b606d2/simulator_screenshot_9B69A167-87BE-4996-813D-CC9D67484B8B.png?raw=true" width="220" />
</p>

## 🏗️ Architecture

~~~
BudgetBattleApp
    └── ContentView
            ├── Dashboard         → spending overview & budget health
            ├── ChallengeView     → browse & join budget challenges
            │     └── ChallengeCard
            ├── AddExpense        → log a new expense
            └── ThemeManager      → app-wide theming
~~~

**Pattern:** MVVM — `ViewModel.swift` drives all state, `Model.swift` defines the data layer, views stay purely declarative.

---

## 📂 File Structure

~~~
BudgetBattle/
├── BudgetBattleApp.swift    # App entry point (@main)
├── ContentView.swift        # Root screen / tab router
├── Model.swift              # Data models: Expense, Challenge, Budget
├── ViewModel.swift          # Business logic & state management
├── Dashboard.swift          # Home screen with spending overview
├── ChallengeView.swift      # Challenge browser
├── ChallengeCard.swift      # Reusable challenge card component
├── AddExpense.swift         # Add / edit expense sheet
├── ThemeManager.swift       # App-wide colour & theme system
└── Assets.xcassets/         # App icon, colours, assets
~~~

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| UI | SwiftUI |
| State | ObservableObject + @StateObject |
| Data | Swift structs + local persistence |
| Min iOS | iOS 16.0+ |
| Language | Swift 5.9 |

---

## 🗺️ Roadmap

- [ ] **Expense logging** — full AddExpense flow with categories & amounts
- [ ] **Dashboard charts** — spending breakdown with SwiftUI Charts
- [ ] **Challenge engine** — auto-track progress against active challenges
- [ ] **Streaks & badges** — reward consistent saving behaviour
- [ ] **Multiplayer battles** — challenge friends to who can save more in a week
- [ ] **Notifications** — daily nudges when approaching budget limits
- [ ] **iCloud sync** — expenses and progress across devices

---

## 💡 Concept

BudgetBattle was built on the idea that **the psychology of games — streaks, challenges, winning — works better than spreadsheets.** If you can make saving money feel like levelling up, people will actually do it.

---

## 👩‍💻 Author

**Charvee Masand** — [@charveemasand108](https://github.com/charveemasand108)

---

## 📄 License

MIT License — free to use, just don't blow your budget.
