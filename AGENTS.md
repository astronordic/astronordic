# Repository guide

- `README.md` is nordic's public GitHub profile. Preserve the existing identity and verified professional details.
- Write profile content in English. Check links and confirm that images, links, and text are suitable for public release. Cite verified public sources.
- Run `git diff --check` and review the rendered README on GitHub. This profile uses Markdown and requires no build or application tests.

## Language

Write repository documentation, GitHub content, and internal code in English. Use Brazilian Portuguese for user-facing website, application, and bot text. Preserve compatibility with existing data, integrations, public commands, and explicit locale options.

## Repository presentation

Keep the README clean and informative. Introduce the project and its audience, then describe a concrete workflow and the features that support it. Use a relevant emoji in the title and each section heading. Finish with a technical section covering the actual stack, entry points, setup or verification commands, and links to deeper guides. Use plain Markdown without banners, badges, or repeated navigation. Give readers enough depth to evaluate and maintain the project from the README itself: explain a representative case, boundaries between components, important data or platform constraints, and what the checks actually verify. Scale the detail to the project and verify names, examples, links, and commands against the source. Keep repository presentation self-contained: omit live product URLs and link to source files, tests, and in-repository references. Document concrete interfaces and failure behavior where the source supports them.

Organize the root README into three level-two chapters: “🧭 Project handbook”, “📚 Field reference”, and “🛠️ Technical details”. Keep project-specific topics as emoji-led subsections. Make the field reference useful on its own with concrete inputs, expected results, alternative outcomes, and a reproducible acceptance case. In the technical chapter, identify the implementing paths, compatibility constraints, verification evidence and limits. Expand coverage as the product grows.
