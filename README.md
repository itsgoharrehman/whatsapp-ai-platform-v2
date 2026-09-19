# whatsapp-ai-platform-v2

A multi-tenant WhatsApp AI automation platform supporting independent WhatsApp session management, Cloudflare edge routing, Node.js Baileys workers, user dashboards, and Super Admin oversight controls.

## Architecture and Stack

* **Core Runtime**: Node.js (v18+), TypeScript
* **Protocol**: `@whiskeysockets/baileys` Multi-Device Architecture
* **Edge Proxy**: Cloudflare Workers
* **Database & Auth**: PostgreSQL / Supabase
* **Frontend UI**: Responsive Admin and User Management Dashboard

## Key Features

* **Multi-Tenant Session Isolation**: Independent WhatsApp auth folders and connection lifecycles per tenant.
* **AI Message Pipeline**: Natural language understanding, automated response routing, and intent classification.
* **Admin Supervision**: Super Admin dashboard displaying active sessions, throughput metrics, and rate limiters.
* **Resilient Reconnection**: Exponential backoff reconnect logic handling temporary disconnections gracefully.

## Getting Started

### Prerequisites
* Node.js v18+
* PostgreSQL database

### Installation
```bash
git clone https://github.com/itsgoharrehman/whatsapp-ai-platform-v2.git
cd whatsapp-ai-platform-v2
npm install
```

### Configuration
Create a `.env` file in the root directory:
```env
PORT=5000
DATABASE_URL=postgresql://user:password@localhost:5432/whatsapp_platform
JWT_SECRET=your_jwt_secret_key
```

### Running the Platform
```bash
npm run build
npm start
```

## Security Policy

Please disclose vulnerabilities directly to `goharrehmanfsd260@gmail.com`.

## Maintainer

* **Gohar Rehman**
* GitHub: [@itsgoharrehman](https://github.com/itsgoharrehman)
* Email: `goharrehmanfsd260@gmail.com`
* Website: [itsgoharrehman.netlify.app](https://itsgoharrehman.netlify.app/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
