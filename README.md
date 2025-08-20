# 🍳 Kitchenware Website - Metaobjects Setup Guide

This guide will help you set up all the necessary metaobjects for your professional kitchenware Shopify website, including recipes, blog posts, kitchen tips, and more.

## 📋 Table of Contents

1. [Recipe Metaobject](#-recipe-metaobject)
2. [Blog Post Metaobject](#-blog-post-metaobject)
3. [Kitchen Tips Metaobject](#-kitchen-tips-metaobject)
4. [Product Reviews Metaobject](#-product-reviews-metaobject)
5. [Chef Profiles Metaobject](#-chef-profiles-metaobject)
6. [Setup Instructions](#-setup-instructions)
7. [Page Templates](#-page-templates)
8. [Example Data](#-example-data)

---

## 🍳 Recipe Metaobject

**Purpose:** Store and manage daily recipes with detailed cooking information.

### Metaobject Configuration
- **Name:** Recipe
- **Type:** `recipe`
- **Storefront API Access:** ✅ Enabled
- **Publishable:** ✅ Enabled

### Fields Structure

| Field Key | Field Name | Type | Required | Description |
|-----------|------------|------|----------|-------------|
| `title` | Recipe Title | Single line text | ✅ | Name of the recipe |
| `description` | Description | Multi-line text | ✅ | Brief recipe description |
| `featured_image` | Featured Image | File reference | ✅ | Main recipe photo |
| `category` | Category | Single line text | ❌ | Breakfast, Lunch, Dinner, Dessert, Snacks |
| `prep_time` | Prep Time (minutes) | Number - Integer | ❌ | Preparation time |
| `cooking_time` | Cooking Time (minutes) | Number - Integer | ❌ | Cooking time |
| `servings` | Servings | Number - Integer | ❌ | Number of servings |
| `difficulty` | Difficulty Level | Single line text | ❌ | Easy, Medium, Hard |
| `ingredients` | Ingredients | Rich text | ✅ | Ingredient list (use bullets) |
| `instructions` | Instructions | Rich text | ✅ | Step-by-step instructions (use numbers) |
| `chef_tips` | Chef's Tips | Rich text | ❌ | Professional cooking tips |
| `nutrition_info` | Nutrition Information | Rich text | ❌ | Nutritional facts per serving |
| `related_products` | Related Kitchen Products | List - Product reference | ❌ | Kitchen tools used in recipe |
| `recipe_video` | Recipe Video URL | URL | ❌ | YouTube or Vimeo video link |
| `tags` | Recipe Tags | List - Single line text | ❌ | vegetarian, gluten-free, quick, etc. |
| `featured` | Featured Recipe | Boolean | ❌ | Mark as featured on homepage |
| `published_date` | Published Date | Date | ❌ | Recipe publication date |

---

## 📝 Blog Post Metaobject

**Purpose:** Manage kitchen-related blog content, cooking guides, and articles.

### Metaobject Configuration
- **Name:** Blog Post
- **Type:** `blog_post`
- **Storefront API Access:** ✅ Enabled
- **Publishable:** ✅ Enabled

### Fields Structure

| Field Key | Field Name | Type | Required | Description |
|-----------|------------|------|----------|-------------|
| `title` | Post Title | Single line text | ✅ | Blog post title |
| `excerpt` | Excerpt | Multi-line text | ✅ | Short summary for previews |
| `featured_image` | Featured Image | File reference | ✅ | Main blog post image |
| `content` | Content | Rich text | ✅ | Full blog post content |
| `author` | Author | Single line text | ❌ | Author name |
| `author_image` | Author Image | File reference | ❌ | Author profile photo |
| `category` | Category | Single line text | ❌ | Cooking Tips, Product Reviews, Guides |
| `tags` | Tags | List - Single line text | ❌ | Content tags for filtering |
| `read_time` | Read Time (minutes) | Number - Integer | ❌ | Estimated reading time |
| `featured` | Featured Post | Boolean | ❌ | Show on homepage |
| `published_date` | Published Date | Date | ✅ | Publication date |
| `related_products` | Related Products | List - Product reference | ❌ | Products mentioned in post |
| `related_recipes` | Related Recipes | List - Metaobject reference | ❌ | Link to recipe metaobjects |
| `seo_title` | SEO Title | Single line text | ❌ | Custom SEO title |
| `seo_description` | SEO Description | Multi-line text | ❌ | Meta description |

---

## 💡 Kitchen Tips Metaobject

**Purpose:** Store quick cooking tips and professional advice.

### Metaobject Configuration
- **Name:** Kitchen Tip
- **Type:** `kitchen_tip`
- **Storefront API Access:** ✅ Enabled
- **Publishable:** ✅ Enabled

### Fields Structure

| Field Key | Field Name | Type | Required | Description |
|-----------|------------|------|----------|-------------|
| `title` | Tip Title | Single line text | ✅ | Short tip title |
| `description` | Description | Multi-line text | ✅ | Detailed tip explanation |
| `icon` | Icon | Single line text | ❌ | Emoji or icon (👨‍🍳, 🔥, 🧂) |
| `category` | Category | Single line text | ❌ | Knife Skills, Heat Control, Seasoning |
| `difficulty` | Difficulty | Single line text | ❌ | Beginner, Intermediate, Advanced |
| `pro_tip` | Pro Tip | Multi-line text | ❌ | Additional professional advice |
| `related_products` | Related Products | List - Product reference | ❌ | Tools needed for this tip |
| `featured` | Featured Tip | Boolean | ❌ | Show in featured tips section |

---

## ⭐ Product Reviews Metaobject

**Purpose:** Manage customer reviews and testimonials for products.

### Metaobject Configuration
- **Name:** Product Review
- **Type:** `product_review`
- **Storefront API Access:** ✅ Enabled
- **Publishable:** ✅ Enabled

### Fields Structure

| Field Key | Field Name | Type | Required | Description |
|-----------|------------|------|----------|-------------|
| `customer_name` | Customer Name | Single line text | ✅ | Reviewer's name |
| `customer_image` | Customer Image | File reference | ❌ | Customer photo |
| `product` | Product | Product reference | ✅ | Product being reviewed |
| `rating` | Rating | Number - Integer | ✅ | 1-5 star rating |
| `review_title` | Review Title | Single line text | ✅ | Short review headline |
| `review_content` | Review Content | Multi-line text | ✅ | Full review text |
| `verified_purchase` | Verified Purchase | Boolean | ❌ | Confirmed purchase |
| `review_date` | Review Date | Date | ✅ | When review was written |
| `featured` | Featured Review | Boolean | ❌ | Show in testimonials slider |
| `location` | Customer Location | Single line text | ❌ | City, State/Country |

---

## 👨‍🍳 Chef Profiles Metaobject

**Purpose:** Feature professional chefs and cooking experts.

### Metaobject Configuration
- **Name:** Chef Profile
- **Type:** `chef_profile`
- **Storefront API Access:** ✅ Enabled
- **Publishable:** ✅ Enabled

### Fields Structure

| Field Key | Field Name | Type | Required | Description |
|-----------|------------|------|----------|-------------|
| `name` | Chef Name | Single line text | ✅ | Full name |
| `title` | Professional Title | Single line text | ✅ | Executive Chef, Pastry Chef, etc. |
| `bio` | Biography | Rich text | ✅ | Professional background |
| `profile_image` | Profile Image | File reference | ✅ | Professional headshot |
| `specialties` | Specialties | List - Single line text | ❌ | Italian, Pastry, Molecular, etc. |
| `experience_years` | Years of Experience | Number - Integer | ❌ | Professional experience |
| `restaurant` | Restaurant/Workplace | Single line text | ❌ | Current workplace |
| `awards` | Awards & Recognition | Multi-line text | ❌ | Professional achievements |
| `social_instagram` | Instagram Handle | Single line text | ❌ | @username |
| `social_website` | Website URL | URL | ❌ | Personal/professional website |
| `featured_recipes` | Featured Recipes | List - Metaobject reference | ❌ | Link to chef's recipes |
| `quote` | Signature Quote | Multi-line text | ❌ | Inspirational cooking quote |

---

## 🛠️ Setup Instructions

### Step 1: Access Metaobjects
1. Go to **Shopify Admin**
2. Navigate to **Settings → Custom Data → Metaobjects**
3. Click **"Add definition"**

### Step 2: Create Each Metaobject
For each metaobject above:

1. **Set Basic Info:**
   - Name: [As specified above]
   - Type: [As specified above]
   - ✅ Enable "Storefront API access"
   - ✅ Enable "Publishable" (if available)

2. **Add Fields:**
   - Click "Add field" for each field in the table
   - Set the field key, name, type, and required status
   - Add descriptions for clarity

3. **Save Definition**

### Step 3: Create Content
1. Go to **Content → Metaobjects**
2. Select your metaobject type
3. Click **"Add entry"**
4. Fill in all required fields
5. **Save and Publish**

---

## 📄 Page Templates

Create these pages in **Online Store → Pages:**

| Page Handle | Template | Purpose |
|-------------|----------|---------|
| `recipe` | `page.recipe` | Individual recipe display |
| `all-recipes` | `page.all-recipes` | Recipe listing with filters |
| `blog-post` | `page.blog-post` | Individual blog post display |
| `all-blog-posts` | `page.all-blog-posts` | Blog listing |
| `chef-profile` | `page.chef-profile` | Individual chef profile |
| `all-chefs` | `page.all-chefs` | Chef directory |

---

## 📊 Example Data

### Recipe Example
```
Title: "Perfect Pasta Carbonara"
Category: "Dinner"
Prep Time: 15
Cook Time: 20
Servings: 4
Difficulty: "Medium"
Ingredients:
• 400g spaghetti
• 200g pancetta, diced
• 4 large eggs
• 100g Pecorino Romano cheese, grated
• Black pepper to taste
• Salt for pasta water

Instructions:
1. Bring a large pot of salted water to boil
2. Cook spaghetti according to package directions
3. Meanwhile, cook pancetta until crispy
4. Whisk eggs with cheese and pepper
5. Drain pasta, reserving 1 cup pasta water
6. Toss hot pasta with pancetta and egg mixture
7. Add pasta water as needed for creamy consistency
8. Serve immediately with extra cheese

Chef's Tips: "The key is to work quickly and use the hot pasta to cook the eggs gently. Never let the eggs scramble!"
Tags: ["Italian", "Pasta", "Quick", "Comfort Food"]
```

### Blog Post Example
```
Title: "10 Essential Kitchen Knives Every Home Cook Needs"
Category: "Product Reviews"
Read Time: 8
Author: "Chef Maria Rodriguez"
Content: [Detailed guide about different types of kitchen knives, their uses, and recommendations...]
Tags: ["Knives", "Kitchen Tools", "Buying Guide", "Professional Tips"]
```

### Kitchen Tip Example
```
Title: "Knife Sharpening Basics"
Icon: "🔪"
Category: "Knife Skills"
Difficulty: "Beginner"
Description: "Keep your knives sharp for safer, more efficient cooking. A sharp knife requires less pressure and gives you better control."
Pro Tip: "A sharp knife is actually safer than a dull one because it's less likely to slip!"
```

### Product Review Example
```
Customer Name: "Sarah Johnson"
Product: [Link to specific knife set]
Rating: 5
Review Title: "Amazing Quality - Worth Every Penny!"
Review Content: "I've been using this knife set for 6 months now and it's completely transformed my cooking experience. The knives stay sharp, feel balanced in my hand, and make food prep so much faster."
Location: "Seattle, WA"
Verified Purchase: Yes
Featured: Yes
```

### Chef Profile Example
```
Name: "Chef Marco Antonelli"
Title: "Executive Chef"
Restaurant: "Bella Vista Italian Kitchen"
Experience Years: 15
Specialties: ["Italian", "Pasta", "Mediterranean"]
Bio: "Chef Marco trained in Italy and brings authentic flavors to modern kitchenware. He specializes in traditional Italian techniques using contemporary tools."
Quote: "Great cooking starts with great tools, but it's perfected with passion and technique."
```

---

## 🎯 Usage in Sections

These metaobjects work with the following theme sections:

- **Featured Recipes** → Recipe metaobject
- **Featured Blog** → Blog Post metaobject
- **Kitchen Tips** → Kitchen Tip metaobject
- **Testimonials Slider** → Product Review metaobject
- **Chef Spotlight** → Chef Profile metaobject

### Section Configuration Examples

#### Featured Recipes Section
```liquid
Recipe Source: "Recipe Metaobjects"
Number to Show: 6
Show View All: Yes
Heading: "Featured Recipes"
Subheading: "Discover delicious recipes using our premium kitchenware"
```

#### Kitchen Tips Section
```liquid
Heading: "Expert Kitchen Tips"
Subheading: "Professional cooking techniques and tips"
Tips to Show: 4
Show Featured Only: No
```

---

## 🚀 Content Management Workflow

### Daily Recipe Publishing
1. **Create Recipe Entry**
   - Go to Content → Metaobjects → Recipe
   - Click "Add entry"
   - Fill in all recipe details
   - Upload high-quality food photos
   - Link related kitchen products

2. **Content Guidelines**
   - Use clear, step-by-step instructions
   - Include prep and cook times
   - Add professional chef tips
   - Link to relevant kitchen tools
   - Use appetizing food photography

3. **SEO Optimization**
   - Use descriptive recipe titles
   - Include relevant tags
   - Add nutrition information
   - Link to related products

### Blog Content Strategy
1. **Content Types**
   - Product reviews and comparisons
   - Cooking technique guides
   - Kitchen tool maintenance tips
   - Seasonal recipe collections
   - Chef interviews and profiles

2. **Publishing Schedule**
   - 2-3 blog posts per week
   - 1 new recipe daily
   - Weekly chef tips
   - Monthly product spotlights

---

## 🔧 Technical Notes

### Metaobject Limitations
- Maximum 100 fields per metaobject
- File references support images and videos
- List fields can contain up to 25 items
- Rich text fields support HTML formatting

### Performance Considerations
- Use image optimization for all uploaded photos
- Limit the number of metaobject entries loaded per page
- Implement pagination for large content collections
- Use lazy loading for images in sliders

### SEO Best Practices
- Include meta titles and descriptions
- Use structured data for recipes
- Optimize images with alt text
- Create XML sitemaps for content pages

---

## 🚀 Next Steps

1. **Create all metaobjects** using the structures above
2. **Add sample content** to test functionality
3. **Configure theme sections** to use metaobjects
4. **Set up daily content workflow** for recipes and blog posts
5. **Train team** on content creation process
6. **Monitor performance** and optimize as needed

---

## 📞 Support & Resources

### Shopify Documentation
- [Custom Data Overview](https://help.shopify.com/en/manual/metafields)
- [Metaobjects Guide](https://help.shopify.com/en/manual/custom-data/metaobjects)
- [Liquid Template Language](https://shopify.dev/docs/themes/liquid)

### Content Creation Tools
- **Image Editing:** Canva, Photoshop, GIMP
- **Food Photography:** Natural lighting, clean backgrounds
- **Video Content:** YouTube, Vimeo for recipe videos
- **SEO Tools:** Google Keyword Planner, SEMrush

---

**Happy Cooking! 👨‍🍳**

*This comprehensive metaobject system will transform your kitchenware website into a professional cooking destination with rich, engaging content that drives sales and builds customer loyalty.*
