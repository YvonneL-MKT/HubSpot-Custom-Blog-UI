HubSpot Custom Blog UI
AI-assisted HubSpot CMS customization for a responsive, brand-aligned blog listing and post experience.
Overview
This project customized a HubSpot-hosted blog so that it aligned more closely with the brand website instead of looking like a disconnected default CMS experience.
The implementation includes:
a custom HubSpot blog listing template
a custom blog post template
reusable global header and footer partials
responsive desktop/tablet/mobile navigation
consistent post-level UI through a shared blog post template
a newsletter subscription section
a Contact Us conversion CTA
brand-aligned typography, spacing, colors, and buttons
HubSpot-native menu, blog content, blog listing, and form components
Architecture
```text
Blog listing template
├── HubSpot blog-posts module
├── Shared global header
├── Shared global footer
├── Shared stylesheet
├── Newsletter form
└── Contact CTA

Blog post template
├── HubSpot blog-content module
├── Shared global header
├── Shared global footer
├── Shared stylesheet
├── Newsletter form
└── Contact CTA
```
AI-Assisted Development
HubSpot's built-in AI was used as a development accelerator during code generation and iteration.
My role included:
defining the UI and responsive requirements
aligning the blog experience with the existing brand website
specifying listing, article, header, footer, and CTA behavior
validating and refining generated code
testing responsive behavior across desktop, tablet, and mobile
maintaining consistency across blog posts through reusable templates
troubleshooting implementation issues in HubSpot's code editor
AI assistance accelerated implementation, but design decisions, acceptance criteria, QA, and publishing decisions remained human-led.
Technical Notes
The templates preserve HubSpot-native functionality through:
`@hubspot/blog_posts`
`@hubspot/blog_content`
`@hubspot/menu`
`standard_header_includes`
`standard_footer_includes`
HubSpot Forms embed
The public version removes production HubSpot form identifiers and selected direct contact/social details.
Repository Structure
```text
src/
├── templates/
│   ├── asteroom-blog-listing-custom.html
│   └── asteroom-elevate-blog-detail.html
├── partials/
│   ├── asteroom-site-header.html
│   └── asteroom-site-footer.html
└── styles/
    └── asteroom-blog-header-footer.css
```
Portfolio Scope
This repository is a code snapshot and portfolio case study, not a deployable standalone website. The templates depend on HubSpot CMS modules and runtime includes.
Privacy / Configuration
Production HubSpot portal and form identifiers have been replaced with placeholders in the public version. Selected contact and social details have also been neutralized.
Potential Improvements
centralize repeated navigation behavior into one shared script
reduce duplicate inline JavaScript between listing and detail templates
move production form configuration into a more maintainable configuration layer where supported
further simplify CSS overrides and reduce `!important` usage where feasible
add structured cross-device regression testing
