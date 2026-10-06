# Reflection

This laboratory activity helped me understand why cloud operations engineers need to monitor both the host system and the applications running inside containers. Even when containers appear to be running correctly, the host resources still need to be checked because containers depend on the underlying CPU, memory, and disk resources. If the host runs out of memory or disk space, containers can experience performance problems or stop working even when their individual configuration is correct.

The `docker logs` command is useful when investigating a user's complaint about being unable to log in or access a website. Logs can show HTTP requests, response status codes, errors, and other application activity. For example, during this activity, the Nginx logs showed successful HTTP 200 requests and the intentionally generated 404 request. This type of information can help an engineer determine what happened when a user encountered a problem.

Logs and metrics provide different types of information. Logs provide detailed events and messages about what happened, while metrics provide numerical measurements such as CPU usage, memory usage, and other resource statistics. Both are important because metrics can indicate that a problem exists while logs can provide additional information about the event that caused it.

Enterprise companies monitoring thousands of containers can use centralized monitoring and observability platforms. Tools such as Prometheus can collect metrics from many systems, while Grafana can display those metrics in dashboards. Centralized logging systems can also collect application logs from many containers, making large environments easier to monitor.

This laboratory improved my Linux troubleshooting skills by giving me practical experience with commands such as `free`, `df`, `top`, `docker logs`, and `docker stats`. I learned that effective cloud operations requires continuously observing resources, applications, logs, and metrics rather than waiting until a service completely fails.
