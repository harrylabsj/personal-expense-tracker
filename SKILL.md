---
name: expense-tracker
description: Personal expense tracker - record expenses, auto-categorize, monthly statistics with total and category breakdown
version: v1.0.0
tags: expense-tracking, personal-finance, budget-management, auto-categorization
---

# Expense Tracker

Simple personal expense tracking assistant.

## Usage Scenarios

### Scenario 1: Record a Daily Expense
**User input:** "记录早餐花了10元。"

**Expected output:** Entry saved successfully - 早餐 | ¥10.00 | food | 2026-06-19 09:54. Category auto-detected as food. Running today total shown.

### Scenario 2: Get Monthly Statistics
**User input:** "这个月花了多少钱？"

**Expected output:** Monthly statistics: total ¥3,250.50, breakdown by category - food ¥1,200 (37%), transport ¥450 (14%), shopping ¥800 (25%), others ¥800.50 (24%). Average daily spend ¥108.35.

### Scenario 3: Check Category Breakdown
**User input:** "查看本周食品类支出了多少。"

**Expected output:** Food category breakdown this week: Mon ¥35, Tue ¥42.50, Wed ¥28, Thu ¥55, Fri ¥30, Sat ¥0, Sun ¥0. Weekly food total ¥190.50.

## Features
- Record expense with amount and note
- Auto-categorize (food/transport/shopping/others)
- Monthly statistics (total + category breakdown)

## Constraints
- ❌ No budget alerts
- ❌ No bank payment integration
- ❌ No cross-device sync

## Usage
```bash
python3 scripts/expense-tracker.py add "早餐" 10
python3 scripts/expense-tracker.py stats
```
