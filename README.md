# Redis Session Java

redis-session-java implement session management for java web application.

## Basic Usage

1. Edit `/etc/hosts` file add redis server host
    
    ```
    127.0.0.1 redis.host.name
    ```

1. Edit `web.xml` file add follow lines

    ```
    <filter>
        <filter-name>sessionFilter</filter-name>
        <filter-class>edu.nwnu.ququzone.session.SessionFilter</filter-class>
    </filter>
    <filter-mapping>
        <filter-name>sessionFilter</filter-name>
        <url-pattern>/*</url-pattern>
    </filter-mapping>
    ```