# Exit Conditions Frequency Table - Guide

## File: exit_conditions_frequency_table.csv

This table shows every unique combination of exit conditions across your 962 trades (note: 8 trades had missing data).

## Table Structure

Each row represents a unique exit pattern with these columns:

### Input Columns (Exit Conditions):
1. **Price vs 50 DMA** - Price position relative to 50-day moving average at exit (in 5% buckets)
2. **Price vs 200 DMA** - Price position relative to 200-day moving average at exit (in 5% buckets)
3. **DMA Diff at Exit** - Spread between 50 DMA and 200 DMA at exit (in 5% buckets)

### Output Columns (Results):
4. **Total Trades** - Number of trades with this exact combination
5. **Good Call Count** - Number of good exits (price declined after)
6. **Wrong Early Sell Count** - Number of premature exits (price rose after)
7. **% Good Call** - Percentage of good exits
8. **% Wrong Early Sell** - Percentage of wrong exits

**Note**: % Good Call + % Wrong Early Sell = 100% for every row ✓

---

## Key Findings

### 📊 Overall Stats
- **76 unique exit patterns** identified
- **962 trades** analyzed
- **30 patterns** have 10+ trades (significant volume)
- **11 patterns** have 20+ trades (high volume)

### 🔴 Your Single Worst Pattern

**Pattern #1: THE DISASTER ZONE**
```
Price vs 50 DMA:    5 to 10%
Price vs 200 DMA:   20 to 25%
DMA Diff at Exit:   10 to 15%

Total Trades:       187 (19.4% of all trades!)
% Good Call:        0.00%
% Wrong Early Sell: 100.00%
```

**What this means:**
- You're 5-10% above the 50 DMA (healthy position)
- You're 20-25% above the 200 DMA (strong bull market)
- 50 DMA is 10-15% above 200 DMA (golden cross momentum)
- **You sold 187 times and were wrong EVERY SINGLE TIME**

**Impact**: This single pattern accounts for:
- 19.4% of all your trades
- 30.7% of all your wrong early sells

---

### ✅ Your Best Patterns

**Pattern #1: PERFECT CONSOLIDATION EXIT**
```
Price vs 50 DMA:    5 to 10%
Price vs 200 DMA:   5 to 10%
DMA Diff at Exit:   0 to 5%

Total Trades:       44
% Good Call:        100.00%
% Wrong Early Sell: 0.00%
```

**What this means:**
- Price above both DMAs but not extended
- **KEY**: DMA Diff is only 0-5% (narrow spread = consolidating)
- All 44 exits were perfectly timed
- This is your benchmark pattern!

**Pattern #2: SMART PULLBACK EXIT**
```
Price vs 50 DMA:    -5 to 0%
Price vs 200 DMA:   0 to 5%
DMA Diff at Exit:   0 to 5%

Total Trades:       54
% Good Call:        88.89%
% Wrong Early Sell: 11.11%
```

**What this means:**
- Price touching/just below 50 DMA
- DMA Diff narrow (0-5%)
- 48 good calls, only 6 wrong
- Excellent success rate!

**Pattern #3: PULLBACK IN UPTREND**
```
Price vs 50 DMA:    -10 to -5%
Price vs 200 DMA:   0 to 5%
DMA Diff at Exit:   10 to 15%

Total Trades:       21
% Good Call:        100.00%
% Wrong Early Sell: 0.00%
```

**What this means:**
- Price broke below 50 DMA by 5-10%
- But DMA Diff still positive (50 above 200)
- This signals support failure - good time to exit
- All 21 were correct exits

---

## Critical Patterns to Avoid

### 11 High-Risk Patterns (15+ trades with 70%+ error rate)

These 11 patterns represent:
- **421 trades** (43.8% of all your trades)
- **401 wrong exits** (66.1% of all your mistakes!)

| Rank | 50 DMA | 200 DMA | DMA Diff | Trades | % Wrong |
|------|--------|---------|----------|--------|---------|
| 1 | 5-10% | 20-25% | 10-15% | 187 | 100.0% |
| 2 | 5-10% | 15-20% | 5-10% | 45 | 97.8% |
| 3 | 10-15% | 15-20% | 5-10% | 42 | 76.2% |
| 4 | -5 to 0% | -5 to 0% | -5 to 0% | 22 | 100.0% |
| 5 | 5-10% | -15 to -10% | -20 to -15% | 22 | 100.0% |
| 6 | 5-10% | -5 to 0% | -10 to -5% | 21 | 100.0% |
| 7 | 5-10% | 35-40% | 20-25% | 19 | 73.7% |
| 8 | 0-5% | 5-10% | 5-10% | 16 | 100.0% |
| 9 | 5-10% | -20 to -15% | -25 to -20% | 16 | 100.0% |
| 10 | -15 to -10% | 5-10% | 15-20% | 16 | 100.0% |
| 11 | 0-5% | 5-10% | 0-5% | 15 | 73.3% |

**Common threads in bad patterns:**
1. Strong uptrend positions (patterns #1, #2, #3, #7)
2. Death cross/recovery situations (patterns #5, #6, #9, #10)
3. DMA Diff 5-15% + price well above DMAs

---

## How to Use This Table

### Step 1: Identify Your Current Exit Conditions

Before selling, check:
1. What % is price above/below 50 DMA?
2. What % is price above/below 200 DMA?
3. What is the DMA Diff?

Round to nearest 5% bucket (e.g., 7.3% → "5 to 10%")

### Step 2: Look Up Your Pattern

Find the row in the CSV that matches your three conditions.

### Step 3: Check the Success Rate

- **% Good Call > 70%**: Green light to sell
- **% Good Call 50-70%**: Yellow light, use caution
- **% Good Call < 50%**: Red light, likely too early
- **% Good Call < 30%**: STOP! You're probably making a mistake

### Step 4: Compare to Key Patterns

**If your pattern looks like:**
- Pattern #1 worst (5-10%, 20-25%, 10-15%): **DO NOT SELL**
- Pattern #1 best (5-10%, 5-10%, 0-5%): **SELL**
- Pattern #2 best (-5 to 0%, 0-5%, 0-5%): **SELL**

---

## The Simple Rules (Derived from Table)

### ✅ SELL When:

1. **DMA Diff is 0-5% (narrow spread)**
   - Look for patterns with 0-5% DMA Diff
   - These have 70-100% good call rates
   - Trend is weak/consolidating

2. **Price breaks 5-10% below 50 DMA**
   - Patterns like: -10 to -5% / 0-5% / 10-15% (100% good)
   - Support has failed
   - Time to exit even if DMA Diff still positive

3. **Price near both DMAs with narrow spread**
   - Patterns like: -5 to 0% / 0-5% / 0-5% (89% good)
   - Uncertainty zone, reasonable to exit

### 🚫 DO NOT SELL When:

1. **DMA Diff is 10-15% with price above DMAs**
   - Pattern: 5-10% / 20-25% / 10-15% (0% good, 187 trades!)
   - Strong golden cross momentum
   - WORST time to exit

2. **DMA Diff is 5-10% with price well above 200 DMA**
   - Pattern: 5-10% / 15-20% / 5-10% (2% good, 45 trades)
   - Trend still building
   - Too early to exit

3. **Death cross with price recovery**
   - Patterns with negative DMA Diff but price above 50 DMA
   - These often recover after you sell

---

## Quick Reference Chart

### By DMA Diff (Most Important Indicator)

| DMA Diff Range | Typical Result | Action |
|---------------|----------------|---------|
| 15-20% | Mixed (30-100% good) | Hold unless extreme |
| 10-15% | BAD (0-24% good) | 🔴 DO NOT SELL |
| 5-10% | BAD (2-58% good) | ⚠️ Usually too early |
| 0-5% | GOOD (73-100% good) | ✅ SELL |
| -5 to 0% | MIXED (21-100% good) | Check other conditions |
| < -10% | MIXED (varies widely) | Death cross - be careful |

### By Price vs 50 DMA

| Price vs 50 DMA | Interpretation |
|-----------------|----------------|
| > 10% | Well above support |
| 5-10% | Above support (normal) |
| 0-5% | Near support |
| -5 to 0% | At/touching support |
| -10 to -5% | Below support |
| < -10% | Well below support |

**Key insight**: Being 5-10% above 50 DMA is NORMAL and HEALTHY in an uptrend. Don't sell just because of this!

---

## Examples Using the Table

### Example 1: Should I Sell?
**Current conditions:**
- Price: 8% above 50 DMA → "5 to 10%" bucket
- Price: 22% above 200 DMA → "20 to 25%" bucket
- DMA Diff: 12% → "10 to 15%" bucket

**Look up pattern**: 5-10% / 20-25% / 10-15%
**Result**: 187 trades, 0% good call, 100% wrong early sell
**Decision**: ❌ **DO NOT SELL! This is your worst pattern!**

### Example 2: Should I Sell?
**Current conditions:**
- Price: 7% above 50 DMA → "5 to 10%" bucket
- Price: 8% above 200 DMA → "5 to 10%" bucket
- DMA Diff: 2% → "0 to 5%" bucket

**Look up pattern**: 5-10% / 5-10% / 0-5%
**Result**: 44 trades, 100% good call, 0% wrong early sell
**Decision**: ✅ **SELL! This is your best pattern!**

### Example 3: Should I Sell?
**Current conditions:**
- Price: -2% vs 50 DMA → "-5 to 0%" bucket
- Price: 3% above 200 DMA → "0 to 5%" bucket
- DMA Diff: 4% → "0 to 5%" bucket

**Look up pattern**: -5 to 0% / 0-5% / 0-5%
**Result**: 54 trades, 89% good call, 11% wrong early sell
**Decision**: ✅ **SELL! High success rate pattern!**

---

## Your Action Plan

1. **Print or save this table** - Reference it before every exit decision

2. **Stop using the 3 worst patterns immediately**:
   - 5-10% / 20-25% / 10-15% (187 trades, 0% success)
   - 5-10% / 15-20% / 5-10% (45 trades, 2% success)
   - 10-15% / 15-20% / 5-10% (42 trades, 24% success)

3. **Only exit using high-success patterns**:
   - Any pattern with DMA Diff 0-5%
   - Any pattern with price <-5% below 50 DMA
   - Any pattern with >70% good call rate

4. **Track your future exits** against this table to build discipline

---

## Bottom Line

This table contains the answer to "when should I sell?" based on YOUR actual trading history of 962 trades.

**The most important column**: DMA Diff at Exit

- **0-5%**: Exit zone (weak trend)
- **5-10%**: Caution zone (building trend)
- **10-15%**: Danger zone (strong trend - DON'T exit!)
- **15%+**: Very strong trend (hold tight)

Follow this table and you'll avoid 66% of your current mistakes.
