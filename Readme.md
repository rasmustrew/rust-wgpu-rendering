# WGPU Rendering Exploration (Rust)

This is a small experimental 3D engine written in **Rust** using **wgpu** (the Rust WebGPU implementation).

The project started from the official wgpu tutorial and was then extended and partially restructured to explore engine-level concerns such as explicit command encoding, GPU resource ownership, and scene representation.

---

## Features

- Explicit pipeline and render pass setup using wgpu  
- Basic scene with camera and mesh transforms  
- GPU resource management for buffers, uniforms, and shaders  
- Per-frame command encoding and submission to the GPU queue  
- Integration with an external ECS for scene component management  

---

## ECS Experiment

An early version included a minimal custom ECS implementation to explore data-oriented component storage and system iteration patterns.  

After experimenting with it, this was replaced with a library ECS to improve ergonomics and scalability, while retaining separation between scene data and the renderer.

See commit 64a2a44

---

## Status

This project is an exploratory prototype and is no longer actively developed. It represents an early experiment with modern explicit graphics APIs and engine structuring.