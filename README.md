# Fiber Laser Cutting Speed Chart & Estimator

An interactive, responsive, and 100% client-side web utility to determine optimal fiber laser cutting parameters. This tool features a pre-loaded empirical dataset covering laser powers from 1000W to 30000W (1kW to 30kW) for various industrial metals, alongside a non-linear parameter estimator for arbitrary thicknesses.

📺 **Live Demo:** https://heretool.com/fiber-laser-cutting-speed-chart

---

## ✨ Features

- **Empirical Parameter Chart:** Instant access to pre-configured feed rates, assist gas types (O2, N2, Air), and recommended gas pressures (Bar) across 1000W to 30000W setups.
- **Support for Key Industrial Metals:** Out-of-the-box parameters for Carbon Steel (Mild Steel), Stainless Steel, Aluminum, and Brass/Copper.
- **Predictive Velocity Estimator:** Uses a non-linear estimation model (v ≈ k · P / dⁿ) to calculate projected feed rates for target thicknesses not explicitly present in the static dataset.
- **Seamless Unit Conversion:** Toggle instantly between metric (mm/min, m/min) and imperial (inch/min / ipm) speed metrics with immediate UI reflows.
- **Privacy-First:** Zero server calls or external tracking. All data is processed entirely in the browser.

---

## 🔬 Estimation Model Formula

The predictive speed estimator calculates cutting velocity (v) using the following empirical physical relationship:

v ≈ k · P / (dⁿ)

Where:
- v is the predicted feed rate (velocity).
- P represents the selected Laser Source Power in Watts.
- d represents the Target Thickness in millimeters.
- k is an empirical material efficiency coefficient.
- n is a power-law attenuation factor reflecting thermal diffusion constraints across thicker cuts.

---

## 🚀 Quick Start / Deployment

This is a single-file static web application. To run it locally or deploy it:

1. Clone or download this repository.
2. Open `index.html` in any web browser.
3. To host it, simply drag and drop the `index.html` file into static hosting platforms like **GitHub Pages**, **Vercel**, or **Netlify**.

---

## 🤝 Contributing

We welcome contributions to refine our speed dataset and enhance the prediction algorithm! If you run custom settings on industrial lasers (such as IPG, Trumpf, Bystronic, Amada, or Raycus sources) and want to contribute more accurate empirical data points, please read CONTRIBUTING.md.

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.