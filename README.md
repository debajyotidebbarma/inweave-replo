# inweave-replo
preview - https://0ywqxi-w0.myshopify.com/apps/alchemy/element/preview?elementId=793ff356-a2f5-4104-a370-9f75fec3aeba&storeId=861ff37d-1c5c-4e56-80f4-3723559f76b4
# High Level File Structure

## Page
- **Hero Section**
  - Title and Desc Container
    - Heading: *Unlock the mysteries…*
    - Desc: *Subtext*
    - Button: *Unlock Offer → scroll to Product Section*
  - Background Image

- **Review Section**
  - Review Container
    - Heading: *The Most Innovative Box…*
    - Multi-Slide Carousel
      - Review Slides
        - Review 1
        - Review 2
        - Review 3
        - Review 4
        - Review 5
      - Indicators (dots)
      - Carousel Navigation (arrows)

- **Product Section**
  - Product Container *(Grid → 2 cols desktop, 1 col mobile)*
    - **Thumbnail Carousel (Left)**
      - Thumbnails
      - Product Images
    - **Prod Details Container (Right)**
      - Product Details
        - Badge: *Top Rated*
        - Title + Subtitle: *Dynamic title block*
        - Description
        - Features Container
          - Checklist Item 1
          - Checklist Item 2
          - Checklist Item 3
        - Show Size Container
          - Text: *Selected*
          - Text: *Color state*
          - Text: *Size state*
      - Variant Selectors
        - Color Swatches
          - Red Box
          - Blue Box
          - White Box
        - Size Buttons
          - XS
          - SM
          - M
          - L
          - XL
      - Add To Cart
        - Quantity Selector
          - Minus Button
          - Quantity Text *(bound to state)*
          - Plus Button
        - ATC Button
          - Text: *Add Magic Box to Bag*
          - Price: *Variant > Price*




---

## 🛠 Approach (Step-by-Step)

### 1️⃣ Hero Section
- Full-width background image with **heading, sub-text, and CTA button**.  
- **Unlock Offer button** is linked to the `Product Section` via an **anchor scroll interaction**.  
- Responsive: text centered on mobile, left-aligned on desktop.  

---

### 2️⃣ Review Section
- Section includes heading + **multi-slide carousel**.  
- Carousel built with:  
  - **Review cards** (image, rating, text, reviewer).  
  - **Indicators (dots)** and **navigation arrows**.  
- Responsive: multiple cards on desktop, stacked/scrollable on mobile.  

---

### 3️⃣ Product Section
- Built as a **Grid Container**:  
  - **Desktop** → 2 columns (Left = carousel, Right = details).  
  - **Mobile** → 1 column (stacked).  

#### Left Side → Thumbnail Carousel
- Displays product images.  
- Thumbnails switch the main image when clicked.  
- Background = light gray for contrast.  

#### Right Side → Product Details
- Includes:  
  - Badge (*Top Rated*)  
  - Dynamic title + subtitle  
  - Description text  
  - Checklist features (✓ styled items)  
  - Variant selection:  
    - **Color swatches** (Red, Blue, White → changes state & updates text)  
    - **Size boxes** (XS, SM, M, L, XL → state-driven)  
  - Dynamic **Selected Text** → displays e.g. `Selected Blue XS`.  

---

### 4️⃣ Add To Cart Section
- Custom **Quantity Selector**:  
  - State-driven counter (– / + buttons).  
  - Quantity text bound to `quantity` state.  
- **Add To Cart Button**:  
  - Text updates with product + price.  
  - On click → adds product to cart (via Shopify Buy Box integration or AJAX).  
- Responsive: full-width on mobile, inline layout on desktop.  

---


