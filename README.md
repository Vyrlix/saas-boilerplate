[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/CyberCowboy404/nuxtgain.svg)](https://github.com/CyberCowboy404/nuxtgain/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/CyberCowboy404/nuxtgain.svg)](https://github.com/CyberCowboy404/nuxtgain/network)
[![GitHub issues](https://img.shields.io/github/issues/CyberCowboy404/nuxtgain.svg)](https://github.com/CyberCowboy404/nuxtgain/issues)

# NuxtGain: Production-Ready SaaS Boilerplate for Nuxt + Supabase

## A Developer's Solution to Common Nuxt Challenges

Building complex applications with Nuxt can be challenging, especially when it comes to SaaS projects. How do you handle state management, organize business logic, deal with environment variables, navigate Nuxt context in composables, and follow best practices? NuxtGain aims to simplify this process, offering a solid foundation based on real-world experience.

NuxtGain isn't just a concept. It's the core of [magic-resume.ai](https://magic-resume.ai), an AI-powered resume builder for developers that's currently generating revenue in production. I'm now opening up this tried and tested setup to the community.

### Why Choose NuxtGain?

- **Production-Tested**: Actively powers a profitable SaaS application.
- **Comprehensive SaaS Setup**: Includes common SaaS features and integrations.
- **Accelerate Development**: Reduces setup time for new Nuxt projects.
- **Supabase Integration**: Built with Supabase as the primary database solution.
- **Open Source**: Free for the community to use and improve.

Nuxt may have a smaller ecosystem, compared to the NextJS, but it's powerful. NuxtGain is here to streamline your development process and prove that we can build robust applications. Got ideas to make it better? Jump in and contribute.

Let's make Nuxt gain again!

Ready to start building? Dive into the details below and [join our discord](https://discord.gg/EyRuX26ahN)

## Key Features

### Core Technologies 🚀
- 🔧 Nuxt3 + Supabase integration
- 📘 Fully TypeScript-based
- 🎨 Tailwind CSS + Nuxt UI for styling
- 🔜 Nuxt4 compatible

### Development and Configuration ⚙️
- 🏭 Production-ready Nuxt configurations
- 🧹 ESLint configuration with Vue and Nuxt best practices
- 🧠 Business logic and state management setup
- 🧩 Configured and installed essential popular Nuxt modules

### Authentication and User Management 🔐
- 🔑 Supabase authentication integration
- 🚪 Easy-to-use authentication component
- 📊 Basic database tables for user handling

### Internationalization and SEO 🌍
- 🗣️ i18n configuration for translations
- 🔍 SEO-ready setup

### Payment and Transactions 💳
- 💰 Stripe payment integration
- 📝 Basic payment tables (one-time payments, subscriptions in progress)
- 📧 Transactional emails with Brevo (free up to 300 emails per day)

### Content Management 📚
- 📝 Ready-to-use blog functionality

### UI Components 🎛️
- 🧱 Numerous components for landing pages, payment forms, and modals
- 📮 Feedback forms

### File Handling 📁
- 🖼️ Image upload functionality

### Deployment and DevOps 🚀
- ☸️ Kubernetes deployment configurations
- 🔄 GitHub Actions for container deployment to Kubernetes cluster
- ▲ Vercel deployment configurations
- ⚡ Vercel Edge deployment configurations

### Analytics and Monitoring 📊
- 📈 Analytics-ready setup (PostHog, GA4)

### API and Server-side Features 🖥️
- 🔌 Server endpoints for data handling and application logic
- ⏰ Cron job routes for scheduled tasks (e.g., discount emails, transactional emails)

### Additional SaaS Features 🛠️
- 📄 Basic SaaS page templates

## NuxtGain Quick Start Guide

## 1. Set Up Supabase

1. Initialize Supabase locally:
```
npm run supabase:start
```
This command runs migrations, setting up basic tables, Row Level Security (RLS), indexes, triggers, and functions.

2. Copy the environment variables:
```
cp .env.example .env
```

3. Update the `.env` file with your Supabase keys:
- `NUXT_PUBLIC_SUPABASE_KEY`
- `NUXT_SUPABASE_SERVICE_KEY`

These keys are essential for core SaaS functionalities.

## 2. Configure Authentication

1. Edit `./supabase/config.toml` to set up authentication providers.

Example configuration for Google OAuth:

```toml
[auth.external.google]
enabled = true
client_id = "your_client_id"
secret = "your_secret"
redirect_uri = "http://localhost:54321/auth/v1/callback"
```

**Note:** Never commit OAuth provider secrets to git. Use environment variables for sensitive information.

1. For more details on configuring auth providers, refer to the [Supabase Local Development Guide](https://supabase.com/docs/guides/cli/local-development?queryGroups=access-method&access-method=postgres#use-auth-locally).

## 3. Final Configuration

1. Review and update all other environment variables in the `.env` file to enable full functionality of your app.

## 4. Launch Your App

Run the development server:
```
npm run dev
```

Your NuxtGain app should now be up and running with authentication and user management enabled.

For additional configuration options and advanced features, please refer to our detailed documentation.

# NuxtGain Documentation

## Table of Contents
- [Business Logic Organization](docs/business-logic-organization.md)
- [Contributing](docs/CONTRIBUTING.md)

We're continuously improving our documentation. If you have any questions or suggestions, please [open an issue](https://github.com/https://github.com/CyberCowboy404/nuxtgain/issues) on GitHub repository, or write it in [discord](https://discord.gg/EyRuX26ahN)

# Community and Support

As the creator of NuxtGain, I'm here to help and discuss ideas. Reach out to me through:

- [Discord](https://discord.gg/EyRuX26ahN)
- [X (Twitter)](https://x.com/CyberCowboy404)
- [LinkedIn](https://www.linkedin.com/in/nick-b-92589418b/)

For issues or feature requests, please use [GitHub Issues](https://github.com/your-repo/issues).

Let's build something great together!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

NuxtGain is a battle-tested SaaS boilerplate for Nuxt3...

## Get Involved

Ready to supercharge your Nuxt3 development? Here's how you can get started with NuxtGain:

1. 🚀 **Try It Out**: Clone the repo and start building your next SaaS project.
   ```
   git clone https://github.com/CyberCowboy404/nuxtgain.git
   ```

2. ⭐ **Show Your Support**: If NuxtGain helps you, consider giving it a star on GitHub.

3. 🐛 **Report Issues**: Encountered a bug? [Open an issue](https://github.com/CyberCowboy404/nuxtgain/issues) and help improve NuxtGain.

4. 🤝 **Contribute**: Got ideas or fixes? [Submit a pull request](https://github.com/CyberCowboy404/nuxtgain/pulls) and be part of NuxtGain's growth.

5. 💬 **Spread the Word**: Share NuxtGain with your network and help the community grow.

6. ☕ **Buy Me a Coffee**: If you find NuxtGain valuable, consider [buying me a coffee](https://buymeacoffee.com/cybercowboy404) to support ongoing development.

7. 📄 **Use Magic Resume**: Need a stellar developer resume? Check out [Magic Resume](https://magic-resume.ai), the AI-powered resume builder that NuxtGain powers!

Join us in making Nuxt3 development faster, easier, and more enjoyable!



POr si no funciona instalar docker-desktop

Posible error
El error permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock indica que el usuario actual no tiene los permisos necesarios para interactuar con el daemon de Docker. Esto es bastante común en sistemas que requieren que el usuario esté en el grupo docker para ejecutar comandos sin sudo.

Soluciones para el problema de permisos:
Ejecutar con sudo:

La forma más rápida de solucionar esto temporalmente es ejecutar el comando con sudo. Esto te dará acceso a Docker con privilegios elevados:

bash
Copiar código
sudo npm run supabase:start
Esto te pedirá la contraseña de superusuario y debería resolver el problema de "permission denied" temporalmente.

Agregar tu usuario al grupo docker:

Para que no tengas que usar sudo cada vez que quieras ejecutar comandos de Docker, puedes agregar tu usuario al grupo docker. Esto te permitirá ejecutar comandos de Docker sin permisos de superusuario:

a. Agregar tu usuario al grupo docker:

bash
Copiar código
sudo usermod -aG docker $USER
Esto agrega tu usuario al grupo docker, que tiene permisos para interactuar con el daemon de Docker.

b. Cierra sesión y vuelve a iniciar sesión:

Después de ejecutar el comando anterior, deberás cerrar tu sesión y volver a iniciarla para que los cambios surtan efecto. Alternativamente, puedes ejecutar:

bash
Copiar código
newgrp docker
Esto actualizará el grupo activo de tu sesión sin necesidad de reiniciar.

Verificar que Docker esté en ejecución:

Asegúrate de que Docker esté en ejecución, ya que el daemon debe estar activo para que puedas interactuar con él. Puedes verificarlo con este comando:

bash
Copiar código
sudo systemctl start docker
O en distribuciones más antiguas de Linux que no usen systemd:

bash
Copiar código
sudo service docker start
Verificar los permisos del socket de Docker:

Asegúrate de que el socket de Docker tenga los permisos correctos. Ejecuta el siguiente comando para ver los permisos actuales:

bash
Copiar código
ls -l /var/run/docker.sock
El resultado debería verse algo así:

bash
Copiar código
srw-rw---- 1 root docker 0 Sep 19 12:34 /var/run/docker.sock
Esto significa que el propietario es root, pero el grupo docker tiene permisos de lectura y escritura. Si no ves el grupo docker, puedes cambiar los permisos con estos comandos:

bash
Copiar código
sudo chown root:docker /var/run/docker.sock
sudo chmod 660 /var/run/docker.sock
Instalar Docker Desktop:

El error también menciona que Docker Desktop es un prerrequisito para el desarrollo local. Si no tienes Docker Desktop instalado, sigue la guía oficial para instalarlo en tu sistema. Aquí está el enlace oficial:

Guía oficial de Docker Desktop

Resumen:
Ejecuta npm run supabase:start con sudo para una solución rápida.
Agrega tu usuario al grupo docker para evitar tener que usar sudo en el futuro:
bash
Copiar código
sudo usermod -aG docker $USER
Cierra y vuelve a iniciar sesión o usa newgrp docker para aplicar los cambios.
Asegúrate de que Docker esté corriendo correctamente.
Verifica que Docker Desktop esté instalado si es necesario.
Con estos pasos, deberías poder solucionar el problema de permisos y ejecutar Docker y Supabase correctamente.