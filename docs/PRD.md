# narrativeAI PRD

## 1. Product Summary

`narrativeAI` is an AI-assisted visual storytelling app that turns a sequence of images and user-written memories into a connected storybook.

Instead of asking AI to invent the whole story from photos alone, the user adds the meaning behind each image. AI then helps connect those moments into a coherent narrative with transitions, chapters, emotional pacing, and exportable keepsakes.

The first wedge is wedding picture books, but the bigger vision is to help people connect fragmented memories into complete personal, family, or event stories.

## 2. Problem

People take many meaningful photos, but the story behind each image is usually scattered, forgotten, or never written down.

Wedding couples often receive hundreds or thousands of photos after the event, but most of the value is trapped in unorganized albums. The photos show what happened, but not always why each moment mattered.

Common pain points:

- Photos are beautiful but hard to revisit meaningfully.
- Couples do not have time to turn individual memories into a coherent story.
- Standard photo albums feel generic.
- AI-generated captions can feel generic when the user does not provide personal context.
- Wedding vendors need differentiated post-event products.
- Family and guests want a simple way to relive the story, not browse a massive gallery.

## 3. Target Users

### Primary User

Newly married couples who want a memorable, personalized wedding keepsake and are willing to add short notes about meaningful photos, but do not want to manually write and design the full storybook.

### Secondary Users

- Wedding photographers who want to offer AI-generated storybooks as an add-on.
- Wedding planners who want a premium post-event deliverable.
- Family members or friends creating a gift for the couple.

## 4. Strategic Positioning

Initial positioning:

> "Add photos and memories. Let AI connect them into a beautiful story."

Potential market wedge:

- Start with weddings because the emotional value and willingness to pay are high.
- Expand later into proposals, anniversaries, baby showers, birthdays, graduation, corporate retreats, and milestone events.

Long-term positioning:

> "A storytelling layer for your most important life moments."

## 5. Goals

### Product Goals

- Let users add images and short story notes for each image.
- Let AI connect individual image stories into a coherent full narrative.
- Let users generate a polished wedding storybook from their photos and memories.
- Make the first usable draft available quickly.
- Allow simple edits without requiring design skills.
- Support export and sharing.

### Business Goals

- Validate willingness to pay for AI-generated wedding keepsakes.
- Test whether distribution is stronger through direct-to-couple channels or wedding vendor partnerships.
- Build reusable infrastructure for image-based storytelling beyond weddings.

## 6. Non-Goals

For the MVP, the product will not:

- Replace professional photographers.
- Provide full photo gallery hosting.
- Offer advanced design software features.
- Handle physical printing and shipping directly.
- Support every event type from day one.

## 7. MVP Scope

### Core Features

1. Photo Upload
   - User can upload a batch of wedding photos.
   - App supports common image formats such as JPG and PNG.
   - App shows upload progress and basic error states.

2. Photo Selection
   - User can select the photos to include in the storybook.
   - App can optionally suggest the best photos based on quality, uniqueness, and people presence.

3. Per-Image Story Input
   - User can add a short memory, caption, or context note to each selected image.
   - User can optionally answer prompts such as "What was happening here?", "Why does this moment matter?", or "Who is in this photo?"
   - App can use AI to clean up rough notes without changing the user's intended meaning.

4. Story Connection
   - App connects the image-level stories into a larger narrative arc.
   - App generates transitions between moments.
   - App groups related images into chapters or sections.
   - Output includes title, chapters, page captions, transition copy, and closing reflection.
   - Tone options may include romantic, elegant, playful, cinematic, or heartfelt.

5. Storybook Editor
   - User can edit generated text.
   - User can reorder pages.
   - User can remove photos from the book.
   - User can regenerate captions, transitions, or chapter text.

6. Preview
   - User can preview the generated storybook as a page-by-page experience.
   - Preview should work well on desktop and mobile.

7. Export and Share
   - User can export the storybook as PDF.
   - User can generate a shareable web link.

### Nice-To-Have Features

- AI-generated cover title.
- AI prompts that ask better follow-up questions for weak or vague story notes.
- Multiple layout templates.
- Face-aware grouping of important people.
- Dedication page.
- Guest messages integration.
- Print-ready PDF export.
- Vendor-branded exports for photographers and planners.

## 8. User Journey

1. User lands on the app.
2. User creates a new wedding storybook project.
3. User uploads wedding photos.
4. User selects photos or accepts AI suggestions.
5. User adds short story notes to selected photos.
6. User chooses a story tone.
7. App connects the image-level stories into a full draft storybook.
8. User edits captions, transitions, order, and title.
9. User previews the final storybook.
10. User exports PDF or shares a link.

## 9. Key Screens

### 1. Project Creation

Purpose: Start a new wedding storybook.

Required inputs:

- Couple names
- Wedding date
- Optional venue
- Preferred tone

### 2. Upload Screen

Purpose: Upload and manage wedding images.

Required functionality:

- Drag-and-drop upload
- File picker
- Upload progress
- Upload error messages
- Thumbnail grid

### 3. Photo Selection Screen

Purpose: Choose which photos become part of the storybook.

Required functionality:

- Select or deselect photos
- Sort by uploaded order
- Mark cover photo
- Optional AI recommendations

### 4. Image Story Input Screen

Purpose: Capture the personal meaning behind each image.

Required functionality:

- Display one image at a time or in a focused grid
- Text input for each image's story
- Optional guided prompts
- AI rewrite for clarity
- Completion indicator for images with missing story notes

### 5. Story Connection Screen

Purpose: Generate the connected storybook draft.

Required functionality:

- Show generation status
- Indicate current step
- Handle generation failure
- Allow retry

### 6. Storybook Editor

Purpose: Refine the generated book.

Required functionality:

- Page list
- Page preview
- Editable title and captions
- Editable transitions between images or chapters
- Reorder pages
- Regenerate selected text
- Delete page

### 7. Preview and Export

Purpose: Review and deliver the final storybook.

Required functionality:

- Full storybook preview
- PDF export
- Shareable link
- Basic access control for private links

## 10. Functional Requirements

### Upload

- The app must support multi-image upload.
- The app must validate file type and file size.
- The app must store uploaded images securely.
- The app must preserve image ordering metadata where possible.

### AI Generation

- The app must generate story text based on selected images, project metadata, and per-image user notes.
- The app must connect image-level stories into a coherent overall storyline.
- The app must generate transitions between images or chapters.
- The app must support at least three tones in MVP.
- The app must avoid inventing sensitive personal details not provided by the user.
- The app must allow users to regenerate weak output.

### Story Input

- The app must allow users to add story notes to each selected image.
- The app must support rough, incomplete notes and improve them with AI.
- The app must make it clear which images still need story input.
- The app must preserve the user's original meaning when rewriting or connecting story notes.

### Editing

- The app must allow users to edit all generated copy.
- The app must allow page reordering.
- The app must allow removing photos or pages.
- The app must allow editing the source story note for each image.

### Export

- The app must generate a PDF.
- The app must support a shareable web preview.
- The app must preserve basic layout consistency across export formats.

## 11. Non-Functional Requirements

- Uploaded photos should be private by default.
- Share links should be unlisted and difficult to guess.
- The app should clearly communicate when AI generation is in progress.
- MVP generation should complete within a few minutes for a typical batch.
- The editor should be responsive on desktop and tablet.
- Mobile should support preview and light editing.

## 12. Monetization

Potential pricing models:

- One-time purchase per storybook.
- Freemium preview with paid export.
- Photographer or planner subscription.
- White-label vendor package.
- Premium print-ready export.

Suggested MVP monetization test:

- Free upload and preview.
- Paid PDF export.
- Higher-priced vendor-branded package for photographers.

## 13. Success Metrics

### Activation

- Percentage of users who upload at least 20 photos.
- Percentage of selected images with user-added story notes.
- Percentage of users who generate a first draft.

### Engagement

- Average number of edits per storybook.
- Percentage of users who preview the full book.
- Regeneration rate for captions, transitions, or pages.
- Average story note length per image.

### Revenue

- Export conversion rate.
- Average revenue per completed storybook.
- Vendor lead conversion rate.

### Quality

- User rating after generation.
- Percentage of generated books exported without major edits.
- Support requests per completed storybook.

## 14. Key Risks and Assumptions

### Assumption 1: Couples Will Pay

The product assumes couples value an AI-generated storybook enough to pay for export or sharing.

Validation:

- Test a landing page with pricing.
- Offer concierge generation manually before building full automation.
- Run pilots with recent wedding couples.

### Assumption 2: Vendors Are Better Distribution

Photographers and planners may be stronger acquisition channels than direct ads.

Validation:

- Interview 10 wedding photographers.
- Offer a white-label sample book.
- Test commission-based partnership.

### Assumption 3: Users Will Add Story Context

The product assumes users are willing to add short notes to photos if the payoff is a better connected story.

Validation:

- Measure completion rate for per-image notes.
- Test guided prompts versus blank text boxes.
- Compare output quality between photos-only generation and photo-plus-memory generation.

### Assumption 4: AI Output Is Emotionally Good Enough

Generic captions will not be enough. The output must feel personal, polished, and faithful to the user's memories.

Validation:

- Compare generated books with human-curated examples.
- Let users rate emotional accuracy.
- Add lightweight prompts for couple story details.

### Assumption 5: Story Connection Is More Valuable Than Caption Generation

The key value is not just writing captions. The key value is helping users connect fragmented moments into a whole story.

Validation:

- Ask users whether transitions and chapter structure are useful.
- Measure how often users edit AI-generated transitions.
- Test whether users would still pay if captions were simple but storyline quality was strong.

### Assumption 6: Photo Understanding Is Sufficient

The app can use image understanding to support story generation, but user-provided context remains the main source of truth.

Validation:

- Use user-provided event sections such as ceremony, reception, family, speeches, and couple portraits.
- Allow manual reordering.
- Measure how much manual correction is needed.

## 15. Tech Stack

The MVP should prioritize speed, low operational overhead, type safety, and a clean path to production. The recommended stack is a TanStack-based full-stack React app with managed database, auth, storage, and a separate worker for long-running AI/export jobs.

### Recommended MVP Stack

| Layer | Recommended Choice | Rationale |
| --- | --- | --- |
| App Framework | TanStack Start with React and TypeScript | Full-stack React framework built around TanStack Router, server functions, server routes, SSR, and deployable server output without Next.js. |
| Routing | TanStack Router | Type-safe routing, route loaders, search params, pending states, and route-level data boundaries for upload, story input, editor, preview, and export flows. |
| Server State | TanStack Query | Handles project data, upload state, generation status, mutations, caching, refetching, and optimistic UI. |
| Forms | TanStack Form | Useful for project setup, per-image story notes, tone selection, checkout forms, and validation-heavy flows. |
| Tables/Grids | TanStack Table where needed | Useful later for vendor dashboards, project lists, export history, and admin views. |
| UI | Tailwind CSS plus a lightweight component system | Fast iteration, responsive layouts, and low design overhead. |
| Backend | TanStack Start server functions and server routes | Keeps the product full-stack while preserving explicit server boundaries for auth, database, storage, AI calls, and payments. |
| API Contract | Server functions for app-internal actions; REST endpoints for webhooks and future external integrations | Keeps product development fast while leaving room for vendor and integration APIs later. |
| Database | Postgres via Supabase | Good relational fit for users, projects, photos, story notes, pages, exports, and payments. |
| Auth | Supabase Auth | Reduces auth implementation time and works well with Postgres access control. |
| File Storage | Supabase Storage or S3-compatible storage | Stores uploaded images and generated exports separately from app and database code. |
| AI | Vision model plus LLM | Vision model describes image context; LLM rewrites notes, creates transitions, and connects the full story. |
| Background Jobs | BullMQ with Redis, or a managed queue | Needed for long-running image analysis, story generation, and PDF export. Keeps slow work out of request handlers. |
| PDF Export | HTML-to-PDF renderer such as Playwright or Puppeteer | Lets the app reuse web storybook layouts for export. |
| Payments | Stripe | Supports paid PDF exports, one-time purchases, and future vendor subscriptions. |
| Deployment | TanStack Start runtime host plus separate worker host | App can deploy to a supported Node/edge-capable host such as Netlify, Cloudflare, Railway, or similar. Worker can deploy separately on Railway, Fly.io, Render, or a cloud container service. |
| Analytics | PostHog, Plausible, or lightweight event tracking | Tracks activation, story note completion, generation, preview, and export conversion. |
| Error Monitoring | Sentry or platform logs | Helps catch upload, generation, export, and payment failures. |

### Service Architecture

- `app`: TanStack Start full-stack app for upload, story input, editor, preview, checkout, server functions, and webhook routes.
- `worker`: Background worker for image analysis, AI story generation, thumbnail processing, and PDF export.
- `db`: Supabase Postgres for relational product data.
- `storage`: Supabase Storage or S3-compatible storage for images, thumbnails, and exported PDFs.
- `queue`: Redis/BullMQ or managed queue for async work.

### AI Pipeline

1. User uploads and selects images.
2. App stores original images in private storage.
3. App creates thumbnails for faster UI preview.
4. User adds a story note to each selected image.
5. Vision model optionally extracts lightweight image context such as people count, scene, objects, and mood.
6. LLM improves rough notes while preserving user meaning.
7. LLM groups image stories into chapters.
8. LLM generates transitions, opening, closing, and chapter titles.
9. User edits the generated storybook.
10. App exports the final layout to PDF or shareable web view.

### Core Data Models

- User
- Project
- Photo
- PhotoStoryNote
- Storybook
- StorybookPage
- StoryTransition
- Export

### Suggested Data Model Notes

- `Project` represents one wedding or event storybook.
- `Photo` stores image metadata, storage path, upload order, selected status, and optional AI image analysis.
- `PhotoStoryNote` stores the user's original note, AI-polished note, prompt answers, and edit history if needed.
- `Storybook` stores the generated title, tone, structure, and status.
- `StorybookPage` stores page order, image reference, caption, layout choice, and body text.
- `StoryTransition` stores generated connective copy between pages or chapters.
- `Export` stores PDF/share-link status, file path, payment status, and generated timestamp.

### MVP Implementation Principles

- Keep the first version simple: one TanStack Start app, one worker, and managed services.
- Store user memories as first-class data, not just generated output.
- Treat uploaded images as private by default.
- Use background processing for AI generation and PDF export to avoid request timeouts in server functions.
- Generate structured JSON from AI before rendering the storybook.
- Keep prompts versioned so output quality can be compared over time.
- Pin TanStack Start and related packages to specific versions while Start is in release-candidate status.
- Avoid building physical print fulfillment until digital export proves demand.
- Avoid building complex image editing, advanced layouts, or collaboration in the first MVP.

### Alternative Backend Options

- Dedicated Fastify API: useful if server functions become too limiting or external API needs grow.
- Go backend: good if performance, simple binaries, and long-term infrastructure control matter more than full-stack TypeScript sharing.
- Python backend: good if the AI pipeline becomes model-heavy or needs more image-processing libraries.
- Java/Spring backend: solid for enterprise robustness, but likely slower for this MVP unless there is a strong reason.

Recommended default: TanStack Start, TanStack Router, TanStack Query, TanStack Form, Supabase, Redis/BullMQ worker, Stripe, and separate app/worker deployment.

### Future Technical Expansion

- Add vendor workspaces for photographers and planners.
- Add reusable story templates by event type.
- Add richer memory graph features connecting people, places, dates, and events.
- Add print-ready export formats when there is evidence users want physical books.
- Add multi-model routing if vision, writing, and layout generation need different models.

## 16. Launch Plan

### Phase 1: Concierge MVP

- Manually create 3 to 5 sample wedding storybooks.
- Use real or mock wedding photo sets with permission.
- Ask users to provide one short memory per selected image.
- Validate output quality and pricing.

### Phase 2: Self-Serve MVP

- Build upload, per-image story input, story connection, editor, preview, and PDF export.
- Release to a small group of couples and photographers.

### Phase 3: Vendor Pilot

- Add photographer branding.
- Add reusable templates.
- Test bundled pricing with wedding vendors.

## 17. Open Questions

- Should the first product be direct-to-couple or vendor-first?
- What is the minimum number of photos needed for a compelling book?
- Should the storybook be positioned as a digital keepsake, print-ready book, or vendor add-on?
- What price point converts best: $19, $49, $99, or vendor subscription?
- How much per-image detail should the app ask for before generation?
- Should the app require notes for every image or allow some images to be visual-only?
- Should AI ask follow-up questions when a story note is too vague?
- Should guest messages be included in the first version?

## 18. Recommended MVP Decision

Start with a direct-to-couple prototype, but validate vendor distribution early.

The fastest path is:

1. Build a simple upload-to-story-note flow.
2. Let users add one memory per selected image.
3. Use AI to connect the image memories into a polished storybook.
4. Generate a polished digital preview.
5. Charge for PDF export.
6. Use sample outputs to pitch wedding photographers as distribution partners.

## 19. Big Vision

The long-term opportunity is not only wedding books. The bigger product is an AI storytelling system that helps people connect important moments across time.

Possible future directions:

- Life storybooks from childhood, school, career, marriage, family, and legacy photos.
- Family archive storytelling where older relatives explain photos and AI preserves the story.
- Travel journals generated from trip photos and notes.
- Founder or company origin stories generated from milestone images.
- Event storybooks for communities, conferences, and retreats.
- A personal memory graph where images, people, places, dates, and stories are connected.

The durable value is the structured story data behind each image. Photos are the raw material, user memories provide truth, and AI provides narrative structure.
