# 8x8 CPaaS Wiki

## Project Purpose
A documentation wiki created by the 8x8 CPaaS Solution Engineering team to educate and demonstrate the various Communication Platform as a Service (CPaaS) APIs available from 8x8. This serves as a companion resource to the official 8x8 developer portal.

## Tech Stack
- Jekyll static site generator (GitHub Pages)
- Markdown documentation
- Obsidian vault structure (`.obsidian` folder present)
- Hosted via GitHub Pages

## Development Setup

**Jekyll Site Configuration:**
- Site config: `_config.yml`
- Main entry: `index.md`
- Documentation: `/docs/` folder organized by topic
- Assets: `/image_assets/` for images and media

**To run locally (if needed):**
```bash
bundle install
bundle exec jekyll serve
```

## Important Notes

### Content Organization
The wiki is organized into several topic areas:
- **Ai Building Blocks** - AI-related API components
- **automation** - Automation workflows
- **basics** - Foundational CPaaS concepts
- **chatapps** - Chat application integration
- **jaas** - Jitsi as a Service
- **q&a** - Frequently asked questions
- **sms** - SMS API documentation
- **tests** - Testing guides
- **tools** - Developer tools
- **verification** - Verification API

### Key Files
- `README.md` - GitHub repository description
- `index.md` - Wiki home page with Jekyll front matter
- `_config.yml` - Jekyll configuration
- `introductionTo8x8Cpaas.md` - Introduction to 8x8 CPaaS
- Official docs: https://developer.8x8.com/

### Notes
- This is a **documentation project**, not a code repository
- Uses Jekyll for static site generation (GitHub Pages compatible)
- Also functions as an Obsidian vault (has `.obsidian` folder)
- Created and maintained by 8x8 CPaaS Solution Engineering team
- Dual-purpose: internal knowledge base (Obsidian) + public wiki (Jekyll)
