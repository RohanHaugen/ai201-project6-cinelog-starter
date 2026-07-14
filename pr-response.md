# PR Response Doc — CineLog Watchlist Feature

## AI Usage
<!-- Fill in at the end — how you used AI tools during this project -->

## Comment 1 — Rename
**What I did:**
Renamed save_to_watchlist in watchlist_service.py to add_to_watchlist. Changed implementations of save_to_watchlist in watchlist.py to add_to_watchlist.
**How I verified:**
I used the find-all-references in order to ensure that save_to_watchlist no longer appeared.
## Comment 2 — Deduplication
**What I did:**
Changed add_to_watchlist to check for deduplications, using add_to_collection from collection_service as a reference. Added an error class to watchlist_service for duplicate entries on watchlist.
**How I verified:**
Created a watchlist and added a film to it twice, noting that the second time produced a 409 error.
## Comment 3 — Missing test
**What I did:**
**How I verified:**

## Comment 4 — Default visibility
**My position:**
**Reasoning:**
**Tradeoff acknowledged:**

## Comment 5 — Sort order
**My position:**
**Reasoning:**
**Engagement with reviewer's point:**

## Comment 6 — Rebase
**What conflicted:**
**How I resolved it:**
**How I verified no conflict remains:**

## PR Description
<!-- Written at the end — feature overview, design decisions, manual testing steps -->