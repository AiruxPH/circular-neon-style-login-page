# Changelog

## February 21, 2026

* **style.css**: Modified `.custom-button` class to use `border-radius: 50px;` to give the login button a circular/pill-shape design.
* **style.css**: Fixed layout so the `.login-form` and `.form-group` elements are correctly centered inside the `.login-form-container`. Absolutely positioned `.login-button` to rest at the bottom edge of the circular container. Restored layout base styles (`body`, `html`, `.root`).
* **index.html & style.css**: Implemented a floating label animation for the login form inputs. Swapped `input` and `label` elements in the HTML structure, and added CSS to position the labels identically to placeholder text inside the inputs. Used the `:focus` and `:not(:placeholder-shown)` pseudo-classes along with adjacent sibling combinators `+` to transition the labels to the upper-left of the input border when correctly prompted.
* **style.css**: Updated `box-shadow` properties for `.login-form-container` and input fields to use `inset` values, creating an "inside out" shadow effect.
* **style.css**: Added a flickering glow animation to the `.login-form-title`. The title rhythmically pulses between the default text color and a neon green (#61ff66) with a text-shadow "glow" effect.
* **Overall Theme Update**: Transitioned the entire UI to a "Cyberpunk/Neon" aesthetic.
    * Changed background to dark gray (#4c4d4e).
    * Implemented extensive hover interactions with neon green (#61ff66) borders and glow effects across the container, title, inputs, and the "round" login button.
    * Refined input styling with dark backgrounds, inset shadows, and floating labels that gain a neon border and shadow on focus.
    * Speed up the title flicker animation and added a scale effect on hover.
* **Smooth Border Glide Animation**: Replaced the choppy border-side color animation on the "Login" button with a sophisticated, fluid "glide" effect. This was achieved using a rotating pseudo-element with a neon green `conic-gradient` that spins behind a masked inner circle.
* **Button Refinements**: Balanced the "Login" text centering by removing legacy padding and added an interaction to pause the border animation upon hovering, enhancing usability and focus.
* **Custom Background Integration**: Implemented a bespoke "Neon Circuit Frame" background for the `.root` container. The asset features glowing `#61ff66` green circuitry lines that radiate from behind the central login form, maintaining the dark `#4c4d4e` base color.
* **Authentication Links**: Added "Forgot Password?" and "Sign Up" links to the login form. Integrated them with the Cyberpunk aesthetic using neon green hover states and glowing text-shadow effects.
* **Password UI Refinements**: 
    - Repositioned "Forgot Password?" link to the bottom-left of the password input field.
    - Isolated the "Forgot Password?" link from the password field's hover effects by moving it out of the `.form-group` and refining its CSS alignment.
    - Added a custom "Show Password" toggle button using FontAwesome inside the password input.
    - Implemented JavaScript logic to toggle password visibility.
    - Added CSS to hide default browser password reveal/clear buttons (Edge/IE) to prevent UI duplication.
* **Mobile Responsiveness**: Implemented media queries to scale the circular login container and its contents for screens smaller than 480px. Ensured font sizes, spacing, and button scaling adjust dynamically to maintain the Cyberpunk aesthetic on mobile devices.
* **Revolving Login Button Refinements**: 
    - Slowed down the orbital animation from 10s to 20s for a more cinematic feel.
    - Updated the interaction so the button continues to revolve even when hovered.
    - Fixed a bug where the orbiting button triggered flickering scrollbars by adding `overflow: hidden` to the main `.root` container.
* **Typography Upgrade**: 
    - Replaced generic fonts with professional futuristic typefaces from Google Fonts.
    - **Orbitron**: Applied to the main title, login button, and curved signature for a bold sci-fi energy.
    - **Rajdhani**: Applied to inputs, labels, and base text for a condensed, high-tech terminal appearance.
    - Adjusted letter-spacing across components to maximize the futuristic aesthetic.
* **Theme Darkening**: Deepened the overall color palette. Switched from mid-grays to deep charcoal (#1a1a1a) and pitch-like black (#121212) to significantly increase the "pop" of the neon green elements.
* **Wandering Background Objects**: Added subtle, semi-transparent geometric shapes (circles, squares, and lines) that drift and rotate slowly across the background. This architectural filling adds depth to the atmosphere without distracting from the login interface.
* **Project Favicon**: Generated and integrated a custom neon green orbital logo as the project favicon, completing the visual branding.
* **Open Source Preparation**: Created a professional `README.md` with feature highlights, quick-start instructions, and credits. Added an MIT `LICENSE` file to facilitate open-source distribution and contributions.
