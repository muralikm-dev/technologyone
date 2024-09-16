# Technologies Used
- **Java**: The core language for the backend logic.
- **Spring Boot**: A framework that simplifies the development of Java applications.
- **JUnit**: A testing framework for Java.
- **Maven**: A build automation tool used for project management.

## Reasons

- **JUnit**: JUnit is a well-known testing framework for Java that allows for unit testing and ensures the functionality of individual components. JUnit is used in this project to ensure code reliability and maintain high standards of software quality by writing and running automated tests that validate the functionality of the backend services.
    - **Advantages**
        - **Test-Driven Development (TDD)**: JUnit encourages test-driven development, ensuring that bugs are detected early and features work as intended.
        - **Integration with Maven**: It integrates smoothly with Maven, providing automated test execution as part of the build lifecycle.
        - **Clear Feedback Loop**: Provides instant feedback when running tests, helping to improve the code's reliability.

- **Maven**: Maven is a build automation and project management tool that simplifies dependency management and project building.For this project, Maven is used to handle the project's dependencies, build lifecycle, and test execution. It simplifies project setup and maintenance by automating the integration of external libraries and managing project configurations.
    - **Advantages**
        - **Dependency Management**: Maven handles libraries and versioning with ease, automatically downloading dependencies from its repositories and maintaining project consistency.
        - **Standardized Build Process**: With Maven, the build process is standardized across the development team, ensuring consistent builds, packaging, and deployment.
        - **Plugin Support**: Maven has a rich plugin ecosystem, making it easy to add support for testing, reporting, and other tasks.

- **Spring Boot**: For Rapid Development, reduces boiler plates, auto configuration support, it provides embedded servers, deployment is straight forward, there is no external server configuration, dependency management using POMs (Maven). For this project, Spring Boot is used to streamline development by automating much of the configuration work and integrating seamlessly with other components

    - **More Elaboration**
        - **Rapid Development**
            - **Spring Boot**: One of the main advantages of Spring Boot is the emphasis on rapid development. Spring Boot comes with built-in templates, auto-configuration, and a rich ecosystem of plugins. These features allow us to build robust, production-ready applications faster by focusing on business logic rather than setup and configuration.
            - **C#**: ASP.NET Core in the C# ecosystem also emphasizes rapid development with integrated tools and project templates. However, the .NET ecosystem tends to be more closely aligned with Microsoft services.
            - **Plain Java**: With plain Java, everything needs to be manually configured, from web servers to database connectivity. This increases development time, as there’s no auto-configuration or built-in tools like Spring Boot provides.
        - **Reducing Boilerplate Code**
            - **Spring Boot**: By eliminating a significant amount of boilerplate code through auto-configuration, Spring Boot drastically reduces the amount of repetitive code, such as database setup or servlet configuration. It also uses annotations like @RestController and @SpringBootApplication to simplify development.
            - **C#**: C# with ASP.NET Core reduces some boilerplate as well, but it may still require manual configurations and settings. Spring Boot excels in using intelligent defaults, which minimizes the need to override settings unless necessary.
            - **Plain Java**: In plain Java, boilerplate is common. Without Spring’s abstraction, we need to spend more time writing configuration files (e.g., XML) and manually handling infrastructure tasks like transaction management or dependency injection.
        - **Auto-Configuration Support**
            - **Spring Boot**: One of the standout features of Spring Boot is auto-configuration, which automatically configures your application based on the libraries present in your classpath. For instance, when Spring Boot detects an embedded database like H2, it automatically configures the data source, reducing development time.
            - **C#**: ASP.NET Core offers some auto-configuration but not at the same depth as Spring Boot. we still need to configure many aspects manually unless using Microsoft-specific integrations.
            - **Plain Java**: In Java, configuration is entirely manual. You need to explicitly set up each component and service, which increases the likelihood of misconfiguration and development complexity.
        - **Embedded Servers**
            - **Spring Boot**: Spring Boot includes embedded servers like Tomcat, Jetty, or Undertow. This means that your application can run independently without needing an external web server. The embedded server can be started with a simple java -jar command, making it ideal for both development and deployment.
            - **C#**: ASP.NET Core can be self-hosted with Kestrel, which is similar to Spring Boot's embedded server model. However, this is typically preferred when deploying within the Microsoft ecosystem, particularly with Azure.
            - **Plain Java**: In plain Java, you need to configure and manage an external server like Tomcat or JBoss manually. This increases the complexity of development and deployment and adds additional configuration steps.
        - **Straightforward Deployment**
            - **Spring Boot**: Deployment in Spring Boot is simplified. With packaging into a single executable JAR or WAR file that contains all dependencies, Spring Boot applications can be deployed on any platform supporting Java. There's no need for manual server configuration, which minimizes the risk of deployment errors.
            - **C#**: ASP.NET Core offers straightforward deployment, especially when working with Microsoft Azure, but there’s still a heavier reliance on the Windows Server ecosystem (unless using Docker for cross-platform needs).
            - **Plain Java**: In plain Java, deployment is often more complex. You need to package your application and deploy it into an external application server (e.g., Tomcat), requiring manual configuration.
        - **No External Server Configuration**
            - **Spring Boot**: One of the biggest conveniences in Spring Boot is the lack of external server configuration. The application ships with an embedded server, and the need for external servers (e.g., Tomcat) is removed, streamlining the entire development and deployment process.
            - **C#**: Similar to Spring Boot, ASP.NET Core can use Kestrel as a lightweight web server. However, deploying on a non-Windows platform often requires additional configurations (or Docker containers).
            - **Plain Java**: With plain Java, external server configuration is necessary. You need to ensure the application server is correctly set up and running before deploying the application, which can add complexity.
        - **Dependency Management with Maven**
            - **Spring Boot**: Spring Boot uses Maven for dependency management, which simplifies the process of adding libraries and managing versions. Maven’s centralized dependency management makes it easy to add, update, or remove libraries without dealing with version conflicts manually. Spring Boot's Starter dependencies package all essential libraries together to streamline setup.
            - **C#**: In the .NET world, NuGet handles dependency management, which is similar to Maven. It’s a strong system but more tied to the Microsoft ecosystem. While NuGet offers good dependency management, Maven has broader support for a variety of open-source libraries and frameworks.
            - **Plain Java**: Plain Java can use Maven for dependency management as well, but without Spring Boot’s smart starter dependencies, you have to configure everything manually. Dependency conflicts can be more frequent, and we need to manage transitive dependencies themselves.