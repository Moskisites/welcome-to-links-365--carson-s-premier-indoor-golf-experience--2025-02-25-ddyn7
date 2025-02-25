# Links-365 Landing Page Maintenance Guide

This guide will help you maintain and customize the Links-365 indoor golf landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Location: Inside the nav element -->
<a href="#" class="text-2xl font-bold">Links-365</a> <!-- Company name -->
```
To update the company name, modify the text between the `<a>` tags.

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-8 leading-tight">
    Welcome to Links-365: Carson's Premier Indoor Golf Experience!
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">
    Experience golf like never before with state-of-the-art technology and premium amenities.
</p>
```
Update the main headline and subheading by changing the text within these elements.

#### Features Section
Each feature card follows this structure:
```html
<div class="bg-gray-900 rounded-xl p-8">
    <h3 class="text-xl font-semibold mb-4">Golf Simulators</h3>
    <!-- Change feature title above -->
    <p class="text-gray-400">Experience realistic golf gameplay...</p>
    <!-- Change feature description above -->
</div>
```

### Tailwind CSS Modifications

#### Understanding Key Classes
- Background colors: `bg-gray-900`, `bg-gray-800`
- Text colors: `text-white`, `text-gray-300`, `text-gray-400`
- Spacing: `p-8` (padding), `mb-4` (margin-bottom)
- Responsive design: `md:text-5xl` (applies at medium screens)

#### Common Customizations
To change background color:
```html
<!-- Original -->
<div class="bg-gray-900">

<!-- Example modification for darker background -->
<div class="bg-gray-950">
```

To adjust text size:
```html
<!-- Original -->
<h3 class="text-xl">

<!-- Make text larger -->
<h3 class="text-2xl">
```

## 2. Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update internal links:
1. Locate the section ID you want to link to
2. Update the `href` attribute with `#` followed by the section ID
3. Example: `<a href="#new-section">New Section</a>`

### External Links
The booking link appears in multiple locations:
```html
<a href="https://links365.moskisites.online" class="inline-block">Book Your Session</a>
```
To update:
1. Replace the URL in `href` with your new booking system URL
2. Test the link to ensure it opens correctly
3. Update all instances of the booking link throughout the page

## 3. Linking Privacy and Terms Pages

### Current Footer Structure
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
    </ul>
</div>
```

### Adding Privacy Policy Link
```html
<!-- Replace the # with the actual path -->
<a href="privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a>
```

### Adding Terms of Service Link
```html
<!-- Replace the # with the actual path -->
<a href="terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a>
```

## Troubleshooting Tips

1. **Broken Internal Links**
   - Ensure section IDs match exactly with href attributes
   - IDs are case-sensitive
   - Check for extra spaces in IDs

2. **Styling Issues**
   - Keep the existing Tailwind classes when adding new ones
   - Test responsiveness at different screen sizes
   - Use browser inspector to debug styling issues

3. **External Links**
   - Test all external links after updating
   - Ensure URLs include `https://` or `http://`
   - Verify links open in correct target (same or new window)

## Best Practices

1. Always backup the original file before making changes
2. Test all changes in a development environment first
3. Maintain consistent styling across all pages
4. Keep the responsive design intact by preserving media query classes
5. Validate all external links regularly

Need more help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).