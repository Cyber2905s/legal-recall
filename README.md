# ⚖️ Legal Recall

**Legal Recall** is a comprehensive, AI-powered legal research assistant designed to streamline the workflow of legal professionals, clinics, and law students. By combining secure document upload, advanced vector search, and conversational analysis, users can interrogate complex case laws, statutes, and contracts in moments. 

Our system prioritizes verifiability through a unique "Split-View" interface, ensuring every AI-generated response is directly cited and linked to the source legal document.

## 📐 Software Design

Our system follows a strict **Client-Server architecture** designed for scalability and maintainability. We separated our concerns by decoupling the Next.js frontend presentation layer from the heavy backend AI vectorization logic, ensuring low coupling and high cohesion. For data storage, we utilized a dual-database approach: PostgreSQL handles relational user/session data, while Pinecone manages high-dimensional vector embeddings, optimizing both query speed and semantic accuracy for legal research.

### Architecture Diagram
*(See the `/docs/design/` folder for high-resolution models)*
![Architecture Diagram](./docs/design/architecture.png)

### UI Prototypes
Our user interface focuses on cognitive load reduction by utilizing a split-screen verifiable citation view. Check out our complete Figma UI designs and wireframes in the `/docs/design/` directory.

## 🚀 Technologies and Frameworks

- **Frontend:** Next.js, React, TypeScript, Tailwind CSS
- **Database & ORM:** PostgreSQL (Neon Serverless), Drizzle ORM, Pinecone (Vector DB)
- **Authentication & Storage:** Clerk, UploadThing
- **AI & Data Processing:** OpenAI API (Edge), LangChain / Vector Embeddings
- **Utilities:** Axios, @tanstack/react-query, clsx, tailwind-merge

## 🛠️ Installation & Setup

Follow the steps below to install and run the project locally:

1. **Clone the repository**
   Open your terminal and run the following command:
   ```bash
   git clone [https://github.com/your-username/legal-recall.git](https://github.com/your-username/legal-recall.git)
