# Xtreme Labs

Bem-vindo à organização **Xtreme Labs**, focada em construir tecnologia de jogos modular e moderna em Rust. Aqui você encontrará projetos que combinam ECS de alta performance, renderização isométrica 3D e ferramentas de IA para acelerar o desenvolvimento de jogos.

## Projetos

### Xtreme Engine

Uma engine de jogos modular com ECS e renderização isométrica 3D.

- **ECS de alto desempenho**: entidades com gerações, armazenamento cache-friendly e agendador de sistemas com estágios configuráveis.
- **Renderização WGPU**: suporte Vulkan, DirectX 12, Metal e WebGPU, câmera isométrica e integração com Egui.
- **Física**: formas de colisão (AABB, esfera, OBB), grade espacial e raycasts rápidos.
- **IA e Navegação**: pathfinding A*, NavMesh, sistema de percepção e inferência opcional via ONNX Runtime.
- **Editor Visual**: viewport 3D, hierarquia de entidades, inspector, browser de assets, histórico de comandos e modo Play.
- **Scripting opcional**: integração com Python via pyo3, com callbacks de ciclo de vida.

#### Como experimentar

```bash
# Clonar e compilar
git clone https://github.com/your-username/xtreme-engine.git
cd xtreme-engine
cargo build

# Executar o editor visual
cargo run --example editor
```

Para usar como dependência em outro projeto, adicione no `Cargo.toml`:

```toml
[dependencies]
xtreme-engine = "0.1"
```

Consulte os exemplos disponíveis (`hello_triangle`, `isometric_camera`, `editor`) com `cargo run --example <nome>`.

## Como contribuir

1. Abra uma issue ou participe das discussões para alinhar ideias.
2. Faça um fork, crie um branch de feature (`git checkout -b feature/sua-ideia`) e envie um PR.
3. Garanta que o código passa por `cargo fmt`, `cargo clippy --all-features -- -D warnings` e `cargo test`.

## Licença

Os projetos da organização são licenciados sob MIT. Veja o arquivo `LICENSE` em cada repositório para detalhes.
