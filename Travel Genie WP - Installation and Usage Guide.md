# Travel Genie WP - Installation and Usage Guide

## Overview

Travel Genie WP is a powerful WordPress plugin designed specifically for travel bloggers and content creators. It leverages AI technology to generate comprehensive, SEO-optimized travel articles with automatic image generation, keyword optimization, and link management.

## What's Included

Your Travel Genie WP package includes:

- **travel-genie-wp.zip** - Ready-to-install WordPress plugin
- **TravelGenieWP/** - Source code directory
- **Installation Guide** - This document
- **README.md** - GitHub documentation

## System Requirements

Before installing Travel Genie WP, ensure your system meets these requirements:

- **WordPress**: Version 5.0 or higher
- **PHP**: Version 7.4 or higher  
- **Server**: Ability to make outbound HTTP requests (for API calls)
- **Memory**: At least 128MB PHP memory limit recommended

## Required API Keys

To use Travel Genie WP, you'll need:

### 1. OpenRouter API Key (Required)
- **Purpose**: Powers the AI content generation
- **Cost**: Pay-per-use pricing
- **Sign up**: Visit [openrouter.ai](https://openrouter.ai)
- **Setup**: Create account → Dashboard → API Keys → Create new key

### 2. Fal AI API Key (Optional)
- **Purpose**: Generates travel destination images
- **Cost**: Pay-per-image pricing
- **Sign up**: Visit [fal.ai](https://fal.ai)  
- **Setup**: Create account → Dashboard → API Keys → Create new key

## Installation Instructions

### Method 1: WordPress Admin Upload (Recommended)

1. **Download the Plugin**
   - Locate the `travel-genie-wp.zip` file in your package

2. **Access WordPress Admin**
   - Log into your WordPress admin dashboard
   - Navigate to **Plugins → Add New**

3. **Upload Plugin**
   - Click **Upload Plugin** button
   - Choose the `travel-genie-wp.zip` file
   - Click **Install Now**

4. **Activate Plugin**
   - After installation, click **Activate Plugin**
   - You'll see "Travel Generator" appear in your admin menu

### Method 2: FTP Upload

1. **Extract Files**
   - Unzip `travel-genie-wp.zip` to get the `TravelGenieWP` folder

2. **Upload via FTP**
   - Connect to your website via FTP
   - Navigate to `/wp-content/plugins/`
   - Upload the entire `TravelGenieWP` folder
   - Rename it to `travel-genie-wp` if needed

3. **Activate Plugin**
   - Go to WordPress Admin → Plugins
   - Find "Travel Genie WP" and click **Activate**

## Initial Configuration

### Step 1: Configure API Settings

1. **Access Settings**
   - Go to **Travel Generator → Settings** in WordPress admin

2. **OpenRouter API Configuration**
   - Enter your OpenRouter API key in the "OpenRouter API Key" field
   - Select your preferred AI model from the dropdown
   - Click **Refresh List** to load latest available models

3. **Fal AI Configuration (Optional)**
   - Enter your Fal AI API key in the "Fal AI API Key" field
   - The plugin will automatically format the key correctly

4. **Save Settings**
   - Click **Save Settings** to store your configuration

### Step 2: Test Configuration

1. **Verify API Connection**
   - The model dropdown should populate with available options
   - If you see models listed, your OpenRouter key is working

2. **Test Image Generation (Optional)**
   - This will be tested when you create your first article

## Creating Your First Travel Article

### Step 1: Access Article Generator

1. **Navigate to Generator**
   - Go to **Travel Generator → Generate Article**

2. **Review the Interface**
   - You'll see a form with several fields for article customization

### Step 2: Fill Article Details

1. **Blog Post Title**
   - Enter a compelling title (e.g., "Hidden Gems in Paris: A Local's Guide")
   - This becomes your article's H1 tag

2. **Focus Keyword**
   - Enter your primary SEO keyword (e.g., "Paris hidden gems")
   - This keyword will be strategically placed throughout the article

3. **Related Keywords**
   - Add supporting keywords separated by commas
   - Example: "Paris attractions, local experiences, travel tips"

4. **Internal Link (Optional)**
   - URL to one of your existing posts
   - The focus keyword will link to this URL

5. **External Link (Optional)**
   - URL to an external resource
   - Related keywords will link to this URL

6. **Image Generation Options**
   - **Featured Image**: Main article image
   - **Destination Image**: Inserted after "Destination Overview" section
   - **Activities Image**: Inserted after "Cultural Experiences & Activities" section

### Step 3: Generate Article

1. **Submit Form**
   - Click **Generate Travel Article & Save as Draft**
   - The process may take 30-60 seconds

2. **Monitor Progress**
   - You'll see a progress indicator
   - The system will show success/error messages

3. **Review Results**
   - Generated articles are saved as drafts
   - Click the "Edit Post" link to review and customize

## Understanding Generated Content

### Article Structure

Travel Genie WP creates comprehensive articles with these sections:

1. **Introduction** - Engaging hook with focus keyword
2. **Destination Overview** - Essential travel information
3. **Getting There & Around** - Transportation details
4. **Where to Stay** - Accommodation recommendations
5. **Must-See Attractions** - Top destinations and experiences
6. **Off the Beaten Path** - Hidden gems and local secrets
7. **Food & Dining Experiences** - Culinary recommendations
8. **Cultural Experiences & Activities** - Immersive activities
9. **Practical Tips** - Essential travel advice
10. **Sample Itinerary** - Day-by-day planning
11. **Budgeting Guide** - Cost breakdowns
12. **Best Time to Visit** - Seasonal recommendations
13. **What to Avoid** - Common mistakes and tourist traps
14. **Sustainability Considerations** - Responsible travel tips
15. **Conclusion** - Summary and call-to-action
16. **FAQs** - Common traveler questions

### SEO Optimization

- **Focus keyword** appears in title, first paragraph, and throughout content
- **Related keywords** are naturally integrated
- **Internal links** boost your site's SEO
- **External links** add credibility and context
- **Structured content** improves readability and search rankings

## Managing Generated Articles

### Viewing Generated Articles

1. **Access Article List**
   - Go to **Travel Generator → Generated Articles**

2. **Article Management**
   - View all AI-generated articles in one place
   - Sort by date, title, or focus keyword
   - Edit, preview, or delete articles

3. **Article Actions**
   - **Edit**: Modify content in WordPress editor
   - **Preview**: See how article looks on your site
   - **Trash**: Delete unwanted articles

### Editing Generated Content

1. **WordPress Editor**
   - Generated articles open in the standard WordPress editor
   - All content is editable HTML

2. **Customization Options**
   - Add your personal experiences and insights
   - Include additional images or media
   - Adjust tone and style to match your brand
   - Add custom sections or remove unwanted parts

3. **Publishing**
   - Articles are saved as drafts initially
   - Review, edit, and publish when ready

## Advanced Features

### Gutenberg Block

1. **Adding the Block**
   - In any post/page, add the "Travel Generator" block
   - Configure settings directly in the editor

2. **Block Settings**
   - Same options as the main generator form
   - Generate content inline with your existing content

### Shortcode Usage

1. **Basic Shortcode**
   ```
   [travel_generator]
   ```

2. **With Parameters**
   ```
   [travel_generator post_title="Your Title" focus_keyword="your keyword" related_keywords="keyword1, keyword2"]
   ```

3. **Placement**
   - Use in posts, pages, or widgets
   - Content generates where shortcode is placed

## Troubleshooting

### Common Issues

1. **"API Key Not Configured" Error**
   - **Solution**: Verify OpenRouter API key in settings
   - **Check**: Ensure key is copied correctly without extra spaces

2. **"No Models Available" Error**
   - **Solution**: Click "Refresh List" in settings
   - **Check**: Verify API key has sufficient credits

3. **Image Generation Fails**
   - **Solution**: Check Fal AI API key configuration
   - **Alternative**: Disable image generation options

4. **Generated Content is Empty**
   - **Solution**: Try a different AI model
   - **Check**: Ensure focus keyword is provided

5. **Plugin Activation Fails**
   - **Solution**: Check PHP version (7.4+ required)
   - **Check**: Verify WordPress version (5.0+ required)

### Getting Help

1. **Plugin Help Page**
   - Go to **Travel Generator → Help**
   - Expandable sections with detailed guidance

2. **Support Channels**
   - Email: info@tunisiaexplorer.com
   - Website: [tunisiaexplorer.com](https://www.tunisiaexplorer.com)

## Best Practices

### Content Quality

1. **Review Generated Content**
   - Always review and edit AI-generated content
   - Add personal experiences and insights
   - Verify factual accuracy

2. **SEO Optimization**
   - Use specific, long-tail focus keywords
   - Include location-based keywords
   - Add relevant related keywords

3. **Image Strategy**
   - Generate images for visual appeal
   - Add custom photos when possible
   - Optimize image alt text for SEO

### Workflow Efficiency

1. **Batch Generation**
   - Create multiple articles in one session
   - Use consistent keyword strategies
   - Plan content calendar in advance

2. **Content Planning**
   - Research keywords before generation
   - Prepare internal link targets
   - Plan image requirements

## GitHub Repository Setup

### Creating Your Repository

1. **GitHub Account**
   - Create account at [github.com](https://github.com) if needed

2. **New Repository**
   - Click "New repository"
   - Name: `travel-genie-wp`
   - Description: "WordPress plugin for AI-powered travel article generation"
   - Choose public or private

3. **Upload Files**
   - Upload the entire `TravelGenieWP` folder contents
   - The `.gitignore` file is already included

### Repository Structure

```
travel-genie-wp/
├── README.md                 # GitHub documentation
├── .gitignore               # Git ignore rules
├── travel-genie.php         # Main plugin file
├── readme.txt               # WordPress.org readme
├── assets/                  # Plugin icons
├── build/                   # Compiled block files
├── src/                     # Source files
└── languages/               # Translation files
```

## Maintenance and Updates

### Regular Maintenance

1. **API Key Management**
   - Monitor API usage and costs
   - Rotate keys periodically for security

2. **Content Review**
   - Regularly review generated content quality
   - Update prompts if needed

3. **Plugin Updates**
   - Check for updates regularly
   - Backup site before major updates

### Performance Optimization

1. **API Usage**
   - Monitor OpenRouter and Fal AI usage
   - Optimize model selection for cost/quality balance

2. **Image Management**
   - Regularly clean up unused generated images
   - Optimize image sizes for web performance

## Conclusion

Travel Genie WP provides a powerful foundation for creating high-quality travel content efficiently. The AI-generated articles serve as excellent starting points that you can customize and enhance with your personal experiences and insights.

Remember to always review and edit generated content to ensure accuracy and add your unique voice. The plugin is designed to accelerate your content creation process, not replace your expertise and creativity.

For ongoing support and updates, visit [tunisiaexplorer.com](https://www.tunisiaexplorer.com) or contact our support team.

Happy travel blogging!

