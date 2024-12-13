# Server Infrastructures 🐳

In this repository, you will find some applications' docker-compose files to setup them easily. These configurations are designed to help developers and system administrators quickly deploy common development tools and services.

## 🎯 Purpose

The main purpose of this repository is to save your time when you need to use commonly used configurations of software development tools. Instead of spending hours configuring each service from scratch, you can use these pre-configured templates that follow best practices and security guidelines.

    ⚠️Remember: These configurations are starting points - you may need to adjust them based on your specific needs and security requirements.

## 🚀 Available Services

Here is a table, it lists these applications:

| Service App | Version | Network Name | IPv4 |
|---|---|---|---|
| PG Admin | `4:8.14.0` | `gui_network` | `10.255.0.2` |
| Single Postgresql | `17.2-alpine3.20` | `postgresql_network` | `10.1.0.2` |
| Single Mongodb | `8.0.0-ubuntu2204` | `mongo_network` | `10.1.1.2` |
| Single MSSQL | `2022-latest` | `mssql_network` | `10.1.2.2` |
| Single Redis | `7.4.0-v1` | `redis_network` | `10.1.4.2` |

**❗Default password is `Password123!`**

> 🚨 **Important! Default credentials are for development only.**  
> Ensure to update them before deploying in a production environment.

🛫 Usage command sample:

```
docker compose -f .\services\service_name\service_name-network.yml -f .\services\service_name\service_name-docker-compose.yml up -d --build
```

## 🛠️ Contributing

I welcome contributions! If you'd like to add a new service or improve existing configurations:

1. Fork the repository
2. Create a new branch for your feature
3. Add your configuration following the existing pattern
4. Create a pull request with a clear description of your changes

## 💫 Future Plans

I'm continuously working to add more services and improve existing configurations. Some planned additions include:
- Databases
- Monitoring tools
- Message brokers
- CI/CD tools
- Code Analysis tools

## 🤝 Support

If you encounter any issues or have questions:
- Look through existing GitHub issues
- Create a new issue with detailed information about your problem

----
EOF