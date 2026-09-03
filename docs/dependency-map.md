# Dependency Map

```text
asteroom-blog-listing-custom.html
├── asteroom-blog-header-footer.css
├── asteroom-site-header.html
│   └── @hubspot/menu
├── @hubspot/blog_posts
├── HubSpot Forms embed script
├── asteroom-site-footer.html
├── standard_header_includes
└── standard_footer_includes

asteroom-elevate-blog-detail.html
├── asteroom-blog-header-footer.css
├── asteroom-site-header.html
│   └── @hubspot/menu
├── @hubspot/blog_content
├── HubSpot Forms embed script
├── asteroom-site-footer.html
├── standard_header_includes
└── standard_footer_includes
```

## Shared architecture

The listing and detail templates reuse the same header, footer, stylesheet, subscription pattern, contact CTA, and HubSpot-native content modules. This is the basis for consistent UI behavior across blog pages and posts.
