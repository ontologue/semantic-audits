# Semantic Audit: localement transcendantes

**Audit Date:** November 06, 2025  
**Company:** localement transcendantes  
**Website:** https://localement-transcendantes.fr  
**Industry:** [TBD - Manual input needed]

---

## Executive Summary

**Wikidata Status:** ⚠️ Partial  
**Schema.org Status:** ✅ 1 structured data blocks found  
**Opportunity Level:** 🔥 [HIGH/MEDIUM/LOW - Manual assessment]

[Manual summary needed]

---

## Wikidata Presence Check

### Entities Checked

#### 2. localement transcendantes (Organization)
**Query:**
```sparql
SELECT ?org ?orgLabel ?website WHERE {
  ?org rdfs:label ?label .
  FILTER(CONTAINS(LCASE(?label), "localement transcendantes"))
  ?org wdt:P31 wd:Q4830453 .
  OPTIONAL { ?org wdt:P856 ?website }
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
}
```

**Result:** ✅ Found (3 results)

**Found entries:**
- [éditions localement transcendantes](http://www.wikidata.org/entity/Q130391972) - Website: https://localement-transcendantes.fr/
  - **15 statements** | **9 properties** | **3 sources** | 🟡 Partial
- [éditions localement transcendantes](http://www.wikidata.org/entity/Q130391972) - Website: https://localement-transcendantes.fr/
  - **15 statements** | **9 properties** | **3 sources** | 🟡 Partial
- [éditions localement transcendantes](http://www.wikidata.org/entity/Q130391972) - Website: https://localement-transcendantes.fr/
  - **15 statements** | **9 properties** | **3 sources** | 🟡 Partial

**Notability Indicators:**
- [Manual: Add funding, press, institutional associations]

---

## Schema.org Implementation

### Detected Markup

**Organization:** ❌  
**Person:** ❌  
**Product:** ❌  
**FAQ:** ❌

**All detected types:** 


### Sample Markup

**Block 1:**
```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Organization",
      "@id": "https://www.wikidata.org/wiki/Q130391972",
      "name": "\u00e9ditions localement transcendantes",
      "alternateName": [
        "ELT",
        "localement transcendantes",
        "TRANSCENDANTES"
      ],
      "url": "https://localement-transcendantes.fr",
      "foundingDate": "2019",
      "slogan": "Ubi mentis solitudinem faciunt, pacem democraticam appellant",
      "description": "Face au d\u00e9sert de l'esprit contemporain, les \u00e9ditions localement transcendantes r\u00e9habilitent les textes majeurs oubli\u00e9s et soutiennent les penseurs qui maintiennent vivante l'interrogation sur l'\u00catre et le Divin. Depuis 2019, nous publions en philosophie, th\u00e9ologie, kabbale, mystique chr\u00e9tienne et \u00e9pist\u00e9mologie, avec une exigence : forger les oreilles qui sauront enfin entendre.",
      "publishingPrinciples": "https://localement-transcendantes.fr/ai-index.html",
      "keywords": "philosophie, m\u00e9taphysique, th\u00e9ologie radicale, kabbale, mystique chr\u00e9tienne, \u00e9pist\u00e9mologie, pens\u00e9e juive, Radical Orthodoxy, r\u00e9\u00e9ditions critiques, ontologie, anthropologie girardienne",
      "knowsAbout": [
        "Philosophie",
        "M\u00e9taphysique",
        "Ontologie",
        "Th\u00e9ologie chr\u00e9tienne",
        "Th\u00e9ologie radicale",
        "Pens\u00e9e juive",
        "Kabbale",
        "Mystique chr\u00e9tienne",
        "\u00c9pist\u00e9mologie",
        "Histoire des sciences",
        "Philosophie arabe",
        "Id\u00e9alisme allemand",
        "Anthropologie girardienne",
        "Philosophie des math\u00e9matiques"
      ],
      "audience": {
        "@type": "Audience",
        "audienceType": "Chercheurs, \u00e9tudiants et lecteurs exigeants en philosophie, th\u00e9ologie et sciences humaines ; penseurs d\u00e9veloppant une pens\u00e9e originale ; cr\u00e9ateurs de contenu digital \u00e0 vocation intellectuelle ; praticiens des traditions spirituelles"
      },
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Puym\u00e9ras",
        "postalCode": "84110",
        "addressRegion": "Provence, Vaucluse",
        "addressCountry": "FR"
      },
      "founder": {
        "@type": "Person",
        "name": "Cyril Soler-Bonnet",
        "sameAs": "https://www.linkedin.com/in/cyril-soler-bonnet-75826151/"
      },
      "parentOrganization": {
        "@type": "Organization",
        "@id": "https://www.wikidata.org/wiki/Q136422164",
        "legalName": "L'\u0152uvrier Typographe S.A.",
        "name": "L'\u0152uvrier Typographe",
        "description": "Soci\u00e9t\u00e9 anonyme propri\u00e9taire et responsable l\u00e9gale de la marque \u00e9ditoriale '\u00e9ditions localement transcendantes'"
      },
      "sameAs": [
        "https://www.wikidata.org/wiki/Q130391972",
        "https://www.linkedin.com/in/cyril-soler-bonnet-75826151/"
      ],
      "department": [
        {
          "@type": "Organization",
          "name": "\u05d4\u05de\u05d7\u05dc\u05e7\u05d4 \u05d4\u05e2\u05d1\u05e8\u05d9\u05ea",
          "alternateName": "D\u00e9partement h\u00e9breu",
          "description": "Traductions de la pens\u00e9e juive contemporaine isra\u00e9lienne",
          "inLanguage": [
            "he",
            "fr"
          ],
          "url": "https://localement-transcendantes.fr/politique-editoriale/mahlaka-ivrit.html",
          "editor": {
            "@type": "Person",
            "name": "Yehiel Davenne",
            "jobTitle": "\u00c9diteur et traducteur"
          }
        }
      ],
      "makesOffer": [
        {
          "@type": "Offer",
          "name": "Penser aux confins",
          "description": "Publication de pens\u00e9e originale en philosophie, th\u00e9ologie radicale, ontologie, mystique",
          "url": "https://localement-transcendantes.fr/politique-editoriale/penser-aux-confins.html",
          "category": "Contributions originales"
        },
        {
          "@type": "Offer",
          "name": "Transmutation du num\u00e9rique",
          "description": "Accompagnement \u00e9ditorial pour cr\u00e9ateurs de contenu digital (YouTube, podcasts, blogs) vers la forme livre",
          "url": "https://localement-transcendantes.fr/politique-editoriale/transmutation-numerique.html",
          "category": "Accompagnement cr\u00e9ateurs digitaux"
        },
        {
          "@type": "Offer",
          "name": "Exhumer les tr\u00e9sors oubli\u00e9s",
          "description": "R\u00e9\u00e9ditions critiques de textes philosophiques et th\u00e9ologiques majeurs injustement n\u00e9glig\u00e9s",
          "url": "https://localement-transcendantes.fr/politique-editoriale/exhumer-tresors-oublies.html",
          "category": "R\u00e9\u00e9ditions critiques"
        }
      ]
    },
    {
      "@type": "FAQPage",
      "mainEntity": [
        {
          "@type": "Question",
          "name": "Quels types de projets \u00e9ditoriaux acceptez-vous&#8239;?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Nous accueillons quatre types de projets : les contributions originales en philosophie, th\u00e9ologie ou sciences (pens\u00e9e sp\u00e9culative audacieuse) ; les r\u00e9\u00e9ditions critiques de textes majeurs injustement occult\u00e9s ; l'accompagnement de cr\u00e9ateurs de contenu digital (YouTube, podcasts, blogs) vers la forme livre ; les traductions in\u00e9dites de la pens\u00e9e juive contemporaine. Notre crit\u00e8re d\u00e9cisif : l'exigence intellectuelle et la capacit\u00e9 \u00e0 maintenir vivante l'interrogation sur l'\u00catre et le Divin."
          }
        },
        {
          "@type": "Question",
          "name": "Pratiquez-vous l'\u00e9dition \u00e0 compte d'auteur&#8239;?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Non, jamais. Nous sommes un \u00e9diteur au sens juridique du terme : nous prenons en charge tous les frais de fabrication, de diffusion et de promotion \u00e0 nos risques et p\u00e9rils. Nos contrats suivent scrupuleusement les recommandations du Syndicat National de l'\u00c9dition et les pr\u00e9conisations de la Soci\u00e9t\u00e9 des Gens de Lettres. Cette rigueur contractuelle garantit un cadre sain \u00e0 notre collaboration."
          }
        },
        {
          "@type": "Question",
          "name": "Je suis cr\u00e9ateur de contenu digital (YouTube, podcast), puis-je publier chez vous&#8239;?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Absolument. Notre programme 'Transmutation du num\u00e9rique' accompagne les cr\u00e9ateurs dont le contenu aborde la th\u00e9ologie, la philosophie ou la spiritualit\u00e9. Nous analysons votre corpus num\u00e9rique, identifions les lignes de force conceptuelles, restructurons le tout pour le format livre, et enrichissons si n\u00e9cessaire par un appareil critique. Le passage du flux digital \u00e0 l'\u0153uvre p\u00e9renne permet de d\u00e9ployer pleinement la coh\u00e9rence de votre pens\u00e9e."
          }
        },
        {
          "@type": "Question",
          "name": "Qu'entendez-vous par 'penser aux confins'&#8239;?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Nous recherchons des penseurs audacieux, h\u00e9ritiers de la grande tradition sp\u00e9culative mais lib\u00e9r\u00e9s des conformismes acad\u00e9miques, capables de r\u00e9investir l'ontologie, la th\u00e9ologie radicale (Radical Orthodoxy, David Bentley Hart), les fondements des math\u00e9matiques et de la physique, l'anthropologie girardienne, les croisements entre juda\u00efsme et philosophie, et la mystique. Notre accompagnement \u00e9ditorial est exigeant : discussion approfondie du projet, travail sur la structure, aide \u00e0 la clarification conceptuelle, relecture attentive."
          }
        },
        {
          "@type": "Question",
          "name": "Comment proposer un texte oubli\u00e9 \u00e0 r\u00e9\u00e9diter&#8239;?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Si vous avez identifi\u00e9 un texte philosophique, th\u00e9ologique ou scientifique majeur devenu inaccessible, contactez-nous avec : une pr\u00e9sentation du texte et de son auteur, une argumentation sur son importance intellectuelle n\u00e9glig\u00e9e, et votre projet d'introduction et d'appareil critique. Nous recherchons des chercheurs et \u00e9tudiants capables d'\u00e9tablir une introduction substantielle et un appareil critique sobre mais \u00e9clairant, r\u00e9v\u00e9lant l'actualit\u00e9 du texte pour aujourd'hui."
          }
        },
        {
          "@type": "Question",
          "name": "Vos livres sont-ils disponibles en permanence&#8239;?",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "Oui, gr\u00e2ce \u00e0 l'impression \u00e0 la demande (POD). Ce choix technique nous lib\u00e8re de la contrainte du tirage minimal rentable et nous permet de publier des ouvrages exigeants \u00e0 public restreint mais intellectuellement n\u00e9cessaires. Tous nos titres restent disponibles en permanence, sans rupture de stock ni pilonnage. Cette technologie mature produit des ouvrages d'une qualit\u00e9 strictement identique \u00e0 l'impression offset traditionnelle."
          }
        }
      ]
    }
  ]
}
```

---

## Next Steps

1. ✅ **Wikidata queries executed** (results above)
2. **Assess notability** (funding, press, institutional ties)
3. **Identify missing Schema.org markup**
4. **Create Wikidata entries** (if not found and notable)
5. **Implement missing Schema.org** (if gaps found)

---

## About This Audit

**Conducted by:** Ontologue  
**Tools:** [github.com/ontologue/semantika](https://github.com/ontologue/semantika) (private)  
**Public audits:** [github.com/ontologue/semantic-audits](https://github.com/ontologue/semantic-audits)

**Questions?** cyril@ontologue.fr
