# ArgoCD for Full-Stack Personal Website

This repository contains GitOps configuration for deploying and managing a full-stack personal website. Images in both environments are automatically updated with [argocd-image-updater](https://github.com/argoproj-labs/argocd-image-updater).

**Production:** [https://vm2.laurimaila.com](https://vm2.laurimaila.com)  
**Development:** [https://vm2-dev.laurimaila.com](https://vm2-dev.laurimaila.com)

## Tech Stack

*   **Client:** Next.js, TypeScript, TailwindCSS
*   **Server:** ASP.NET Core
*   **Database:** PostgreSQL, Entity Framework
*   **CMS:** Directus
*   **Deployment:** K8s, Helm, ArgoCD

## Project Structure

*   `argocd/`: Contains the ArgoCD `Application` custom resources that define the applications to be deployed. It also contains configurations for the image updater and ingress.
*   `charts/`: Holds the Helm charts for the three main components of the application: `backend`, `frontend`, and `postgres`. Charts for frontend and backend use images built in their respective repositories.
