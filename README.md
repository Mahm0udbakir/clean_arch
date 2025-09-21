# Clean Architecture Flutter Project

## Project Structure

```mermaid
graph TD
    A[normalCleanArch] --> B[core]
    A --> C[features]
    A --> D[lib]

    B --> B1[constants]
    B --> B2[di]
    B --> B3[error]
    B --> B4[routes]
    B --> B5["shared<br/>models, widgets"]
    B --> B6[utils]

    C --> C1["feature_1<br/>data, domain, presentation"]
    C --> C2["feature_2<br/>data: api, mapper, models, repo_impl<br/>domain: entities, repo, use_cases<br/>presentation: cubit, screens"]

    D --> D1[lib]

    classDef core fill:#ADD8E6,stroke:#000000,stroke-width:1px;
    classDef features fill:#90EE90,stroke:#000000,stroke-width:1px;
    classDef lib fill:#D3D3D3,stroke:#000000,stroke-width:1px;
    class A,B,B1,B2,B3,B4,B5,B6 core;
    class C,C1,C2 features;
    class D,D1 lib;
```

This diagram illustrates the clean architecture of the `normalCleanArch` project, organized into `core`, `features`, and `lib` directories. The `features` directory includes modular components like `feature_1` and `feature_2`, each adhering to clean architecture layers.

## Support the Project

If you find this project helpful, consider supporting it:

[![Buy me a coffee](https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=your-username&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=FF0000)](https://buymeacoffee.com/your-username)