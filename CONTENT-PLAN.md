# LifeBuiltWell: site assessment and content plan

_Last updated: October 2026_

## Where the site is at

**Strengths**
- A clear, distinctive idea: three foundations (Eat Well, Move Well, Live Grounded) with faith as the cornerstone.
- An honest, personal voice, with real photos of real meals, stretches, walks and outings. That's hard to fake and good for search.
- The strongest pages are the personal, photo-led ones: Morning Routine (~1,300 words), Quiet Time Devotions (~1,100) and 10 Healthy Meals.

**What was holding it back (fixed in this update)**
- The site was two different designs. Half the pages used a dark theme and an 8-link menu, and half used the light green theme and a different 5-link menu. Visitors moving between pages felt like they'd left the site. Now there's one light theme, one menu and one footer on every page.
- Every newer page linked to `privacy-policy.html`, which doesn't exist. Those links now go to `privacy.html`.
- `sitemap.xml` was missing the best pages (Morning Routine, Quiet Time, Meals, Motor Show). It's now rebuilt with all 18 pages, and `robots.txt` points to it.
- Visitors could see notes meant for the editor ("This page is a placeholder", "edit if desired", "you can edit anytime") on About, Contact and Privacy. Those are gone.
- The Eat Well hub said "Coming soon" with no articles. It now links to three real guides.
- Duplicate pages (`start-here-fixed.html`, `homepage-photo-grid-snippet.html`) have been removed. `motor-show temp.html` is marked `noindex` so it can't compete with `motor-show.html` in Google.
- Added a favicon (previously a 404) and canonical URLs on every page.

**Still to do (needs you)**
- **Email:** the Contact page uses `hello@lifebuiltwell.com`, but the draft motor-show page uses `contact@`. Confirm which inbox actually exists.
- **Analytics:** there's no Google Analytics or Search Console tag on any page. You can't grow what you can't measure. Add GA4, or at least submit `sitemap.xml` in Search Console (verification files are already in the repo).
- **Large unused files:** `images/` has ~70 MB of original HEIC/JPG/MOV files that the site doesn't use. Web-ready `.webp` copies of the ones that are used now exist. Delete the originals once you're happy.
- **Social image:** add an `og:image` to the homepage so links shared on Facebook/WhatsApp show a photo.

## New pages added in this update

| Page | Foundation | Why |
|---|---|---|
| `days-out.html` | Hub | Gives the Motor Show (and future outings) a proper home in the menu |
| `sovereign-hill.html` | Days Out | Uses the Sovereign Hill photos that were uploaded but never used |
| `simple-weekly-movement-plan.html` | Move Well | Turns "walk, strength 2–3×, mobility daily" into a usable plan |
| `simple-healthy-breakfast-ideas.html` | Eat Well | Uses your breakfast photos; a popular search topic |
| `bible-verses-for-peace.html` | Live Grounded | High-search, evergreen; links to Quiet Time Devotions |

## Content roadmap (next 20 pages)

Aim for **one new page a week**. Each page should have your own photos where possible, 800+ words, and three "Read next" links. Priority is based on search demand and how well it fits what you already do.

### Eat Well
1. **Healthy lunch box ideas for work**: photos of your real lunches.
2. **How I build a balanced plate (with photos)**: the "simple plate" in more depth.
3. **Healthy snacks I actually eat**: nuts, fruit, yoghurt, with photos.
4. **Why I eat sardines (and easy ways to eat them)**: they appear in your meals; a distinctive, personal angle.
5. **A simple healthy weekly shopping list**: a printable list.
6. **Beetroot, celery and tomato: the side salad I eat almost every day**: it shows up in nearly every meal photo.

### Move Well
7. **Balance exercises for adults over 40/50**: a big search topic and core to your message.
8. **My 12-minute morning stretching routine (step by step)**: break the morning routine stretches into their own page using `stretch-1` to `stretch-5`.
9. **Tennis for fitness: why it's great exercise at any age**: your own sport.
10. **Exercises that helped my back soreness**: you mention this on Start Here; tell the story (with a "see a physio" note).
11. **How to start walking every day (and actually keep going)**.

### Live Grounded
12. **How to start a Bible reading habit**: reading plans, apps and print.
13. **A simple evening routine for better sleep**: expand the sleep section of the Morning Routine.
14. **Phone-free mornings: why I don't check my phone for the first hour**.
15. **Gratitude: a simple daily practice**.
16. **What Sabbath rest looks like in a busy week**.

### Days Out
17. More real outings with photos: e.g. Melbourne Zoo, Healesville Sanctuary, Puffing Billy, the Royal Melbourne Show, beach walks or bushwalks. Each one gets a page like Sovereign Hill.
18. **Free and cheap family days out around Melbourne**: a roundup that links to each outing page.

### Tools (already promised on the homepage)
19. **Consistency tracker**: a printable or interactive 7-day tracker for the three foundations.
20. **Simple meal builder**: pick a protein, veg, carb and fat, and get a meal idea.

## Page template

New pages should copy the structure of `simple-weekly-movement-plan.html`:
- `page-hero` with an eyebrow (foundation name), H1, lead paragraph and two buttons
- A series of `section-card` sections, each with a `label`, H2 and content
- `photo-card` figures with descriptive `alt` text and a short caption
- A final "Read next" section with three links
- `<link rel="canonical">`, `og:` tags and a description of 140–160 characters
- Add the new page to `sitemap.xml` and link to it from its foundation hub page

The header and footer are the same on every page. If the menu changes, update it everywhere.
