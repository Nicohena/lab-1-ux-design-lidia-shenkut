# Gazzette Plus - Layout Preview Screenshots & Render Specs

This directory contains layout preview documentation and screenshots rendering the **Gazzette Plus** Android XML designs across multiple display sizes (Standard Phone 5.1" and Large Display 6.7").

---

## Screen Previews Overview

| Screen Name | Layout Resource XML | Rendered Features | Device Sizes Tested |
| :--- | :--- | :--- | :--- |
| **1. Home News Feed** | `app/src/main/res/layout/activity_main.xml` | Top app bar with search & offline sync status pill, horizontal category filter chips, breaking news hero card, article feed cards | Phone 5.1" (Budget), Phone 6.7" |
| **2. Article Detail Reader** | `app/src/main/res/layout/activity_article_detail.xml` | Top action toolbar, hero banner, author/time metadata, reader mode options (A-/A+ font resize, listen audio), high-contrast body text | Phone 5.1" (Budget), Phone 6.7" |
| **3. Saved Offline Bookmarks** | `app/src/main/res/layout/activity_bookmarks.xml` | Storage usage badge (3 Articles Cached / 4.2 MB), cached offline article feed cards, empty state UI layout | Phone 5.1" (Budget), Phone 6.7" |

---

## Rendered Layout Specs & Accessibility Compliance

* **Minimum Touch Target Height:** All interactive buttons (`btn_top_search`, category chips, `btn_font_decrease`, `btn_font_increase`, `btn_listen_audio`, `btn_item_bookmark`) enforce `minHeight="48dp"` and `minWidth="48dp"`.
* **Outdoor Sunlight Legibility:** High-contrast color tokens (`text_primary: #1C1B1F`, `background_light: #F8F9FA`, `primary: #B71C1C`) guarantee clear visibility under bright natural sunlight in Ethiopia.
* **Responsive Scaling:** Flexible layout weights and `ScrollView` scroll containers ensure zero overflow or clipped text on both small budget screens and modern widescreen displays.
