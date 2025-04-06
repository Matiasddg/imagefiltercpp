# ImageFilterCPP: Custom Image Filter for MRTech IFF C++ SDK 🎨

![Image Filter](https://img.shields.io/badge/Image%20Filter-Example-blue.svg) ![C++](https://img.shields.io/badge/Language-C%2B%2B-orange.svg) ![CUDA](https://img.shields.io/badge/Technology-CUDA-green.svg) ![Release](https://img.shields.io/badge/Release-v1.0.0-yellow.svg)

Welcome to the **ImageFilterCPP** repository! This project showcases a custom image filter designed for the MRTech IFF C++ SDK. The filter demonstrates advanced image processing techniques, optimized for performance and low latency, making it suitable for applications in machine vision, video streaming, and more.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Contributing](#contributing)
6. [License](#license)
7. [Contact](#contact)
8. [Releases](#releases)

## Introduction

In the age of digital imaging, the need for efficient image processing solutions is more significant than ever. **ImageFilterCPP** serves as a practical example of how to implement custom image filters using the MRTech IFF C++ SDK. This project leverages the power of CUDA to accelerate image processing tasks, ensuring smooth performance even in demanding scenarios.

## Features

- **Custom Filters**: Create and apply various filters to images.
- **CUDA Acceleration**: Utilize GPU resources for faster processing.
- **Low Latency**: Ideal for real-time applications.
- **Demosaicing**: Convert raw image data from sensors into viewable images.
- **Support for Multiple Formats**: Handle DNG, TIFF, and other image formats.
- **Integration with GenICam**: Streamline camera communication.
- **REST API Support**: Access filters and images over the network.
- **RTSP Streaming**: Stream processed images in real-time.
- **Vulkan Support**: Leverage modern graphics APIs for rendering.

## Installation

To get started with **ImageFilterCPP**, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Matiasddg/imagefiltercpp.git
   cd imagefiltercpp
   ```

2. **Install Dependencies**:
   Ensure you have the following installed:
   - C++ compiler (GCC or Clang)
   - CUDA Toolkit
   - MRTech IFF C++ SDK

3. **Build the Project**:
   Use CMake to configure and build the project:
   ```bash
   mkdir build
   cd build
   cmake ..
   make
   ```

4. **Run the Example**:
   Execute the example application to see the filter in action:
   ```bash
   ./ImageFilterExample
   ```

## Usage

Once installed, you can start using the image filter in your applications. Here’s a simple example of how to apply a filter:

```cpp
#include "ImageFilter.h"

int main() {
    ImageFilter filter;
    filter.loadImage("input.dng");
    filter.applyFilter();
    filter.saveImage("output.tiff");
    return 0;
}
```

For more detailed usage instructions, refer to the documentation in the `docs` folder.

## Contributing

We welcome contributions to **ImageFilterCPP**! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

Please ensure your code follows the project's coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For questions or feedback, please reach out to the project maintainer:

- **Name**: Matias
- **Email**: matias@example.com

## Releases

You can find the latest releases of **ImageFilterCPP** [here](https://github.com/Matiasddg/imagefiltercpp/releases). Download the latest version and follow the installation instructions to get started.

If you encounter any issues or have questions, please check the "Releases" section for updates.

---

Thank you for visiting the **ImageFilterCPP** repository! We hope you find this project useful for your image processing needs. Happy coding!