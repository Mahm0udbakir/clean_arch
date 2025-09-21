# Clean Architecture Flutter Project

## Project Structure

```mermaid
graph TD
    A(normalCleanArch) ==> B(core)
    A ==> C(features)

    B ==> B1(constants)
    B ==> B2(di)
    B ==> B3(error)
    B ==> B4(routes)
    B ==> B5("shared<br/>models, widgets")
    B ==> B6(utils)

    C ==> C1(feature_1)
    C1 ==> C1a(data)
    C1a ==> C1a1(api)
    C1a ==> C1a2(mapper)
    C1a ==> C1a3(models)
    C1a ==> C1a4(repo_impl)
    C1 ==> C1b(domain)
    C1b ==> C1b1(entities)
    C1b ==> C1b2(repo)
    C1b ==> C1b3(use_cases)
    C1 ==> C1c(presentation)
    C1c ==> C1c1(cubit)
    C1c ==> C1c2(screens)
    C1c2 ==> C1c2a(screen_1)
    C1c2 ==> C1c2b(screen_2)

    C ==> C2(feature_2)

    classDef core fill:#FF9A00,stroke:#ED3F27,stroke-width:4px,color:#F6F1E9,font-weight:bold;
    classDef features fill:#FF9A00,stroke:#ED3F27,stroke-width:4px,color:#F6F1E9,font-weight:bold;
    classDef lib fill:#FF9A00,stroke:#ED3F27,stroke-width:4px,color:#F6F1E9,font-weight:bold;
    class A,B,B1,B2,B3,B4,B5,B6 core;
    class C,C1,C1a,C1a1,C1a2,C1a3,C1a4,C1b,C1b1,C1b2,C1b3,C1c,C1c1,C1c2,C1c2a,C1c2b,C2 features;
```

This diagram illustrates the clean architecture of the `normalCleanArch` project, organized into `core`, `features`, and `lib` directories. The `features` directory includes modular components like `feature_1` and `feature_2`, each adhering to clean architecture layers.

## Support the Project

If you find this project helpful, consider supporting it:

[![Buy me a coffee](https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=your-username&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=FF0000)](https://buymeacoffee.com/your-username)