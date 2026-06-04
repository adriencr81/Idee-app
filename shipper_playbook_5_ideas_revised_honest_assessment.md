# Playbook Shipper: 5 Idées — Révision Honnête (Juin 2026)

**Date:** 4 juin 2026  
**Status:** REVISED ASSESSMENT — ZapFlow downgraded, QuickAvatar + ClientGrow upgraded

---

## 🚨 La Révision

J'ai d'abord présenté ZapFlow comme #1. **J'avais tort.**

### Pourquoi ZapFlow est plus complexe que présenté

#### 1. **Les Intégrations API = Maintenance Permanente**
```
Initial thought: "Just call 5 APIs, done"

Reality:
- Stripe API changes → code breaks → user's automations fail
- Notion API deprecates → need to rewrite → user loses data
- Slack API changes → need to update → more testing
- Each API has: OAuth, rate limiting, webhooks, error handling

Timeline: 
- Week 1-2: Build 1 integration (seems easy)
- Week 3-4: Add 2nd integration (harder, conflicts)
- Week 5-6: Add 3rd integration (debugging nightmare)
- Week 7-8: Add 4th-5th (you're exhausted)
- Month 3: First API breaks → emergency fix
- Month 4: 2nd API changes → emergency fix
- Month 5+: Permanent firefighting mode

Realistic effort: NOT 5-6 weeks, actually 12+ weeks initial + 20h/week maintenance forever
```

#### 2. **Zapier's Defensibility is REAL**
```
Zapier advantages:
- 1000+ integrations (you have 5)
- Massive brand (everyone knows Zapier)
- Network effects (Zapier devs build on top)
- $5B valuation (has resources to dominate)
- Switching cost = high (users invested in Zapier workflows)

Your advantage:
- Cheaper ($9/mth vs $20/mth)
- Simpler (5 integrations vs 1000)

Reality: Zapier can cut prices to $9/mth tomorrow → you lose only advantage
```

#### 3. **Network Effects Don't Exist**
```
QuickAvatar: Creator makes video → shares on TikTok → 10k see it → 500 signups
ClientGrow: Freelancer uses it → tells 5 freelancer friends → word-of-mouth

ZapFlow: User creates automation → nobody sees it → no viral loop
= Network effect = ZERO
```

#### 4. **Acquisition is Hard**
```
- No one shares their automations on Twitter
- No viral potential
- SEO weak ("simple automation" = nobody googles this)
- PPC = too expensive vs revenue
- Direct sales = founder's burden forever

Growth path: Unclear. How do you get to 1000 customers without viral or sales?
```

---

## ✅ New Ranking

### **🥇 QuickAvatar** (vs Synthesia @ $4B)

**Why it wins:**

| Aspect | Reality |
|---|---|
| **Tech Complexity** | 🟢 EASY (call API + post TikTok) |
| **Maintenance** | 🟢 LOW (2-3 APIs, stable) |
| **Viral Potential** | 🟢🟢🟢 MASSIVE |
| **Network Effects** | 🟢 HUGE (creators share videos) |
| **TAM** | ⭐⭐⭐⭐⭐ (1.5M+ creators) |
| **Time to MVP** | 6-8 weeks |
| **Time to $10k/mth** | 2-3 months (with viral) |
| **Defensibility** | 🟢 Medium (hard to copy viral) |

**The Play:**
1. Build QuickAvatar in 6-8 weeks
2. Make 5 demo TikToks (showing it works)
3. Post TikTok → viral → 10k visits
4. Product Hunt → 5k upvotes
5. Creators naturally share → exponential growth

**Upside:** If one video goes viral = $50k+/mth day 1

---

### **🥈 ClientGrow** (vs Mind @ Unicorn)

**Why it's solid:**

| Aspect | Reality |
|---|---|
| **Tech Complexity** | 🟢 EASY (CRM + email + invoicing) |
| **Maintenance** | 🟢 LOW (Stripe stable, email stable) |
| **Viral Potential** | 🟡 MEDIUM (word-of-mouth) |
| **Network Effects** | 🟡 GOOD (freelancers tell freelancers) |
| **TAM** | ⭐⭐⭐⭐⭐ (27M+ freelancers) |
| **Time to MVP** | 4-5 weeks |
| **Time to $10k/mth** | 2-3 months (steady growth) |
| **Defensibility** | 🟢 Medium (switching cost = medium) |
| **Proof of Demand** | ✅ Mind raised $50M, became unicorn |

**The Play:**
1. Build MVP in 4-5 weeks
2. Email 100 freelancers directly
3. Product Hunt launch
4. Word-of-mouth kicks in
5. Steady, predictable growth

**Upside:** Consistent $50k/mth achievable (no viral needed)

---

### 3️⃣ **SimpleBuild** (vs Lovable @ $6.6B)

**Challenges:**
- 🔴 Lovable has massive hype (every maker knows it)
- 🔴 TAM smaller than I said (100k vs 1M+)
- 🔴 Hard to differentiate (both AI + no-code)
- 🔴 Lovable can drop price from $20 to $10 → you're stuck
- 🟡 Viable but lower ceiling ($5-10k/mth potential)

---

### ❌ **ZapFlow** (vs StackOne/Zapier)

**Why I was wrong:**
- 🔴 API maintenance = nightmare forever
- 🔴 Zapier dominates with 1000 integrations
- 🔴 Zero network effects
- 🔴 Acquisition unclear (how do you grow?)
- 🔴 One Zapier price cut = you lose only advantage
- 🔴 5 integrations look simple, actually 12+ weeks work

**Verdict:** Skip this. Better ideas exist.

---

### ❌ **MedPerplexity** (vs Perplexity @ $20B)

**Why it's hard:**
- 🔴 Medical compliance = liability nightmare
- 🔴 Data curation = 3 months of work (before code)
- 🔴 B2B sales cycle = 6 months minimum
- 🔴 Regulatory = slow (healthcare = regulated)
- 🔴 First $10k/mth = month 5-6 (not realistic in 3 months)

**Verdict:** Biggest TAM but highest friction. Build later (after easier wins).

---

## 📊 Final Scoring

| Idea | Complexity | TAM | Viral | Growth Path | Timeline | Potential | Rank |
|---|---|---|---|---|---|---|---|
| **QuickAvatar** | 🟢 Easy | ⭐⭐⭐⭐⭐ | 🟢🟢🟢 | Viral TikTok | 6-8w | $10-50k/mth | **🥇 #1** |
| **ClientGrow** | 🟢 Easy | ⭐⭐⭐⭐⭐ | 🟡 Medium | Word-of-mouth | 4-5w | $10-20k/mth | **🥈 #2** |
| **SimpleBuild** | 🟡 Medium | ⭐⭐⭐⭐ | ❌ Low | Unclear | 4-5w | $5-10k/mth | 3️⃣ |
| **ZapFlow** | 🔴 Hard | ⭐⭐⭐⭐ | ❌ None | Unclear | 12+w | $5-15k/mth | ❌ SKIP |
| **MedPerplexity** | 🔴 Hard | ⭐⭐⭐⭐⭐ | ❌ None | B2B Sales | 16+w | $20-50k/mth | 4️⃣ |

---

## 🎯 My Honest Recommendation

**Pick ONE of these:**

### **Option A: Go for Home Run (Viral Potential)**
→ **QuickAvatar**
- Build 6-8 weeks
- Launch on TikTok
- If 1 video goes viral = $50k+/mth
- Risk: Viral is random, but the upside is massive

### **Option B: Boring but Safe (Predictable Growth)**
→ **ClientGrow**
- Build 4-5 weeks  
- Launch + direct outreach
- $10-15k/mth in 3 months guaranteed
- Risk: Lower (proven market, simple tech)
- Upside: Slower but consistent (compound to $100k/mth over 1 year)

---

## 🚀 Decision Point for Tomorrow

**Challenge ClientGrow** means:
1. Deep dive into freelancer market
2. Test if demand is REALLY there
3. Validate pricing ($15/mth)
4. Identify distribution channels
5. Build realistic launch plan

Goal: Decide if ClientGrow is your next move, or pivot to something else.

---

## Key Learnings

1. **Simple-sounding ideas hide complexity** (ZapFlow looked simple, actually hard)
2. **API integrations = maintenance burden forever** (not just build once)
3. **Viral potential matters** (QuickAvatar = exponential, ZapFlow = linear ceiling)
4. **Proven market > untested market** (Mind proved demand, easier to sell ClientGrow)
5. **Network effects are everything** (creators share videos, freelancers share tools)

---

## Files Saved

- `shipper_playbook_5_ideas_detailed_explanations.md` — Initial analysis (keep for reference)
- `shipper_playbook_5_ideas_revised_honest_assessment.md` — This file (honest takes)
- `clientgrow_challenge_deep_dive.md` — Ready for tomorrow's challenge

**Next:** Tomorrow, we challenge ClientGrow with real data 🎯
