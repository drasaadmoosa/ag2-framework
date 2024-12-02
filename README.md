# AG2 Framework Docker Image

This image provides a minimal environment for running the AutoGen 2 (AG2) framework, ag2==0.3.2, a powerful tool for developing large language model (LLM)-based applications.

## What is AG2?

[AutoGen 2 (AG2)](https://github.com/ag2ai/ag2) is an open-source framework designed to simplify the development of LLM-based applications by enabling easy orchestration and communication between multiple agents. AG2 provides an infrastructure for creating autonomous agents that can interact and collaborate, allowing developers to build robust and scalable AI-driven solutions. 

AG2 enables you to:
- Define individual agents with distinct skills and goals.
- Orchestrate the communication between agents using a centralized control mechanism.
- Integrate external APIs, web services, or databases to enhance agent functionality.

With AG2, building complex AI systems becomes more intuitive, thanks to its user-friendly syntax and extendable architecture.

## Key Features of AG2

- **Agent Collaboration**: AG2 allows developers to build LLM-driven agents that can collaborate seamlessly.
- **Modular Design**: The framework supports a modular approach, allowing you to reuse and extend components as needed.
- **Customizable Behaviors**: You can define custom agent behavior and interactions through scripting or code.
- **Interoperability**: Easily integrate external APIs and services to expand the capabilities of agents.

You can find detailed information and tutorials on how to use AG2 in the [official documentation](https://github.com/ag2ai/ag2).

## How to Use This Docker Image

1. **Pull the Image**

   To get started with the AG2 Framework Docker image, pull it from Docker Hub:
   ```bash
   docker pull amotcenter/ag2-framework:latest
   ```

2. **Run a Container**

   You can run a container based on this image using the following command:
   ```bash
   docker run -it amotcenter/ag2-framework:latest
   ```
   This command will start an interactive shell, allowing you to begin using AG2 right away.

3. **Customize the Environment**

   This Docker image provides a minimal AG2 environment. You may wish to mount additional directories or set environment variables for more complex use cases:
   ```bash
   docker run -it -v /path/to/your/data:/workspace/data amotcenter/ag2-framework:latest
   ```
   This mounts a local directory (`/path/to/your/data`) into the container, which can be useful for storing your AG2 scripts or agent data.

## Docker Image Details

- **Image Name**: `amotcenter/ag2-framework`
- **Base Image**: This image uses an official minimal Linux base, with Python and all AG2 dependencies pre-installed.
- **AG2 Version**: The version of AG2 included in this image is kept in sync with the latest stable release from the official AG2 repository.

## Credits

The AutoGen 2 (AG2) framework is developed and maintained by the AG2 open-source community. The full source code, documentation, and contribution guidelines are available in the [official AG2 GitHub repository](https://github.com/ag2ai/ag2). We extend our sincere gratitude to the AG2 authors and contributors for making this powerful tool available to everyone.

## Disclaimer

This Docker image is published by **Dr. Asaad Moosa**. While every effort has been made to ensure the reliability and security of this image, it is provided "as is," without warranty of any kind, express or implied.

**Disclaimer of Liability**: Dr. Asaad Moosa accepts no liability for any damage, loss of data, or issues arising from the use of this Docker image. Users are advised to test and validate the containerized environment according to their own security and compliance requirements.

This image is publicly accessible on Docker Hub, and users are responsible for any modifications they make to the container or its environment.

## License

The AG2 framework and this Docker image are distributed under the terms of the [AG2 License](https://github.com/ag2ai/ag2/blob/main/LICENSE). Please ensure you comply with the licensing terms when using or distributing this image.

## Support

For questions or support regarding AG2, please refer to the official [AG2 GitHub repository](https://github.com/ag2ai/ag2). If you encounter issues specific to this Docker image, you may raise an issue on the image's repository (if available).
