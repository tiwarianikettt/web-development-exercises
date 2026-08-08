# Exercise 08 - CSS Transitions & Animations

## 📌 Topic

CSS Transitions & Animations

## 🎯 Objective

Create a bouncing ball animation using CSS animations.

The ball should move across the container while continuously bouncing vertically.

---

## 📚 Concepts Practiced

- CSS Animations
- `@keyframes`
- Animation Shorthand
- `animation-name`
- `animation-duration`
- `animation-timing-function`
- `animation-iteration-count`
- `position: relative`
- `position: absolute`
- `left` property
- `bottom` property
- `border-radius`
- Combining Multiple Animations

---

## 🛠️ Technologies Used

- HTML5
- CSS3

---

## 💡 How It Works

The ball uses two animations simultaneously:

### `bounceX`

Moves the ball horizontally across the container.

```css
@keyframes bounceX {
    from {
        left: 0;
    }

    to {
        left: calc(100% - 121px);
    }
}
```

### `bounceY`

Moves the ball vertically to create the bouncing effect.

```css
@keyframes bounceY {
    0% {
        bottom: 0;
    }

    50% {
        bottom: 70%;
    }

    100% {
        bottom: 0;
    }
}
```

Both animations are applied to the ball at the same time:

```css
animation: bounceX 2s linear infinite,
           bounceY 0.75s ease-out infinite;
```

This creates a combined two-dimensional movement where the ball travels horizontally while repeatedly bouncing vertically.

---

## 📂 Project Structure

```text
Exercise-08-CSS-Transitions-Animations/
│
├── index.html
├── style.css
└── README.md
```

---

## 🧠 What I Learned

- How `@keyframes` define different stages of an animation.
- How animation percentages such as `0%`, `50%`, and `100%` control an element's movement.
- How `animation-duration` controls how long an animation takes.
- How `animation-timing-function` controls the speed pattern of an animation.
- How `infinite` makes an animation repeat continuously.
- How multiple animations can run on the same element simultaneously.
- How `position: relative` and `position: absolute` can be used to position an animated element inside a container.
- How horizontal and vertical animations can be combined to create 2D movement.

---

## 🚀 Future Improvements

- Add more realistic bounce physics.
- Add rotation while the ball moves.
- Add a shadow that changes during the bounce.
- Make the animation responsive to different screen sizes.
- Add interactive controls using JavaScript.

---

## 📖 Author

**Aniket Tiwari**

Learning Web Development through structured notes, exercises, and projects.