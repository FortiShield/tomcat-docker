```mermaid
graph TD;
    A[my-tomcat-app] --> B[app]
    A --> C[db]
    A --> D[docker-compose.yml]
    A --> E[README.md]
    A --> F[.env]

    B --> B1[Dockerfile]
    B --> B2[your-app.jar]
    B --> B3[mysql-connector-java.jar]
    B --> B4[src]
    B4 --> B4a[main]
    B4a --> B4a1[java]
    B4a1 --> B4a1a[your]
    B4a1a --> B4a1a1[package]
    B4a1a1 --> B4a1a1a[MainClass.java]
    B --> B5[resources]

    C --> C1[init.sql]
