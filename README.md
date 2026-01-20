# Gift Palace Shopify Theme

This repository contains the local build of the Gift Palace Shopify theme.

## Development

### Prerequisites

- [Node.js](https://nodejs.org/)
- [Shopify CLI](https://shopify.dev/docs/themes/tools/cli)

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/GiftPalace2026/GiftPalace.git
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Working with the theme

- **Serve local preview**:
  ```bash
  npm run shopify:serve
  ```
- **Pull latest changes from Shopify**:
  ```bash
  npm run shopify:pull
  ```
- **Push local changes to Shopify**:
  ```bash
  npm run shopify:push
  ```

## Repository Structure

- `assets/`: Theme assets (CSS, JS, images)
- `layout/`: Layout templates
- `sections/`: Theme sections
- `snippets/`: Theme snippets
- `templates/`: Page templates
- `locales/`: Translation files
- `config/`: Theme configuration
