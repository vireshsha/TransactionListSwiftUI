## Overview
iOS app that displays a list of transactions with detailed views.  
Built using **SwiftUI** and **MVVM** for clean architecture and scalability.

## Environment
- **Xcode:** 26.3  
- **Swift:** 5  
- **Minimum Deployment Target:** iOS 16.2  
- **Architecture:** MVVM

## Features
- **Programmatic UI:** Views like `TransactionList`, `TransactionRowView`, `TransactionDetailView` are fully built programmatically.  
- **Navigation:** Type-safe navigation using `NavigationStack` and `.navigationDestination`.  
- **Accessibility:** Identifiers added for UI testing:  
  - `transactionList` for the transaction list  
  - `transactionCell_<id>` for each transaction cell  
- **Data Handling:** Loads transactions from `transaction-list.json` in the main bundle.  
- **Formatting:** Amounts formatted according to locale (CAD) with proper currency display.

---

## Testing
- **Unit Tests:**  
  - JSON decoding and parsing  
  - Computed properties (`shortCardSuffix`, `fromDisplayText`)  
  - Formatted amounts  
- **UI Tests:**  
  - Verify transaction list visibility  
  - Check cells exist and are tappable  
  - Open transaction details  
  - Scroll performance  

---

## How to Run
1. Open the project in Xcode 15+  
2. Run the **App** through the target (`TakeHomeAssignment`)  
3. Run **Unit Tests**: `Product > Test` or `Cmd+U`  
4. Run **UI Tests**: `Product > Test` or `Cmd+U` (ensure simulator has access to `transaction-list.json` in main bundle)  

---

## Notes
- UI is fully functional and ready for review.  
- Designed with scalability and maintainability in mind.  
- Accessibility identifiers added to support automated UI testing.
