# externalizingConfig

Instructions: 

In application.yml embedded inside the project, i have used 

spring:
  application:
    name: ExternalizingConfig
  config:
    location: ${MODULE_PROPERTY_CONFIG}
    
    MODULE_PROPERTY_CONFIG is an OS env variable with file path file:///D:/boot/module/config/application.yml
    
    When i launch the app, the property file is not getting fetched, the startup fails because it couldnt find database url as i included spring-data-jpa as dependency
