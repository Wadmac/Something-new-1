# Every Scroll, Something New

An editorial graphic-design portfolio built with React, TypeScript, Vite, Tailwind CSS v4, React Three Fiber, Three.js, Framer Motion, and Lucide.

## The Experience

- A persistent Three.js canvas connects the opening workspace, seven creative stages, interactive project gallery, and completed final drawing board.
- Scroll position controls camera movement, object composition, pencil movement, and progressive artwork. Scrolling upward restores earlier creative states.
- Drag the drawing board with a mouse to adjust its perspective. The project gallery supports category filters, scrolling, previous/next controls, and accessible project dialogs.
- Services, the creative showcase, process stages, and testimonial placeholders are interactive.
- Mobile rendering uses a lower pixel ratio and fewer lighting effects. Artwork loads near the gallery. A photographic, scroll-reactive fallback and CSS 3D gallery remain available without WebGL.
- Reduced-motion preferences, keyboard focus management, form validation, a skip link, and mobile navigation are included.

## Personalize

Edit `src/data.ts` to replace the designer name, email, social URLs, verified project counts, portfolio projects, and service descriptions. Unprovided details are deliberately marked as placeholders. The experience value is the supplied 3+ years; the category count reflects the ten actual services.

The included portfolio projects are clearly labeled self-initiated concept studies. Packaging mockups are AI-generated concept imagery. Testimonials are explicit layout placeholders, not fabricated client endorsements. Replace these with genuine work and approved client quotes before publication.

The document title and description are in `index.html`. Replace the name there when personalizing the site.

## Contact Flow

Phone links call +91 9625422343. WhatsApp links open a conversation with the same number. The form validates a project brief, preserves the draft in this browser, and opens a prefilled WhatsApp message for the visitor to send. It does not silently submit to a server or claim delivery. No email service or backend is configured.

Unconfigured social and email links open a clear placeholder dialog with direct contact alternatives. Enter real URLs in `src/data.ts` to activate them.

## Project Structure

- `src/App.tsx`: navigation, scene lifecycle, project/service dialogs, and shared application state.
- `src/scene-state.ts`: responsive scroll waypoints for the continuous journey.
- `src/components/StudioScene.tsx`: 3D drawing board, tools, camera, lighting, and gallery.
- `src/art.ts`: procedural artwork textures and staged drawing logic.
- `src/components/Sections.tsx`: editorial sections and scroll-driven interactions.
- `src/components/Contact.tsx`: validated project-brief form and local draft handling.
- `src/components/UI.tsx`: magnetic buttons, reveal/tilt animations, counters, and accessible dialogs.
- `src/index.css`: responsive visual system and reduced-motion styles.

Use `npm run dev` for local development and `npm run build` for a production build. The supplied Vite setup produces a single-file application bundle, with artwork in `public/images` copied as static assets.