# Entry Conditions Frequency Table - Guide

## File: entry_conditions_frequency_table.csv

This table shows every unique combination of entry conditions across your 957 trades analyzed.

## Table Structure

Each row represents a unique entry pattern with these columns:

### Input Columns (Entry Conditions):
1. **Price vs 50 DMA** - Price position relative to 50-day moving average at entry (in 5% buckets)
2. **Price vs 200 DMA** - Price position relative to 200-day moving average at entry (in 5% buckets)
3. **DMA Diff at Entry** - Spread between 50 DMA and 200 DMA at entry (in 5% buckets)

### Output Columns (Results):
4. **Total Trades** - Number of trades with this exact combination
5. **Good Call Count** - Number of profitable entries
6. **Bad Call Count** - Number of losing entries
7. **% Good Call** - Percentage of profitable entries
8. **% Bad Call** - Percentage of losing entries

**Note**: % Good Call + % Bad Call = 100% for every row ✓

---

## Key Findings

### 📊 Overall Stats
- **99 unique entry patterns** identified
- **957 trades** analyzed
- **31 patterns** have 10+ trades (significant volume)
- **13 patterns** have 20+ trades (high volume)

### ✅ YOUR BEST ENTRY PATTERNS

**Pattern #1: EXTENDED BUT STRONG TREND**
```
Price vs 50 DMA:    25 to 30%
Price vs 200 DMA:   15 to 20%
DMA Diff at Entry:  -10 to -5%

Total Trades:       23
% Good Call:        100.00%
% Bad Call:         0.00%
```

**What this means:**
- Price extended 25-30% above 50 DMA (seems overbought!)
- But only 15-20% above 200 DMA
- **KEY**: Negative DMA Diff means 50 DMA below 200 DMA
- This is a PULLBACK in a long-term uptrend - perfect entry!
- **All 23 entries were profitable**

**Pattern #2: STRONG GOLDEN CROSS**
```
Price vs 50 DMA:    5 to 10%
Price vs 200 DMA:   20 to 25%
DMA Diff at Entry:  10 to 15%

Total Trades:       100
% Good Call:        97.00%
% Bad Call:         3.00%
```

**What this means:**
- Price moderately above 50 DMA (5-10%)
- Price well above 200 DMA (20-25%)
- Strong positive DMA Diff (10-15% = golden cross)
- **97 out of 100 entries were profitable!**
- **This is your #1 high-volume winner**

**Pattern #3: MODERATE UPTREND**
```
Price vs 50 DMA:    0 to 5%
Price vs 200 DMA:   10 to 15%
DMA Diff at Entry:  10 to 15%

Total Trades:       104
% Good Call:        87.50%
% Bad Call:         12.50%
```

**What this means:**
- Price near 50 DMA (0-5%)
- Price moderately above 200 DMA (10-15%)
- Strong DMA Diff (10-15%)
- **91 out of 104 entries were profitable**
- **Your #1 highest volume pattern**

---

### 🔴 YOUR WORST ENTRY PATTERNS

**Pattern #1: DEATH CROSS OVERBOUGHT**
```
Price vs 50 DMA:    20 to 25%
Price vs 200 DMA:   -10 to -5%
DMA Diff at Entry:  -30 to -25%

Total Trades:       18
% Good Call:        0.00%
% Bad Call:         100.00%
```

**What this means:**
- Price 20-25% above 50 DMA (extended)
- Price BELOW 200 DMA (-10 to -5%)
- Severe death cross (-30 to -25% DMA Diff)
- **All 18 entries were losers**
- You're buying into a bear market rally that fails

**Pattern #2: ANOTHER DEATH CROSS DISASTER**
```
Price vs 50 DMA:    10 to 15%
Price vs 200 DMA:   -10 to -5%
DMA Diff at Entry:  -15 to -10%

Total Trades:       17
% Good Call:        0.00%
% Bad Call:         100.00%
```

**Pattern #3: CONFUSING SETUP**
```
Price vs 50 DMA:    -10 to -5%
Price vs 200 DMA:   0 to 5%
DMA Diff at Entry:  10 to 15%

Total Trades:       15
% Good Call:        0.00%
% Bad Call:         100.00%
```

**What this means:**
- Price BELOW 50 DMA (weak)
- But above 200 DMA and positive DMA Diff (looks strong?)
- This is a confusing/choppy setup
- **All 15 entries failed**

---

## Critical Patterns Analysis

### ⚡ HIGH-RISK PATTERNS (10+ trades with 50%+ error rate)

**9 patterns represent 162 trades with 131 bad calls (42.5% of all bad entries)**

| Rank | Price vs 50 DMA | Price vs 200 DMA | DMA Diff | Trades | % Bad |
|------|-----------------|------------------|----------|--------|-------|
| 1 | 20-25% | -10 to -5% | -30 to -25% | 18 | 100.0% |
| 2 | 10-15% | -10 to -5% | -15 to -10% | 17 | 100.0% |
| 3 | 20-25% | -10 to -5% | -25 to -20% | 16 | 100.0% |
| 4 | -10 to -5% | 0-5% | 10-15% | 15 | 100.0% |
| 5 | 5-10% | 10-15% | 5-10% | 16 | 81.25% |
| 6 | 5-10% | -10 to -5% | -20 to -15% | 20 | 70.00% |
| 7 | 15-20% | -10 to -5% | -25 to -20% | 27 | 66.67% |
| 8 | 10-15% | 25-30% | 10-15% | 19 | 63.16% |
| 9 | -5 to 0% | 0-5% | 0-5% | 14 | 57.14% |

**Common threads in bad patterns:**
1. **Death cross positions** (negative DMA Diff with price below 200 DMA)
2. **Price extended above 50 DMA in a death cross** (false rallies)
3. **Weak DMA Diff** (0-5%) with uncertain price position

### 🎯 EXCELLENT PATTERNS (10+ trades with ≤20% error rate)

**14 patterns represent 443 trades with 413 good calls (93.2% success rate)**

| Rank | Price vs 50 DMA | Price vs 200 DMA | DMA Diff | Trades | % Good |
|------|-----------------|------------------|----------|--------|--------|
| 1 | 25-30% | 15-20% | -10 to -5% | 23 | 100.0% |
| 2 | 5-10% | -20 to -15% | -25 to -20% | 16 | 100.0% |
| 3 | 5-10% | 35-40% | 25-30% | 13 | 100.0% |
| 4 | 15-20% | -5 to 0% | -15 to -10% | 13 | 100.0% |
| 5 | 5-10% | 20-25% | 10-15% | 100 | 97.00% |
| 6 | -5 to 0% | 5-10% | 5-10% | 26 | 96.15% |
| 7 | -5 to 0% | -5 to 0% | 0-5% | 33 | 90.91% |
| 8 | 0-5% | 10-15% | 10-15% | 104 | 87.50% |
| 9 | 0-5% | 10-15% | 5-10% | 39 | 87.18% |
| 10 | 0-5% | 5-10% | 0-5% | 24 | 87.50% |

**Common threads in good patterns:**
1. **Strong positive DMA Diff (10-15%)** with reasonable price positions
2. **Pullbacks in strong trends** (negative DMA Diff but price extended)
3. **Price near 50 DMA with positive momentum** (0-5% above with good DMA Diff)

---

## The Critical Insight: Position Matters Less Than Trend

### Analysis by DMA Diff (Most Important Factor)

**DMA Diff 10-15% (Strong Golden Cross)**
- When combined with reasonable price (0-10% above 50 DMA): 87-97% success
- Example: 0-5% / 10-15% / 10-15% = 104 trades, 87.5% success
- Example: 5-10% / 20-25% / 10-15% = 100 trades, 97% success
- **This is your sweet spot for entries!**

**DMA Diff 5-10% (Moderate Uptrend)**
- Mixed results: 60-96% success depending on other factors
- Better when price near 50 DMA: -5 to 0% / 5-10% / 5-10% = 96% success
- Worse when price extended: 0-5% / 5-10% / 5-10% = 60% success

**DMA Diff 0-5% (Weak Trend)**
- Generally poor: 51-91% success (highly variable)
- Can work if other factors align
- Risky - need confirmation from other indicators

**DMA Diff Negative (Death Cross Territory)**
- **DANGEROUS unless it's a deep value play**
- Good ONLY when price severely extended above 50 DMA (25-30%+)
- This indicates oversold bounce in longer-term uptrend
- Most other negative DMA Diff entries fail

---

## The Simple Rules (Derived from Data)

### ✅ BUY When:

1. **DMA Diff 10-15% + Price 0-10% above 50 DMA**
   - Pattern: 0-5% / 10-15% / 10-15% (104 trades, 87.5% success)
   - Pattern: 5-10% / 20-25% / 10-15% (100 trades, 97% success)
   - **These are your bread and butter entries**

2. **DMA Diff 5-10% + Price near 50 DMA**
   - Pattern: -5 to 0% / 5-10% / 5-10% (26 trades, 96% success)
   - Buying the pullback in a building trend

3. **Negative DMA Diff + Price VERY extended above 50 DMA**
   - Pattern: 25-30% / 15-20% / -10 to -5% (23 trades, 100% success)
   - Counter-intuitive but works - oversold bounce
   - Requires price 25%+ above 50 DMA

4. **Neutral trend + Price near DMAs**
   - Pattern: -5 to 0% / -5 to 0% / 0-5% (33 trades, 91% success)
   - Low-risk consolidation entry

### 🚫 DO NOT BUY When:

1. **Death Cross + Price Below 200 DMA**
   - Pattern: 20-25% / -10 to -5% / -30 to -25% (18 trades, 0% success)
   - Pattern: 10-15% / -10 to -5% / -15 to -10% (17 trades, 0% success)
   - **NEVER buy in death cross with price below 200 DMA**

2. **Price Below 50 DMA + Strong DMA Diff**
   - Pattern: -10 to -5% / 0-5% / 10-15% (15 trades, 0% success)
   - Confusing setup - price weak but trend looks strong
   - Wait for confirmation

3. **Weak DMA Diff (0-5%) + Uncertain Price Position**
   - Pattern: -5 to 0% / 0-5% / 0-5% (14 trades, 57% success)
   - No clear trend - coin flip
   - Better opportunities exist

4. **Overextended in Weak Trend**
   - Pattern: 5-10% / 10-15% / 5-10% (16 trades, 19% success)
   - Price looks strong but trend is weak
   - Likely false breakout

---

## High Volume Patterns (Your Trading Habits)

### Top 5 Entry Patterns by Volume:

**#1: Moderate Golden Cross (104 trades, 87.5% success)** ✅
- 0-5% / 10-15% / 10-15%
- Your most common entry - and it works!

**#2: Strong Golden Cross (100 trades, 97% success)** ✅
- 5-10% / 20-25% / 10-15%
- Your second most common - and it's even better!

**#3: Pullback Entry (45 trades, 69% success)** ⚡
- -5 to 0% / 5-10% / 10-15%
- Decent but not great - buying pullbacks needs work

**#4: Moderate Uptrend (39 trades, 87% success)** ✅
- 0-5% / 10-15% / 5-10%
- Another winner

**#5: Consolidation Entry (33 trades, 91% success)** ✅
- -5 to 0% / -5 to 0% / 0-5%
- Good low-risk entry

**Summary**: Your top 5 patterns (321 trades) have 85% success rate overall. Your entry game is actually quite good when you stick to these!

---

## Comparison: Good vs Bad Entry Habits

### Your Strengths (High Volume + High Success):

**443 trades across 14 excellent patterns with 93.2% success rate**

You excel when:
- DMA Diff is 10-15% (strong golden cross)
- Price is 0-10% above 50 DMA (not overextended)
- You buy pullbacks in strong longer-term trends

### Your Weaknesses (Medium Volume + High Failure):

**162 trades across 9 poor patterns with 80.9% failure rate**

You struggle when:
- Buying in death cross territory (negative DMA Diff below 200 DMA)
- Buying extended prices in weak trends
- Buying confusing setups (conflicting signals)

**The Gap**: 
- Your best patterns: 46.3% of trades, 93.2% success
- Your worst patterns: 16.9% of trades, 19.1% success
- **Fix these 9 bad patterns and your overall success rate jumps from 67% to 81%**

---

## How to Use This Table

### Before Every Entry:

1. **Check your three conditions:**
   - Price vs 50 DMA: ____%
   - Price vs 200 DMA: ____%
   - DMA Diff: ____%

2. **Round to 5% buckets**

3. **Look up the pattern in the CSV**

4. **Check the success rate:**
   - **>80% good call rate**: GREEN LIGHT ✅
   - **60-80% good call rate**: YELLOW LIGHT ⚡
   - **<60% good call rate**: RED LIGHT 🔴

### Quick Decision Matrix:

**DMA Diff Check (Most Important):**
- **10-15%**: Usually good (87-97% success with right price position)
- **5-10%**: Moderate (60-96% success - check price position)
- **0-5%**: Weak (51-91% success - risky)
- **Negative**: AVOID unless price very extended (25%+) above 50 DMA

**200 DMA Check (Second Most Important):**
- **Above 200 DMA**: Preferred (long-term uptrend)
- **Below 200 DMA**: High risk unless specific patterns

**Price Position:**
- **0-10% above 50 DMA**: Sweet spot for golden cross entries
- **>20% above 50 DMA**: Only if negative DMA Diff (oversold bounce)
- **Below 50 DMA**: Requires strong DMA Diff confirmation

---

## Examples Using the Table

### Example 1: Should I Buy?
**Current conditions:**
- Price: 7% above 50 DMA → "5 to 10%" bucket
- Price: 22% above 200 DMA → "20 to 25%" bucket
- DMA Diff: 12% → "10 to 15%" bucket

**Look up pattern**: 5-10% / 20-25% / 10-15%
**Result**: 100 trades, 97% good call, 3% bad call
**Decision**: ✅ **BUY! This is your #2 best high-volume pattern!**

### Example 2: Should I Buy?
**Current conditions:**
- Price: 22% above 50 DMA → "20 to 25%" bucket
- Price: -7% below 200 DMA → "-10 to -5%" bucket
- DMA Diff: -28% → "-30 to -25%" bucket

**Look up pattern**: 20-25% / -10 to -5% / -30 to -25%
**Result**: 18 trades, 0% good call, 100% bad call
**Decision**: 🔴 **DO NOT BUY! Worst pattern - 100% failure rate!**

### Example 3: Should I Buy?
**Current conditions:**
- Price: 3% above 50 DMA → "0 to 5%" bucket
- Price: 12% above 200 DMA → "10 to 15%" bucket
- DMA Diff: 11% → "10 to 15%" bucket

**Look up pattern**: 0-5% / 10-15% / 10-15%
**Result**: 104 trades, 87.5% good call, 12.5% bad call
**Decision**: ✅ **BUY! This is your #1 highest volume pattern with excellent results!**

---

## Action Plan

### Priority 1: AVOID These 9 Patterns (Fix 42.5% of Bad Entries)

1. Death cross entries (negative DMA Diff + below 200 DMA)
2. Extended prices in weak trends (high % above 50 DMA, low DMA Diff)
3. Conflicting signals (price below 50 DMA but strong DMA Diff)

**Impact**: Avoiding these 9 patterns = 162 fewer trades but eliminates 131 bad calls!

### Priority 2: FOCUS on These 14 Patterns (93.2% Success Rate)

1. Golden cross entries (DMA Diff 10-15%, price 0-10% above 50 DMA)
2. Pullback entries in strong trends (price near 50 DMA, strong DMA Diff)
3. Consolidation breakouts (neutral position with positive setup)

**Impact**: These patterns = 443 trades with 413 winners (93.2% success)

### Priority 3: Use DMA Diff as Your North Star

**The Single Best Entry Indicator**: DMA Diff

- **10-15%**: BEST ZONE - Golden cross momentum (87-97% success)
- **5-10%**: MODERATE ZONE - Building trend (variable results)
- **0-5%**: WEAK ZONE - Uncertain trend (often fails)
- **Negative**: DANGER ZONE - Avoid unless very specific conditions

---

## Bottom Line

**Your entry game is BETTER than your exit game.**

- Entry success rate: 67.4% (654 good / 970 total)
- But you have 14 excellent patterns with 93.2% success
- Problem: You're mixing in 9 terrible patterns with 19.1% success

**The Fix**: 
1. Stick to DMA Diff 10-15% entries (your wheelhouse)
2. NEVER buy in death cross below 200 DMA
3. Avoid weak trend setups (DMA Diff 0-5%)

Do this and your entry success rate jumps from 67% to 81%+.

**Combined with better exits**, you could have:
- 81% good entries (vs 67% now)
- 70% good exits (vs 37% now)
- Overall success rate: 57% (vs 24% now) ← **More than DOUBLE**
