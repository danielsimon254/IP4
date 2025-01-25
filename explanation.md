# 1. Choice of Kubernetes Objects

## Backend

- Deployment: Ensures two replicas of the backend service are always running. This provides high availability.

- Service: A ClusterIP service is used to expose the backend internally to the frontend.

## Frontend

- Deployment: Three replicas are deployed to handle incoming traffic efficiently.

- Service: A LoadBalancer service is used to expose the frontend to the internet.

## Persistent Storage

- A Persistent Volume Claim (PVC) is used for the backend to store any potential stateful data or logs, ensuring data persists even if the pod is restarted.


# 2. Method Used to Expose Pods to Internet Traffic

- The frontend is exposed using a LoadBalancer service, which provides an external IP address to route traffic from the internet to the frontend pods.

# 3. Use of Persistent Storage

A Persistent Volume Claim (PVC) is attached to the backend deployment to store any file-based data or logs. This ensures data is retained even if pods are rescheduled.

# 4. Git Workflow

The project was developed using a well-structured Git workflow:

- Descriptive Commits: Each commit describes the changes made in detail.

- Versioning: Docker images were tagged using semantic versioning for clarity (e.g., v1.0.0).

# 5. Debugging Measures


Logs: Kubernetes logs can be reviewed to troubleshoot issues.


# 6. Good Practices

- Image Tagging: Docker images are tagged with specific versions for easy tracking.

- Resource Limits: CPU and memory limits are set for containers to prevent resource exhaustion.

- Documentation: The repository includes detailed documentation for setup and implementation.