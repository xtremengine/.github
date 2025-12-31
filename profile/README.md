# Xtreme Labs

Welcome to the **Xtreme Labs** organization, focused on building modern, modular game technology in Rust. Here you'll find projects that combine high-performance ECS, 3D isometric rendering, and AI tools to accelerate game development.

## Projects

### Xtreme Engine

A modular game engine with ECS and 3D isometric rendering.

- **High-performance ECS**: entities with generations, cache-friendly storage, and a system scheduler with configurable stages.

- **WGPU rendering**: Vulkan, DirectX 12, Metal, and WebGPU support, isometric camera, and Egui integration.

- **Physics**: collision shapes (AABB, sphere, OBB), spatial grid, and fast raycasts.

- **AI and Navigation**: A* pathfinding, NavMesh, perception system, and optional inference via ONNX Runtime.

- **Visual Editor**: 3D viewport, entity hierarchy, inspector, asset browser, command history, and Play mode.

- **Optional Scripting**: Python integration via pyo3, with lifecycle callbacks.

### How to try it

```bash
# Clone and compile
git clone https://github.com/xtremengine/xtreme.git
cd xtreme
cargo build

# Run the visual editor
cargo run --example editor
```

To use as a dependency in another project, add to `Cargo.toml`:

```toml
[dependencies]
xtreme-engine = "0.1"
```

See the available examples (`hello_triangle`, `isometric_camera`, `editor`) with `cargo run --example <name>`.

## How to contribute

1. Open an issue or participate in the discussions to align ideas.

2. Fork the repository, create a feature branch (`git checkout -b feature/your-idea`) and submit a PR.

3. Ensure the code passes `cargo fmt`, `cargo clippy --all-features -- -D warnings`, and `cargo test`.

## License

The organization's projects are licensed under MIT. See the `LICENSE` file in each repository for details.

Footer
© 2025 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Community
Docs
Contact
Manage cookies
Do not share my personal information
