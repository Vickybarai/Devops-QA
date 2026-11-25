
1. Tell me about yourself
> “I have completed my Master’s degree in Computer Applications from Wainganga College of Engineering and Management, Nagpur.
> I started with a frontend development internship, where I got the opportunity to deploy an application on the cloud and launch servers. That first-time, high-level exposure to cloud infrastructure sparked my strong interest in Cloud and DevOps, motivating me to switch completely into this domain.
> Following that, I completed an eight-month DevOps Internship at HisanLabs in Pune. There, I gained hands-on experience provisioning and managing AWS infrastructure—including EC2, VPC, S3, IAM, RDS, and EKS—automating deployments using Terraform, containerizing applications with Docker, and monitoring Ubuntu Linux servers using CloudWatch and Datadog.
> Currently, I’m strengthening my practical skills by building end-to-end microservices projects on Kubernetes and automating CI/CD workflows with GitHub Actions and Jenkins. I’m looking for a full-time entry-level Cloud or DevOps Engineer role where I can apply my hands-on experience and grow with an engineering team.”
> 
2. Tell me about your current project
(Note: Keep the focus on your actual projects—Medpharm ERP or Flight Reservation Microservices—rather than an e-commerce app you didn't build).
> “Currently, I’m working on a Flight Reservation Microservices Platform consisting of four core services: Frontend, Flight Search, Booking, and Payment.
> The architecture is containerized using multi-stage Docker builds to keep image sizes lightweight and secure, and it runs on an AWS EKS cluster. To manage external traffic securely, I configured an Nginx Ingress Controller with TLS termination. For automation, I built CI/CD pipelines using GitHub Actions to handle automated builds and deployments whenever code is updated.
> Alongside this, I also worked on Medpharm ERP, a pharmaceutical supply chain platform hosted on AWS across a custom VPC with public and private subnets, S3, CloudFront, Route 53, and MongoDB Atlas, where infrastructure was provisioned via Terraform and monitored using Datadog.”
> 
3. Explain the complete CI/CD flow you built
(Note: Only mention tools you have actually configured—like Git, Docker, ECR, Jenkins/GitHub Actions, and EKS—so you can answer deep-dive questions on every stage).
> “In my recent microservices and ERP deployments, I built an automated CI/CD workflow using Git, Jenkins / GitHub Actions, Docker, Amazon ECR, and EKS:
>  * Source & Trigger: Developers push code changes to a specific branch in GitHub/GitLab, which automatically triggers the pipeline via a webhook.
>  * Build & Test: The pipeline pulls the latest code, installs dependencies, runs unit/build checks, and verifies API endpoints.
>  * Containerization: Once the build passes, it builds a Docker image using a multi-stage Dockerfile and tags it with the unique commit SHA or build number for traceability.
>  * Image Registry: The pipeline authenticates with AWS via IAM and pushes the tagged image to Amazon ECR.
>  * Deployment & Verification: Finally, the pipeline updates the Kubernetes deployment manifests on AWS EKS with the new image tag, performs a rolling update to ensure zero downtime, and verifies that the pods reach a healthy running state.”
> 
4. What were your roles and responsibilities?
> “During my DevOps Internship at HisanLabs, I worked closely with the development and QA teams to streamline application deployments and maintain cloud environments.
> My core responsibilities included:
>  * Infrastructure Provisioning: Setting up and managing AWS resources like EC2 instances, VPCs, Security Groups, S3 buckets, and IAM roles using Terraform with a remote S3 backend.
>  * Containerization & Deployment: Writing Dockerfiles, managing multi-container setups with Docker Compose, and assisting with Kubernetes deployments on EKS.
>  * Server Administration & Support: Managing Ubuntu Linux servers, configuring Nginx reverse proxies, and troubleshooting deployment or environment bottlenecks for developers and QA engineers.
>  * Monitoring: Setting up CloudWatch alarms and Datadog dashboards to track CPU, memory, and disk utilization.”
> 
5. What are your day-to-day responsibilities?
> “My typical day revolved around proactive monitoring and supporting active development releases:
>  * Morning Health Checks: First thing after logging in, I checked emails, Jira tickets, and monitoring dashboards in Datadog and AWS CloudWatch to ensure all servers, databases, and containers were healthy overnight.
>  * Deployment & Pipeline Support: I reviewed failed CI/CD builds, helped developers debug environment or configuration issues on staging servers, and deployed updated builds for QA testing.
>  * Infrastructure & Maintenance: During the day, I worked on assigned Jira tasks—such as writing or updating Terraform modules, adjusting Security Group rules, managing backups, or optimizing server configurations—while coordinating with the team to clarify requirements before pushing changes.”
> 
6. Explain one production issue you handled
(The Load Balancer health check example from your notes is a classic, realistic DevOps scenario—here is how to frame it cleanly using the STAR method).
> “During one of our deployments behind an AWS Application Load Balancer (ALB), the target group kept marking our newly deployed EC2 instances as unhealthy, causing intermittent 502 Bad Gateway errors.
> Investigation: I SSH’d into the Ubuntu server and checked the application logs and local curl responses—the application was actually running fine on its port. However, when I checked the ALB target group health check configuration, I noticed the health check path was hitting a heavy database-connected endpoint, and the application took about 45 seconds to initialize, while the ALB timeout and threshold were set too aggressively.
> Resolution: I worked with the developer to expose a lightweight /health endpoint that checked application readiness without heavy DB queries, and I adjusted the ALB health check grace period and interval settings. Once updated, the instances registered as healthy cleanly, and zero-downtime deployments worked as expected.”
>
> 
