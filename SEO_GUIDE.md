# SEO Optimization Guide - Gift Palace

This document outlines the SEO enhancements implemented in the Gift Palace Shopify theme.

## Implemented SEO Features

### 1. Structured Data (JSON-LD)

Structured data helps search engines understand your content better and can result in rich snippets in search results.

#### Product Schema (`schema-product.liquid`)
- **Automatically included on**: Product pages
- **Benefits**: Rich product snippets in Google search with price, availability, and ratings
- **Data included**: 
  - Product name, images, description
  - Price and currency
  - Availability status
  - SKU and barcodes (GTIN)
  - Brand information
  - Aggregate ratings (if available)

#### Organization Schema (`schema-organization.liquid`)
- **Automatically included on**: All pages
- **Benefits**: Brand recognition, knowledge panel in Google
- **Data included**:
  - Company name and logo
  - Website URL
  - Contact information
  - Social media profiles

#### Breadcrumb Schema (`schema-breadcrumbs.liquid`)
- **Automatically included on**: Product, collection, page, and blog pages
- **Benefits**: Breadcrumb navigation in search results
- **Data included**: Navigation hierarchy from homepage to current page

### 2. Enhanced Meta Tags

#### Open Graph Tags (Facebook, LinkedIn)
- ✅ Fixed protocol issue (now uses HTTPS)
- ✅ Optimized image dimensions (1200x630px)
- ✅ Added image alt text
- ✅ Product-specific tags (price, availability, condition)

#### Twitter Cards
- ✅ Summary large image card
- ✅ Twitter image tags
- ✅ Image alt text support

### 3. Performance Optimizations

#### Resource Hints
- `preconnect` for CDN and Google Fonts
- `dns-prefetch` for analytics services
- Faster page load times

#### Analytics Placement
- Google Analytics moved to `<head>` for better tracking
- Meta Pixel properly positioned

### 4. SEO Best Practices

✅ **Canonical URLs**: Prevent duplicate content issues  
✅ **Meta Descriptions**: Dynamic descriptions for all page types  
✅ **Title Tags**: Optimized with page type and pagination  
✅ **Mobile Optimization**: Responsive viewport settings  
✅ **Favicon**: Proper favicon implementation  
✅ **Language Tags**: Proper HTML lang attribute  

## How to Verify SEO Implementation

### 1. Google Rich Results Test
Test your product pages:
```
https://search.google.com/test/rich-results
```
Enter your product URL to verify structured data.

### 2. Facebook Sharing Debugger
Test Open Graph tags:
```
https://developers.facebook.com/tools/debug/
```
Enter any page URL to see how it appears when shared.

### 3. Twitter Card Validator
Test Twitter Cards:
```
https://cards-dev.twitter.com/validator
```
Enter your URL to preview Twitter card appearance.

### 4. Google Search Console
Monitor your site's performance:
- Submit your sitemap
- Check for indexing issues
- Monitor search performance
- View structured data reports

### 5. Lighthouse SEO Audit
Run in Chrome DevTools:
1. Open DevTools (F12)
2. Go to "Lighthouse" tab
3. Select "SEO" category
4. Click "Generate report"

## SEO Checklist for Content Editors

When adding products or pages, ensure:

- [ ] **Product Title**: Clear, descriptive, includes key terms (50-60 characters)
- [ ] **Product Description**: Detailed, unique content (minimum 150 words)
- [ ] **Meta Description**: Compelling summary (150-160 characters)
- [ ] **Images**: High quality with descriptive alt text
- [ ] **URL Handle**: Clean, keyword-rich URLs
- [ ] **Product Vendor**: Always fill in brand/vendor name

## Advanced SEO Settings

### Customizing Social Sharing

To customize social media links, go to:
**Theme Settings → Social Media**

Add your profiles for:
- Facebook
- Twitter
- Instagram
- YouTube
- Pinterest

These will be automatically included in the organization schema.

### Google Site Verification

Already configured with verification code:
```
jHzys8zjzeRmtGVUoNDxEEkmJ9kzcYynLX7JeuB4kUk
```

### Analytics Tracking

**Google Analytics**: `G-NBNXJ57532`  
**Meta Pixel**: `6026655854124379`

## Troubleshooting

### Structured Data Not Showing
- Clear your cache
- Wait 24-48 hours for Google to re-crawl
- Verify with Rich Results Test

### Social Sharing Preview Issues
- Use Facebook Debugger to refresh cache
- Ensure images are at least 1200x630px
- Check that page is publicly accessible

### Low Search Rankings
SEO is a long-term strategy. Focus on:
- Quality, unique content
- Regular updates
- Building backlinks
- Improving page speed
- Mobile optimization

## Additional Resources

- [Google Search Central](https://developers.google.com/search)
- [Shopify SEO Guide](https://www.shopify.com/blog/ecommerce-seo-beginners-guide)
- [Schema.org Documentation](https://schema.org/)
- [Open Graph Protocol](https://ogp.me/)

## Support

For questions about this SEO implementation, refer to the code comments in:
- `snippets/schema-product.liquid`
- `snippets/schema-organization.liquid`
- `snippets/schema-breadcrumbs.liquid`
- `snippets/meta-tags.liquid`
- `layout/theme.liquid`
