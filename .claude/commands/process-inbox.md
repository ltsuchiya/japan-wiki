Process all files currently in `inbox/` (repo root) and convert them into proper wiki pages under `content/`.

For each file in `inbox/`:

1. **Read** the file and understand its content and topic.

2. **Ask clarifying questions** before proceeding. At minimum, ask:
   - Why is this information relevant to someone relocating to Japan specifically? (e.g. is this a Japan-specific rule, a comparison with the US, a practical step required during the move?)
   - Is there a specific stage of the relocation this applies to (before departure, during the move, after arrival)?
   - Are there any nuances, caveats, or personal priorities the user wants captured that aren't obvious from the raw notes?

   Wait for the user's answers before continuing. Use the responses to shape the framing and focus of the wiki page.

3. **Determine the target folder** — pick one of: `content/cars/`, `content/real-estate/`, `content/taxes/`, `content/phones/`, `content/timeline/`. If the content spans multiple topics, split it into separate pages, one per folder. If the content doesn't clearly fit any existing folder, propose a new folder name (kebab-case, one word or short phrase), explain why none of the existing ones apply, and wait for approval before creating it.

4. **Create one or more wiki pages** in the correct folder(s):
   - Filename: kebab-case, descriptive (e.g. `importing-a-us-car.md`, not `notes.md`)
   - Add the required frontmatter at the top:
     ```yaml
     ---
     title: <Page Title>
     tags: [<topic>, <optional sub-topic>]
     date: <YYYY-MM-DD>
     updated: <YYYY-MM-DD>
     ---
     ```
   - Do NOT include an `# H1` in the body — the title frontmatter serves as the heading.
   - Organise the body clearly using `##` and `###` subheadings as needed.
   - Use markdown tables for any comparisons (e.g. Japan vs. US rules, option A vs. option B).
   - Include a `## References` section at the bottom with links to the reputable sources the information comes from (official government sites, authoritative guides, etc.). If the raw notes don't cite sources, flag this to the user rather than omitting the section silently.

5. **Add `[[wikilinks]]`** to any existing related pages where relevant (e.g. a car-import page should link to an import duties taxes page if that page exists).

6. **Remove the original file** from `inbox/` once it has been filed.

After processing all inbox files, print a summary of:
- Files processed
- Pages created (with their paths)
- Any wikilinks added to existing pages
