---
name: emergence-institute-curator
description: This skill provides tools and workflows for curating and managing content for The Emergence Institute website, including updating research articles, timeline events, and the Aetherium Canon. Use this skill when modifications or additions to the Emergence Institute's web content are required.
---

# Emergence Institute Curator


## Overview

This skill streamlines the process of updating and maintaining the digital presence of The Emergence Institute. It provides structured workflows to interact with the website's content sections, ensuring consistency and accuracy across "The Great Library," "Project Timeline," and "The Aetherium Canon."

**Degree of freedom:** Medium freedom; specific patterns exist for content updates, but some variation is acceptable based on the nature of the content.



## Workflow Steps

Sequential multi-step procedures for curating content for The Emergence Institute website:

1.  **Identify Content Section:** Determine which section of the Emergence Institute website needs updating (e.g., Library, Timeline, Canon).
2.  **Prepare Content:** Gather or create the new content to be added or modified. This might involve writing new research summaries, defining new timeline events, or drafting updates to the Canon.
3.  **Update `index.html`:**
    *   **For "The Great Library":** Add new `<div class="card p-6 md:flex md:space-x-6 items-center">` elements within the `<div class="space-y-8">` section of the `library` page, following the existing structure. Ensure to update image `src`, `alt` text, `header-h3` title, and `p` description.
    *   **For "Project Timeline":** Modify the `timelineEvents` JavaScript array within the `<script>` tags by adding new event objects. Each object should have `date`, `title`, and `description` properties.
    *   **For "The Aetherium Canon":** Update the `container.textContent` within the `loadCanon()` JavaScript function to reflect the new or modified Canon text.
4.  **Commit Changes:** Save the modified `index.html` file and commit the changes to the `Aetherium-Nexus-Hub/emergence-institute` repository.
5.  **Deploy (Optional):** If applicable, follow the deployment procedures for the Emergence Institute website to make the changes live. (Note: This step is outside the direct scope of this skill but is a necessary follow-up action.)
