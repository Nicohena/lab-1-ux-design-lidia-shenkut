# Learning Documentation & Design Resources: Gazzette Plus Rebuild

This document logs the research, design patterns, technical specifications, and resources referenced while critiquing and rebuilding the **Gazzette Plus** Ethiopian news mobile app.

---

## 1. Official Guidelines & Documentation

* **Material Design 3 (M3) Specification:**
  * [Material Design 3 Overview](https://m3.material.io/) – Modern UI layout principles, color system, elevation, and component specs.
  * [Material Components Android GitHub](https://github.com/material-components/material-components-android) – Official Android XML implementation guide for `MaterialCardView`, `Chip`, `TopAppBar`, and `MaterialButton`.

* **Android Accessibility & Touch Targets:**
  * [Android Accessibility - Touch Target Size](https://developer.android.com/guide/topics/ui/accessibility/apps#touch-targets) – Mandating minimum touch target sizes of **48dp × 48dp** for all interactive elements to prevent mis-taps.
  * [WCAG 2.1 Color Contrast Guidelines](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html) – Minimum contrast ratio of 4.5:1 for standard text and 3:1 for large text to ensure outdoor sunlight readability.

---

## 2. Design Patterns for Low-Connectivity & Emerging Markets

* **Offline-First UI Design:**
  * [Designing for Offline & Unstable Networks](https://developer.android.com/architecture/patterns/offline-first) – Best practices for displaying cached data, connection badges, empty states, and storage indicators for Ethiopian mobile network environments.
* **Typography & Reader Views:**
  * [Android Typography Scale](https://m3.material.io/styles/typography/overview) – Guidelines for font hierarchy across headline display, title, body serif text, and metadata tags in news reading apps.

---

## 3. Project Tooling & References

* **Original Student Artifacts:**
  * [`gazzetteplus.drawio.png`](file:///home/benoch/AndroidStudioProjects/WeekndExe/gazzetteplus.drawio.png) – Inherited wireframe from `lab-1-ux-design-lidia-shenkut`.
  * [`ux.pdf`](file:///home/benoch/AndroidStudioProjects/WeekndExe/ux.pdf) – UX tutorial reference.
* **Active Project Repositories:**
  * Original Classroom Repo: [`Debre-birhan-university/lab-1-ux-design-lidia-shenkut`](https://github.com/Debre-birhan-university/lab-1-ux-design-lidia-shenkut)
  * Personal Student Fork: [`Nicohena/lab-1-ux-design-lidia-shenkut`](https://github.com/Nicohena/lab-1-ux-design-lidia-shenkut)

---

## 4. Key Takeaways & Applied Learning

1. **Accessibility First:** Enforcing `minHeight="48dp"` and `minWidth="48dp"` on all buttons, chips, and icons ensures usable interfaces across budget Android hardware with varying touch screen sensitivities.
2. **Resilient UX:** Providing a dedicated Offline Bookmarks screen solves real-world connectivity challenges faced by users in Ethiopia.
3. **High Contrast:** Designing DayNight theme tokens ensures legibility under direct sunlight as well as comfortable night reading.
