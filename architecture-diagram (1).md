# AWS Application Load Balancer Architecture

```
                    Internet
                        |
                        |
               +---------------------+
               |  Application Load   |
               |      Balancer       |
               +---------------------+
                        |
            -----------------------------
            |                           |
      EC2 Instance 1              EC2 Instance 2
     (Apache Installed)           (Apache Installed)
        Server-1                      Server-2
```

## Key Points

- ALB distributes incoming HTTP requests
- If one server becomes unhealthy, traffic is routed to healthy instance
- DNS of ALB is used instead of EC2 public IP
