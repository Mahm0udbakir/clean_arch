# Clean Architecture Flutter Project

<a id="readme-top"></a>

Welcome to Clean Architecture Flutter Project! This Flutter application follows Clean Architecture principles for scalable and maintainable development. I originally explored patterns ad‑hoc, but I’ve since studied Clean Architecture in depth—watching Omar Ahmed’s course and reading Uncle Bob’s Clean Architecture book. I’m now taking those learnings to update this repository myself, aiming for a modular, testable, and loosely coupled codebase that demonstrates best practices end‑to‑end.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [Built With](#built-with)
- [Top Contributors](#top-contributors)
- [Support the Project](#support-the-project)
- [Contact](#contact)

## Installation

To get started with this project, follow these steps:

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/mahmoudbakir_week2_cleanarch.git
   cd mahmoudbakir_week2_cleanarch
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the application**
   ```bash
   flutter run
   ```

## Usage

This project demonstrates Clean Architecture implementation in Flutter with the following structure:

- **Core Layer**: Contains shared utilities, constants, error handling, and dependency injection
- **Features Layer**: Modular features following Clean Architecture principles
- **Presentation Layer**: UI components, screens, and state management using BLoC pattern

## Features

- ✅ **Clean Architecture**: Follows Uncle Bob's Clean Architecture principles
- ✅ **Modular Structure**: Feature-based organization for scalability
- ✅ **State Management**: BLoC pattern for predictable state management
- ✅ **Dependency Injection**: GetIt for service locator pattern
- ✅ **Network Layer**: Dio for HTTP requests with interceptors
- ✅ **Local Storage**: SharedPreferences and Secure Storage
- ✅ **Error Handling**: Comprehensive error handling and user feedback
- ✅ **Navigation**: GoRouter for declarative navigation
- ✅ **Theming**: Consistent theming and styling system

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
    
    C ==> C2(feature_2)

    classDef core fill:#0366d6,stroke:#1f2937,stroke-width:3px,color:#ffffff,font-weight:bold;
    classDef features fill:#28a745,stroke:#1f2937,stroke-width:3px,color:#ffffff,font-weight:bold;
    classDef lib fill:#6f42c1,stroke:#1f2937,stroke-width:3px,color:#ffffff,font-weight:bold;
    class A,B,B1,B2,B3,B4,B5,B6 core;
    class C,C1,C1a,C1a1,C1a2,C1a3,C1a4,C1b,C1b1,C1b2,C1b3,C1c,C1c1,C1c2,C1c2a,C1c2b,C2 features;
```

This diagram illustrates the clean architecture of the `normalCleanArch` project, organized into `core`, `features`, and `lib` directories. The `features` directory includes modular components like `feature_1` and `feature_2`, each adhering to clean architecture layers.

## Contributing

We welcome contributions to this project! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/contributer-feature`)
3. **Commit your changes** (`git commit -m 'Add some contributer feature'`)
4. **Push to the branch** (`git push origin feature/contributer-feature`)
5. **Open a Pull Request**

### Development Guidelines

- Follow Clean Architecture principles
- Write tests for new features
- Update documentation as needed
- Follow the existing code style
- Ensure all tests pass before submitting

## Built With

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins the acknowledgements section. Here are a few examples.

- ![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white) 

### Top contributors:

<a href="https://github.com/Mahm0udbakir/mahmoudbakir_week2_cleanarch/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Mahm0udbakir/mahmoudbakir_week2_cleanarch" alt="contrib.rocks image" />
</a>

## Support the Project

If you find this project helpful, consider supporting it:

[![Buy me a coffee](https://img.buymeacoffee.com/button-api/?text=Buy%20me%20a%20coffee&emoji=☕&slug=mahmoudbakir&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=FF0000)](https://buymeacoffee.com/mahmoudbakir)

## Contact

- **Author**: Mahmoud Bakir
- **Email**: [mahmoud.m.bakir@gmail.com](mailto:mahmoud.m.bakir@gmail.com)
- **GitHub**: [@Mahm0udbakir](https://github.com/Mahm0udbakir)
- **LinkedIn**: [Mahmoud Bakir](https://www.linkedin.com/in/mahm0udbakir/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
