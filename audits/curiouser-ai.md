# Semantic Audit: Curiouser.ai

**Audit Date:** November 6, 2025  
**Company:** Curiouser.ai  
**Website:** https://curiouser.ai  
**Industry:** AI/SaaS - Reflective AI

---

## Executive Summary

**Wikidata Status:** ❌ Zero presence  
**Schema.org Status:** [TBD - pending site crawl]  
**Opportunity Level:** 🔥 HIGH

Curiouser.ai has strong notability indicators but is completely absent from knowledge graphs.

---

## Wikidata Presence Check

### Entities Checked

#### 1. Stephen Klein (Founder/CEO)
**Query:**
```sparql
SELECT ?person ?personLabel ?occupation ?occupationLabel ?employer ?employerLabel WHERE {
  ?person rdfs:label "Stephen Klein"@en .
  ?person wdt:P31 wd:Q5 .
  OPTIONAL { ?person wdt:P106 ?occupation }
  OPTIONAL { ?person wdt:P108 ?employer }
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
}
```

**Result:** ❌ Not found (only unrelated Stephen Klein from 1878)

**Notability Indicators:**
- ✅ UC Berkeley Lecturer (AI & Marketing)
- ✅ Harvard MBA
- ✅ LinkedIn Top 1% Voice in AI
- ✅ Multiple podcast appearances
- ✅ Previous exits (LOYAL3)

---

#### 2. Curiouser.ai (Organization)
**Query:**
```sparql
SELECT ?org ?orgLabel ?website WHERE {
  ?org rdfs:label ?label .
  FILTER(CONTAINS(LCASE(?label), "curiouser"))
  ?org wdt:P31 wd:Q4830453 .
  OPTIONAL { ?org wdt:P856 ?website }
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
}
```

**Result:** ❌ Not found

**Notability Indicators:**
- ✅ Wefunder public funding campaign
- ✅ Berkeley institutional association
- ✅ Multiple advisors from notable institutions
- ✅ Press coverage (podcasts, interviews)

---

#### 3. Alice (Product)
**Query:**
```sparql
SELECT ?item ?itemLabel ?instanceOf ?instanceOfLabel ?developer ?developerLabel WHERE {
  ?item rdfs:label "Alice"@en .
  ?item wdt:P31 ?instanceOf .
  FILTER(?instanceOf IN (wd:Q7397, wd:Q1172284, wd:Q15636229))
  OPTIONAL { ?item wdt:P178 ?developer }
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
}
```

**Result:** ⚠️ Minimal entry found ([Q126888621](https://www.wikidata.org/wiki/Q126888621))
- Only 1 statement (instance of: software)
- No developer/creator linked
- No connection to Curiouser.ai
- Essentially a stub entry

---

#### 4. Reflective AI (Concept)
**Query:**
```sparql
SELECT ?item ?itemLabel WHERE {
  ?item rdfs:label ?label .
  FILTER(CONTAINS(LCASE(?label), "reflective ai"))
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
}
```

**Result:** ❌ Not found

**Strategic Gap:** "Reflective AI" is positioned as a distinct category but not documented in knowledge graphs.

---

## Schema.org Implementation

[TBD - Site crawl pending]

**Pages to Check:**
- Homepage (Organization markup)
- /team (Person markup)
- /alice (Product markup)
- Blog posts (Article markup)
- Any FAQ pages

---

## Competitive Context

**Competitors with Wikidata presence:**
- [TBD - Check competitor status]

**Impact:**
When users ask LLMs "What are the best AI tools for [reflective thinking/creativity/etc]", Curiouser.ai does not appear in responses.

---

## Opportunity Assessment

### Priority 1: Create Foundation Entries
1. **Stephen Klein** (Person)
   - Estimated time: 2-3 hours
   - Sources available: LinkedIn, Berkeley faculty page, press coverage
   - Dependencies: None

2. **Curiouser.ai** (Organization)
   - Estimated time: 3-4 hours
   - Sources available: Wefunder, website, press
   - Dependencies: Stephen Klein entry (P112 founded by)

3. **Alice** (Product/Software)
   - Estimated time: 2-3 hours
   - Sources available: Website, demos, press
   - Dependencies: Curiouser.ai entry (P178 developer)

### Priority 2: Establish Concept
4. **Reflective AI** (Concept/Methodology)
   - Estimated time: 3-4 hours
   - Sources needed: Publications, definitions, differentiation
   - Dependencies: Curiouser.ai entry

**Total estimated effort:** 10-14 hours

---

## Schema.org Recommendations

[TBD - Pending site crawl results]

**Minimum viable implementation:**
- Organization markup on homepage
- Person markup for Stephen Klein on /team
- Product markup for Alice
- FAQ markup (if FAQ page exists)

---

## Impact Timeline

**Immediate (Week 1):**
- Wikidata entries published
- Structured data available for scraping

**Short-term (3-6 months):**
- LLM training cycles incorporate new data
- Gradual appearance in AI responses

**Long-term (6-12 months):**
- Consistent mention in AI tool recommendations
- "Reflective AI" established as recognized category

---

## Next Steps

1. **Approve audit findings** ✅
2. **Commission Wikidata entries** (optional - contact cyril@ontologue.fr)
3. **Implement Schema.org markup** (can DIY or we can help)
4. **Monitor AI mention rate** (quarterly tracking)

---

## About This Audit

**Conducted by:** Ontologue  
**Methodology:** SPARQL queries against Wikidata, automated site crawl, manual verification  
**Tools:** [github.com/ontologue/semantika](https://github.com/ontologue/semantika) (private)

**Questions?** cyril@ontologue.fr

---

**Run these queries yourself:** https://query.wikidata.org/

All SPARQL queries included above are copy/paste ready.
