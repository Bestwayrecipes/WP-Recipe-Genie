# TunisiaExplorer Travel WP

A powerful WordPress plugin that helps travel bloggers create SEO-optimized travel articles with AI assistance.

## Description

**TunisiaExplorer Travel WP** is a beginner-friendly WordPress plugin designed for travel bloggers and content creators. It generates comprehensive, SEO-optimized travel articles using AI technology, complete with focus keywords, related keywords, internal and external links, and destination images.

## Features

- **AI-Powered Content Generation**: Create comprehensive travel articles using OpenRouter API
- **SEO Optimization**: Built-in focus keyword and related keyword integration
- **Image Generation**: Automatic travel destination image creation using Fal AI
- **Link Management**: Easy internal and external link embedding
- **WordPress Integration**: Seamless integration with WordPress admin interface
- **Gutenberg Block**: Custom block for the new WordPress editor
- **Shortcode Support**: Use `[travel_generator]` shortcode anywhere
- **Multi-Language Ready**: Translation-ready with proper text domains

## Installation

### From ZIP File
1. Download the `travel-genie-wp.zip` file
2. Go to your WordPress admin panel
3. Navigate to **Plugins > Add New > Upload Plugin**
4. Choose the ZIP file and click **Install Now**
5. Activate the plugin

### From GitHub
1. Clone this repository to your WordPress plugins directory:
   ```bash
   git clone https://github.com/yourusername/travel-genie-wp.git /path/to/wordpress/wp-content/plugins/travel-genie-wp
   ```
2. Activate the plugin from your WordPress admin panel

## Configuration

### Required API Keys

1. **OpenRouter API Key**: Required for AI content generation
   - Sign up at [OpenRouter.ai](https://openrouter.ai)
   - Get your API key from the dashboard
   - Enter it in **Travel Generator > Settings**

2. **Fal AI API Key** (Optional): Required for image generation
   - Sign up at [Fal.ai](https://fal.ai)
   - Get your API key from the dashboard
   - Enter it in **Travel Generator > Settings**

### Setup Steps

1. Go to **Travel Generator > Settings** in your WordPress admin
2. Enter your OpenRouter API key
3. Select your preferred AI model
4. (Optional) Enter your Fal AI API key for image generation
5. Save settings

## Usage

### Creating Travel Articles

1. Go to **Travel Generator > Generate Article**
2. Fill in the form:
   - **Blog Post Title**: Your article title (e.g., "Hidden Gems in Paris")
   - **Focus Keyword**: Primary SEO keyword (e.g., "Paris hidden gems")
   - **Related Keywords**: Supporting keywords (comma-separated)
   - **Internal Link**: Link to your own content (optional)
   - **External Link**: Link to external resources (optional)
   - **Image Options**: Choose which images to generate
3. Click **Generate Travel Article & Save as Draft**
4. Edit and publish your generated article

### Using the Gutenberg Block

1. Create a new post or page
2. Add the **Travel Generator** block
3. Configure the block settings
4. Generate content directly in the editor

### Using the Shortcode

Add the shortcode anywhere in your content:

```
[travel_generator post_title="Your Title" focus_keyword="your keyword" related_keywords="keyword1, keyword2"]
```

## File Structure

```
travel-genie-wp/
├── travel-genie.php          # Main plugin file
├── readme.txt                # WordPress.org readme
├── README.md                 # GitHub readme
├── .gitignore               # Git ignore file
├── assets/                  # Plugin assets
│   ├── icon-128x128.png
│   └── icon-256x256.png
├── build/                   # Built Gutenberg block files
│   ├── block.json
│   ├── index.js
│   ├── index.css
│   └── style-index.css
├── src/                     # Source files for Gutenberg block
│   ├── index.js
│   ├── edit.js
│   ├── save.js
│   ├── style.scss
│   └── editor.scss
└── languages/               # Translation files
```

## Requirements

- WordPress 5.0 or higher
- PHP 7.4 or higher
- OpenRouter API key (required)
- Fal AI API key (optional, for image generation)

## Frequently Asked Questions

### How do I get API keys?

- **OpenRouter**: Visit [openrouter.ai](https://openrouter.ai), create an account, and get your API key from the dashboard
- **Fal AI**: Visit [fal.ai](https://fal.ai), create an account, and get your API key from the dashboard

### Can I use the plugin without image generation?

Yes! Image generation is optional. You can uncheck the image generation options when creating articles.

### What AI models are supported?

The plugin supports all models available through OpenRouter, including:
- OpenAI GPT models (GPT-3.5, GPT-4, GPT-4o)
- Anthropic Claude models
- Google Gemini
- Meta Llama models
- Mistral AI models

### Is the plugin translation-ready?

Yes! The plugin is fully translation-ready with proper text domains and can be translated into any language.

## Support

For support and questions:
- Visit [TunisiaExplorer.com](https://www.tunisiaexplorer.com)
- Email: info@tunisiaexplorer.com
- Create an issue on this GitHub repository

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This plugin is licensed under the GPLv2 or later.

## Credits

Developed and maintained by [TunisiaExplorer](https://www.tunisiaexplorer.com) - Smart tools and content automation for travel bloggers and creators.

## Changelog

### 1.0.0
- Initial release
- AI-powered travel article generation
- SEO optimization features
- Image generation with Fal AI
- Gutenberg block and shortcode support
- WordPress admin interface

