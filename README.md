# Sydney OS (`sydney_OS`)

**A dual-environment hybrid Web Operating System unifying Windows 11 and iOS inside a single, zero-dependency browser runtime.**

🌐 **Live Demo:** [https://os.sydney-accelerator.site]

---

## Overview

**Sydney OS** is an interactive, browser-based operating system engineered to deliver both desktop (Windows 11) and mobile (iOS) user experiences within a single-page application. Rather than relying on heavy frontend frameworks like React, Vue, or external UI component libraries, the entire system runs on **sydney.js**, a lightweight custom Virtual DOM engine.

Both operating environments share a unified runtime, virtual filesystem, media state, and window compositor—allowing seamless switching between desktop and mobile paradigms without page reloads or state loss.

---

## ⚠️ Build & Source Code Notice

> **Compiled Output Notice:** The JavaScript source files in this repository are **minified, bundled, and compressed build outputs** generated automatically by **Accelerator** (`sydney-accelerator.site`), a custom visual web builder and compiler ecosystem. The production bundle in this repository was not written manually by hand; it is the compiled artifact produced from visual component trees and lexer transformations.

---

## Core Architecture & Highlights

* **2-in-1 Dual OS Runtime:** Switch seamlessly between a full Windows 11 desktop environment and an iOS mobile interface sharing the same underlying state and storage.
* **Custom Virtual DOM (`sydney.js`):** Powered by an ultra-lean custom VDOM runtime (~15 KB gzipped) built from scratch with zero external dependencies.
* **Zero Local Stylesheets:** 100% of component styling is compiled inline directly into the Virtual DOM tree—requiring zero local CSS files and zero render-blocking stylesheets (Google Fonts is loaded asynchronously as the sole external asset).
* **Hardware-Constrained Performance:** Engineered for low memory footprints (typically under 15–20 MB JS heap) and smooth 60 FPS window dragging, stacking, and compositing even on entry-level hardware.

---

## Built-in Applications & Features

Sydney OS ships with a suite of functional native web applications across both environments:

* **Window & Desktop Compositor:** Draggable, stackable windows, taskbar/dock navigation, Start Menu, Control Center, and virtual desktop switching.
* **File Manager:** Interactive virtual filesystem supporting folder navigation and drag-and-drop file interactions.
* **Gallery & Media Player:** Shared media state across both Windows 11 and iOS modes.
* **Camera:** Live browser media stream integration.
* **Browser & Settings:** Simulated web navigation and live system customization (wallpapers, themes, and OS mode switching).
* **Live System Telemetry:** Real-time performance metrics on the landing page displaying cold boot time, active DOM node count, JS heap allocation, and registered component count.

---

## Technical Specifications

| Metric | Specification |
| :--- | :--- |
| **Core Framework** | `sydney.js` (Custom Virtual DOM) |
| **Gzipped Bundle Size** | ~15 KB |
| **External Dependencies** | `0` (Pure Vanilla JS) |
| **Local CSS Files** | `0` (100% compiled inline styles) |
| **Environments** | Windows 11 (Desktop) + iOS (Mobile) |
| **Build Pipeline** | Compiled via **Accelerator** |

---

## Running Locally

Because Sydney OS compiles down to static, zero-dependency browser assets, no `npm install` or build step is required to run the distribution files:
