# Ad Demo Simulator

A web-based mobile app simulator for demonstrating MRAID ad creatives in realistic app environments. Perfect for pitching ad formats to partners like SoundCloud.

## Features

- 🎯 **Realistic App UI**: SoundCloud iOS interface simulation
- 📱 **Mobile First**: Responsive design with iPhone X mockup
- 🎨 **Customizable Ads**: Configure title, subtitle, and styling
- 🔗 **Shareable URLs**: Generate links with pre-configured ad parameters
- ✨ **MRAID Support**: Basic MRAID environment mock
- 🎬 **Interactive**: Close button and ad interactions

## Quick Start

1. Clone the repository
2. Open `index.html` in a web browser
3. Customize the ad parameters in the control panel
4. Copy the shareable URL and share with customers

## URL Parameters

The demo supports the following query parameters for sharing:

- `title` - Ad title text
- `subtitle` - Ad subtitle text
- `creative_id` - Creative identifier (e.g., KM-CREA-197599)
- `gradient` - Color gradient preset (default, blue, sunset, mint, berry)

### Example URLs

```
https://yourdomain.com/index.html?title=Premium+Headphones&subtitle=Crystal+Clear+Sound&creative_id=KM-CREA-197599&gradient=sunset
```

## Customization

### Adding New Gradient Presets

Edit the `gradients` object in the JavaScript section to add new color schemes:

```javascript
const gradients = {
    custom: 'linear-gradient(135deg, #color1 0%, #color2 100%)'
};
```

### Embedding Custom MRAID Creative

Replace the placeholder content in the `mraid-creative` div with your actual MRAID HTML:

```html
<div class="mraid-creative" id="mraid-creative">
    <!-- Your MRAID creative HTML here -->
</div>
```

## Deployment

### GitHub Pages

1. Push this repository to GitHub
2. Go to Settings → Pages
3. Set source to `main` branch
4. Access your demo at `https://yourusername.github.io/ad-demo-simulator/`

### Custom Domain

Update the `updateShareUrl()` function to use your custom domain for shareable links.

## Browser Support

- Chrome (recommended)
- Safari
- Firefox
- Edge

Works best on mobile devices and tablets. Desktop view includes iPhone X mockup.

## MRAID Compatibility

This simulator includes a basic MRAID mock implementation with the following methods:

- `getState()` - Returns ad state
- `getMaxSize()` - Returns max ad dimensions
- `getScreenSize()` - Returns device screen size
- `addEventListener()` - Event listener stub
- `removeEventListener()` - Remove listener stub
- `expand()` - Expand ad stub
- `close()` - Close ad (functional)
- `isViewable()` - Returns viewability state

## Use Cases

- **Pitch Sessions**: Show prospective partners how their ads look in your app
- **Ad Network Demos**: Demonstrate format compatibility
- **Creative Testing**: Test different ad variations
- **Customer Presentations**: Share pre-configured demos with stakeholders

## License

MIT

## Contact

Created for demonstrating ad creative implementations in mobile apps.
