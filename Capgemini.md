Capgemini Cloud/DevOps Engineer Interview Experience

This document provides a detailed breakdown of the interview process and questions encountered during the recruitment for a Cloud/DevOps Engineer role (approx. 4.5–5 years of experience).

Round 1: Initial Screening (Telephonic)
Focus: Profile validation, logistics, and basic interest.
Topics discussed: Reasons for seeking a job change, current notice period (crucial for quick onboarding), preferred work location, and validation of core technical skill sets (e.g., Linux, AWS, CI/CD, and specific tools like Harness if applicable).

Round 2: Technical Interview
Focus: Deep dive into technical knowledge, troubleshooting, and hands-on expertise.

1. Question: How do you check system performance and resource usage in Linux?
   Answer: Use commands like `top`, `htop`, or `free` to monitor CPU and memory. Use `iostat` for disk I/O. Familiarity with process monitoring is essential.

2. Question: Can you explain the Linux file system structure?
   Answer: You must understand directories like `/etc` (config), `/var` (logs/data), `/bin` (binaries), and `/home` (users).

3. Question: How do you migrate a monolithic application to AWS EKS?
   Answer: Break the monolith into microservices, containerize the components, configure the Kubernetes cluster, and manage deployments using manifests or Helm charts.

4. Question: What is a Kubernetes 'CrashLoopBackOff' and why does it happen?
   Answer: A state where a pod crashes repeatedly. Causes include missing environment variables, dependency issues, invalid entry point commands, or resource constraints (OOMKills).

5. Question: Can you describe your CI/CD pipeline implementation?
   Answer: Explain the automation workflow from code commit (e.g., GitHub) to build, test, and deployment phases using tools like Jenkins, GitHub Actions, or ArgoCD.

6. Question: What is the difference between hosting a database on EC2 versus using AWS Lambda?
   Answer: EC2 offers full control and requires manual management. Lambda is serverless, stateless, and event-driven with automatic scaling but has execution time limits.

7. Question: How do you handle SSL certificate management?
   Answer: Use AWS Certificate Manager (ACM) to provision, deploy, and renew certificates for load balancers and services.

8. Question: How do you troubleshoot a 502 Bad Gateway error on a server?
   Answer: Verify the backend service status, check the reverse proxy (Nginx/Apache) configuration, and ensure connectivity between the proxy and the upstream application.

Round 3: Technical + Managerial Interview
Focus: Architecture, strategic thinking, daily operations, and behavioral assessment.

1. Question: How do you set up production infrastructure?
   Answer: Discuss the use of Infrastructure as Code (Terraform), implementing high availability, auto-scaling, and secure network design (VPC/Subnets).

2. Question: What are the differences in database strategies for Fintech vs. E-commerce?
   Answer: Fintech emphasizes strict regulatory compliance, governance, and auditing. E-commerce prioritizes high availability, traffic handling, and performance.

3. Question: What are your daily operational tasks as a DevOps Engineer?
   Answer: Beyond CI/CD, focus on server patching, incident resolution, environment maintenance, and proactive cloud cost optimization.

4. Question: Can you describe two complex production incidents you have resolved?
   Answer: Share specific real-world scenarios, describing the symptoms, the troubleshooting steps taken, and the permanent resolution.

5. Question: What are your professional certifications and total experience?
   Answer: This confirms your expertise and aligns your profile with the seniority level of the role.

Round 4: HR & Offer Negotiation
Focus: Salary discussion, document verification, and onboarding formalities.
Discussion: Verification of salary structure (fixed vs. variable), background check documentation (education, previous experience letters, relieving letters, and F&F settlement records).