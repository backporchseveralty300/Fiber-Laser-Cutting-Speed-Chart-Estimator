# Contributing to Fiber Laser Cutting Speed Chart

First off, thank you for taking the time to contribute! This utility relies on empirical industrial machining data, and your real-world parameter updates can save engineering hours for laser operator communities globally.

## How to Help

### 1. Suggesting Empirical Data Improvements
If you operate CNC fiber lasers and find that our speed chart rates differ significantly from optimized industry standards (e.g., Bystronic, IPG, Trumpf, or Han's Laser parameters), we want to know!
- Please open an **Issue** outlining the material, thickness, laser power, target speed, gas type, and average cut quality.
- Alternatively, submit a **Pull Request (PR)** modifying the `dataset` array inside the `<script>` section of `index.html`.

### 2. Refining the Estimation Formula
Our estimator utilizes v ≈ k · P / dⁿ. If you have a mathematically superior model for heat-affected zones or power scaling in thick plate laser cutting, feel free to pitch it or suggest adjustable coefficients.

## Submission Workflow

1. **Fork** the repository.
2. Create a feature branch: `git checkout -b feature/refine-brass-6kw`
3. Commit your changes with descriptive messages: `git commit -m "Refine 6kW Brass parameters based on actual production data"`
4. Push to your branch and open a **Pull Request**.

All contributors will be featured in the repository update logs!