---
title: "Designing and building the Vercel Ship conference platform"
source: "https://vercel.com/blog/designing-and-building-the-vercel-ship-conference-platform"
author:
  - "[[Genny Dee]]"
  - "[[Daniel Linthwaite]]"
  - "[[Yav Punchev]]"
  - "[[James Clements]]"
published: 2025-06-12
created: 2025-06-26
description: "Here's how we designed and built our Vercel Ship conference platform. We generated 15,000+ images and videos with tools like Flux, Veo 2, Runway, and Ideogram. Then, we moved to v0 for prototyping. See our iterations, examples, tech stack, and more."
tags:
  - "clippings"
---
## Summary
The article details the design and build process for the Vercel Ship 2025 conference platform, aiming for a \\"fluid and fast\\" experience. It covers the evolution of its visual identity, from ferrofluid-inspired 3D visuals (initially causing trypophobia, leading to a softer metallic liquid system) to rapid iteration using generative AI tools like Flux, Veo 2, Runway, and Ideogram (generating over 15,000 assets). The team leveraged v0 for rapid prototyping of site elements like registration and schedules. The article also dives into the technical implementation, simplifying the stack with Next.js, Postgres, and Payload CMS for a unified data source, and optimizing performance with ISR and PPR. It highlights the use of Vercel's own platform features, modular components, and fluid motion interactions built with ray-marching, Motion, and Three.js, while also addressing challenges in local development tooling.

## Key Points
-   **Visual Identity Evolution:** Shifted from magnetic particles (Ship 2024) to ferrofluid-inspired 3D visuals for Ship 2025, then refined to a softer, metallic liquid system due to trypophobia concerns.
-   **Rapid AI-Powered Iteration:** Used generative AI tools (Flux, Google Veo 2, Runway, Ideogram) to generate over 15,000 images and videos for quick prototyping of visual directions.
-   **Prototyping with v0:** Leveraged v0.dev for rapid creation and iteration of core site structures and functionalities, such as registration flows, schedules, and galleries, enabling efficient design-to-code handoff.
-   **Fluid Motion & Interaction:** Implemented interactive fluid visuals using ray-marching for smooth surfaces, simulating light bending, and dynamic interactions, with explorations into ferrofluid displacement and water simulations.
-   **Simplified Tech Stack:** Built on Next.js, backed by a Postgres database, and powered by Payload CMS, unifying content and registrant data into a single source of truth for independent team workflows.
-   **Performance Optimization:** Employed Incremental Static Regeneration (ISR) with on-demand invalidation and Partial Prerendering (PPR) for efficient content delivery.
-   **Dogfooding Vercel Platform:** Utilized Vercel's own features like Sign In with Vercel and integrated the Payload admin panel on the same domain for streamlined development and collaboration.
-   **Modular Component System:** Developed reusable, themeable components using shadcn, Geist, and cva, and integrated React Email for transactional emails, enhancing consistency and accelerating development.
-   **Interactive UI Elements:** Implemented advanced scroll animations using Motion for React and a dynamic sticky header with `mix-blend-mode` for a fluid user experience.

---

https://vercel.com/blog/designing-and-building-the-vercel-ship-conference-platform
# Original Content

[Blog](https://vercel.com/blog)

7 min read

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

It's also a chance to push ourselves to create an experience that builds excitement and reflects the quality we strive for in our products. For Vercel Ship 2025, we wanted that experience to feel *fluid* and *fast*.

This is a look at how we made the conference platform and visuals, from ferrofluid-inspired 3D visuals and generative AI workflows, to modular component systems and more.

[Vercel Ship 2024](https://vercel.com/ship/2024) 's visual direction was magnetic particles. Then, we launched [Fluid compute](https://vercel.com/fluid) and brought motion to the particles. For Ship 2025, we wanted to push things even further.

We explored [ferrofluid](https://en.wikipedia.org/wiki/Ferrofluid), a black magnetic liquid developed by NASA. It felt like the right intersection of motion, magnetism, and something complex under the surface (but simple above).

![[03_resources/attachments/8c0a4bbcc138ccd4308fba2274f8c984_MD5.png]]

A fluid visual identity that subtly nods to our past while pushing into something new.

Generative AI helped us rapidly prototyped ideas and test visual directions.

We bounced between Cinema4D, Figma, and Flux to kickstart the visual identity, spinning up quick mocks that shaped the foundation of this year’s brand.

When we first explored ferrofluid, its structured elegance and responsiveness felt like a perfect fit. But during internal reviews, we found a major issue. The visuals were triggering symptoms of trypophobia, an aversion to clustered bumps or holes. So we decided to pivot.

We explored full-spectrum color, oil-slick vibes, and even a callback to our prism from a previous Next.js Conf. But the visuals started to drift. Too far, too shiny, and too loud.

So we pulled back. We had already trained a model to output consistent lighting, form, and material. That gave us a stable base to evolve without starting over. We softened the shapes and removed the spikes. What we landed on was darker, sleeker, and more suitable. A near-metallic liquid system. Reflective and grounded.

![[03_resources/attachments/f5f311efd7cfbe1b07bc34ecde9d041b_MD5.png]]

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

In total, we generated **over 15,000 images and videos** during the design exploration using tools like Flux, Google Veo 2, Runway, and Ideogram. There was no waiting around for "perfect." Instead, we embraced the momentum, shared in-progress work early, and built on top of each other’s thinking.

For the site and registration flow, we turned to [v0](https://v0.dev/), which helps you quickly create your ideas through simple text prompts. Once the core structure and functionality were mapped in Figma, it made sense to move straight into code.

We prompted key parts of the registration, [schedule](https://v0.dev/chat/vercel-ai-event-schedule-usYe0dLnkve), and [gallery](https://v0.dev/chat/vercel-ai-event-schedule-usYe0dLnkve) interactions directly in v0, aligning to our design system. Because we shipped live prototypes on day one, we could share, gather feedback, and iterate rapidly.

Having this kind of prototyping capability within the Design team was a huge unlock. It saved time and made handoff more efficient. Design Engineering started from real components, not mockups. By the time the they stepped in, the structure, layout, and interactions were already set and ready for their final sprinkle of magic.

While the concept was being shaped, we started experimenting on how users would interact with it on the site. One thing was clear: we wanted some type of fluid.

We began by translating some of the AI concepts into code, aiming to capture the same sense of motion and lighting. We used a ray-marching rendering technique to create a smooth surface without any visible polygons.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/1LsO4lddfKxTSgaUXg72nv/1a77d6eee80177f71396fca87e2f881c/depth.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Try the demo → [ship-25-explorations.vercel.app/depth](https://ship-25-explorations.vercel.app/depth)

We also experimented with a glass prism. Since we were using ray-marching, we could simulate how light bends through transparent materials.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/2hkJiHSjStUNkyXVx5bMl1/b1b8ddee58c6d12e6a34226504c5e453/liquid.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Try the demo → [ship-25-explorations.vercel.app/liquid](https://ship-25-explorations.vercel.app/liquid)

Once we had the shape and rendering process in place, we began layering in interactions.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/4WjZUtjQE5p2MikpxXXzSy/5f66b40ec9b0a399b3ebba5e02d8114b/ferro-tetrahedron.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Try the demo → [ship-25-explorations.vercel.app/ferro-pyramid](https://ship-25-explorations.vercel.app/ferro-pyramid?debugTarget=screen)

We explored simulating ferrofluid by displacing a subdivided mesh.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/LtfgGhCx4hGURRqnsllVK/2bc2aad6c8129db68ac95a5634521ad3/ferro-mesh-2.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Try the demo → [ship-25-explorations.vercel.app/ferro-mesh-2](https://ship-25-explorations.vercel.app/ferro-mesh-2)

This created the effect of fluid particles acting as magnetic fields, pushing the mesh outward.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/3wxrHUvq5Hac0nVNArhxdF/23151a69778f487c6ba12919f1546895/ferro-mesh.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Try the demo → [ship-25-explorations.vercel.app/ferro-mesh](https://ship-25-explorations.vercel.app/ferro-mesh)

That version didn’t quite feel right, so we shifted to simulating more realistic fluids using ray-marching. In one version, two simulations ran in parallel, one for the floor and another for the tetrahedron.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/2UZkEIYjrib9YdYiagjOBb/411f66e429c8e4f89b598a4ed8b29548/water-2.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Try the demo → [ship-25-explorations.vercel.app/water-2](https://ship-25-explorations.vercel.app/water-2)

How does this work? The fluid simulation is calculated in one shader, then passed as input into a ray-marching scene. In this setup, the simulation runs on the large plane, while a smaller plane acts as a "ray-marching portal."

This means the liquid isn’t made from triangles. Instead, we simulate a light ray shooting from the camera through the portal and into the surface.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/ogLtkaX7fipFifsrrYczP/3fd9f85d2f9815a0e798724d7df1a807/light-ray-shooting-from-camera-through-small-plane-into-the-surface.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

After that, we added shading and made the simulation collide with a solid prism at the center.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/7CQgdJ4bkKCVgeb4VcraQE/fe8af016a9de286f418c872a94ad8761/water-triangle.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Try the demo → [ship-25-explorations.vercel.app/water-triangle](https://ship-25-explorations.vercel.app/water-triangle)

Once we adjusted the lighting and interaction, we had our hero.

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/5hcZ9TzbnsaElucVUlRwMq/924764aa9137ec64bf3b086d19932e73/final-hero.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

Conference sites can be deceptively complex. Content needs to be editable on-demand, without deployments. Registration data needs to be queryable. Everything needs to feel fast.

In past years, we supported those needs with a mix of external tools and internal caching layers. It got the job done, but maintaining that balance became increasingly difficult.

To reduce latency, we first tried introducing as a fast, supplementary data layer. It helped with performance in key areas, but introduced new challenges. Duplicated data, extra update steps, limited querying, and a reliance on engineering for edits to high-priority information like promo codes or workshop capacity.

This year, we stepped back and simplified. We built the site as a [Next.js](https://nextjs.org/) app, backed by a , and powered by [Payload](https://payloadcms.com/) as the CMS. With full ownership over the API and database, we could shape the system around how we actually work.

Previously, content lived in one place, registrant data in another, and engineering had their own models. Payload let us unify those concerns into a single source of truth:

- A CMS for editable landing-page content
- A searchable, real-time database of registrants
- A backend that engineering could build against directly, without sync logic or duplicated models

The result was a system where teams could move independently. The Events team could manage capacity, content, and promo codes without engineering involvement. Developers could optimize for performance without waiting on upstream APIs.

This stack gave us more control, but we still had to be deliberate about speed. We used [Incremental Static Regeneration (ISR)](https://vercel.com/blog/isr-a-flexible-way-to-cache-dynamic-content) for CMS-driven pages, with on-demand cache invalidation tied to updates. [Partial Prerendering (PPR)](https://vercel.com/blog/partial-prerendering-with-next-js-creating-a-new-default-rendering-model) let us generate most of the homepage at build time, while keeping elements like CTAs and login states dynamic.

We used the [`use cache` directive](https://nextjs.org/docs/app/api-reference/directives/use-cache) and [cacheLife](https://nextjs.org/docs/app/api-reference/functions/cacheLife) to tune freshness by content type. For example, we kept ticket availability up to date with a short cache lifetime, while allowing lower-churn content to stay cached longer. [after()](https://nextjs.org/docs/app/api-reference/functions/after) handled post-checkout logic like sending confirmation emails and logging registrations without holding up the user flow.

The Payload admin panel lives on the same domain as the Vercel and the Ship site, which made debugging and logging more streamlined. [Sign In with Vercel](https://vercel.com/docs/integrations/sign-in-with-vercel) gives us secure, account-based access without additional setup. Our backend [lives in the monorepo](https://vercel.com/blog/how-vercel-adopted-microfrontends), so we could use shared UI assets, like logos or design tokens, directly in the CMS.

This kept the experience consistent, simplified setup, and made collaboration easier across teams.

To support multiple events each year, we built a library of reusable, themeable components using [shadcn](https://ui.shadcn.com/), [Geist](https://vercel.com/geist/colors), and [cva](https://cva.style/docs). This gave us the flexibility to iterate quickly without sacrificing consistency across properties.

For transactional emails, we used [React Email](https://react.email/) and plugged it directly into our CMS. Marketing could preview and edit content live, with no engineering lift.

These shared systems made it easier for Brand, Engineering, and Marketing to collaborate across surfaces, and helped us move faster while keeping everything on-brand

Managing our own database gave us flexibility, but surfaced some limitations in our local tooling. Standing up Postgres locally, running migrations, and seeding data added overhead when working on UI changes or prototyping features. Seed scripts helped, but the local developer experience isn't where it needs to be.

We’re now focusing on automating more of that setup. Previewing real data in local environments, simplifying schema updates, and improving workflows for dynamic content like Open Graph generation and campaign previews.

On the frontend, we’re continuing to explore how to deliver more visual detail without sacrificing speed or performance. Tools like [Motion](https://motion.dev/) and [Three.js](https://threejs.org/) helped us push this year’s visuals forward.

We wanted the site to move as smoothly as it looked. One standout moment was the **What you can expect** section, built using `useTransform` from [Motion for React](https://motion.dev/). Sticky containers and full-screen sections gave us control over scroll behavior, including a custom zoom effect that took a bit of fun math to get right. v0 helped us prototype the logic quickly and dial in the feel.

Another subtle touch was the sticky header. To make sure it adapted across light and dark sections, we tested several options, including [clip-paths](https://developer.mozilla.org/en-US/docs/Web/CSS/clip-path). We eventually landed on a much simpler solution using [mix-blend-mode](https://developer.mozilla.org/en-US/docs/Web/CSS/mix-blend-mode).

<video src="https://assets.vercel.com/video/upload/vc_auto/contentful/video/e5382hct74si/3MdvUjwLFPEDNrxhxbteOX/e7df67c068250f4589970bcc941263dc/ship-25-scroll-animation-and-sticky-header.mp4"></video>

Our two conferences (Vercel Ship and Next.js Conf) are our chance to show what we've been building, how we're thinking, and cast a vision of where we're going next.

The registration page was just the start. It brought Brand, Engineering, and Marketing together in a way that felt fast, fluid, and collaborative from day one.

We prototyped in code, explored quickly, made a few pivots, and pushed the system forward along the way. Not everything went as expected, but it came together into something we’re proud of.

And we’re just getting started. The full experience is on the way. Keynotes, IRL moments, and everything we’ve been building behind the scenes. If you haven’t already, sign up now and be part of it. We'd love to chat with you there.

And yes, we’re still iterating. Because when you ship, you learn. And when you learn, you ship again.

*Special thanks to Matias Gonzalez Fernandez and the rest of* [*basement.studio*](https://basement.studio/) *for partnering with us to create the Vercel Ship site.*