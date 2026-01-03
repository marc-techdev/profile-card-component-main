# Profile Card Component

My solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). A clean, centered profile card with a beautiful overlapping avatar, stats section, and full background patterns — excellent practice for CSS layout, flexbox, and working with multiple background images!

## Live Demo

[View Live Site](https://marc-techdev.github.io/profile-card-component-main/)

## Built With

- Semantic HTML5 markup
- CSS custom properties (variables) for colors and typography
- Flexbox for centering and stats layout
- Mobile-first workflow (layout stays consistent on larger screens)
- Kumbh Sans font from Google Fonts
- Multiple background images for the decorative top and bottom patterns
- Pure CSS (no JavaScript required)

## Key Features

- Fully centered card on a cyan background with large decorative SVG patterns
- Profile image overlapping the top pattern with a clean white border
- Name, age, and location centered below the avatar
- Subtle light gray divider separating profile info from stats
- Stats section with three evenly spaced columns (Followers, Likes, Photos)
- Responsive design that matches the provided mobile and desktop previews
- Pixel-perfect typography and spacing using rem units

## What I Learned

### Positioning Background Patterns Responsively

The biggest challenge was placing the large top and bottom SVG patterns behind the card without media queries. Solved it cleanly with multiple backgrounds on the body:

```css
body {
  background-image: 
    url('./images/bg-pattern-top.svg'),
    url('./images/bg-pattern-bottom.svg');
  background-repeat: no-repeat, no-repeat;
  background-position: 
    right 48vw bottom 35vh,
    left 48vw top 50vh;
  background-color: var(--dark-cyan);
}