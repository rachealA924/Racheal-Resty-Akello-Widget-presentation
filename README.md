# FractionallySizedBox Demo

> A Flutter widget that sizes its child as a fraction of the available screen space, making layouts automatically adapt to any screen size.

---

## 📱 Demo Preview

my_flutter_widget/assets/Screenshot.png

---

## 🚀 How to Run

1. Make sure Flutter is installed — run `flutter doctor` to verify.
2. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   cd YOUR_REPO_NAME
   ```
3. Get dependencies:
   ```bash
   flutter pub get
   ```
4. Run the app:
   ```bash
   flutter run
   ```

---

## 🧩 Widget: FractionallySizedBox

`FractionallySizedBox` sizes its child widget relative to the parent's dimensions using factors between 0.0 and 1.0, instead of fixed pixel values. This makes it ideal for building responsive UIs that look consistent across different screen sizes.

Real-world use case: A centered profile card that always takes up 80% of the screen width and 55% of the height — no matter what device it runs on.

---

# ⚙️ Three Key Properties

# 1. `widthFactor`
- *What it is: A multiplier (0.0–1.0) that sets the child's width as a percentage of the parent's width.
- Default: `null` (fills available width)
- In this demo: Set to `0.80` so the card takes up 80% of the screen width.
- Why use it: Prevents your UI from stretching edge-to-edge on wide screens, keeping content readable and visually balanced.
- Try changing it: Set to `0.5` for a narrow card, or `1.0` to fill the screen.

# 2. `heightFactor`
- What it is: A multiplier (0.0–1.0) that sets the child's height as a percentage of the parent's height.
- Default: `null` (fills available height)
- In this demo: Set to `0.55` so the card takes up 55% of the screen height.
- Why use it: Keeps cards and modals from being too tall or too short across phones with different screen sizes.
- Try changing it: Set to `0.9` for a nearly full-screen card, or `0.3` for a compact one.

# 3. `alignment`
- What it is: Controls where the sized box is positioned within its parent.
- Default: `Alignment.center`
- In this demo: Set to `FractionalOffset.center` to place the card in the middle of the screen.
- Why use it: Lets you position the widget anywhere — top, bottom, or center — without manual padding or positioning widgets.
- Try changing it: Use `FractionalOffset.topCenter` to pin the card to the top, or `FractionalOffset.bottomCenter` to push it to the bottom.

---

# Source

Widget catalog reference: [Flutter Docs — FractionallySizedBox](https://api.flutter.dev/flutter/widgets/FractionallySizedBox-class.html)

Code adapted from the official Flutter widget sample with modifications for a real-world profile card use case.
