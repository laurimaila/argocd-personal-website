# ArgoCD for Full-Stack Personal Website

This repository contains GitOps configuration for my full-stack personal website. Images in both environments are automatically updated with [argocd-image-updater](https://github.com/argoproj-labs/argocd-image-updater).

**Production:** [https://prod.laurimaila.com](https://prod.laurimaila.com)
**Development:** [https://dev.laurimaila.com](https://dev.laurimaila.com)
## Tech Stack

*   **Client:** Next.js, TypeScript, TailwindCSS
*   **Server:** ASP.NET Core
*   **Database:** PostgreSQL, Entity Framework
*   **CMS:** Directus
*   **Deployment:** K8s, Helm, ArgoCD

## Project Structure

*   `argocd/`: Contains the ArgoCD `Application` custom resources that define the applications to be deployed. It also contains configurations for the image updater and ingress.
*   `charts/`: Holds the Helm charts for the main components of the application: `backend` and `frontend`. Charts for frontend and backend use images built in their respective repositories.
