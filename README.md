<p align="center">
  <img 
    src="assets/dashboard-greeting-bits-and-brains-ai.png"
    alt="Blockchain Task Management System Dashboard"
    width="900"
  />
</p>
<h1>🏷️ Project Title</h1>

<p>
  <strong style="font-size: 2rem;">
    Decentralized Blockchain-Based To-Do List Application (DApp)
  </strong>
</p>

<hr />

<h2>🧾 Executive Summary</h2>
<p>
This project is a modern decentralized To-Do List application built using <strong>Next.js</strong>,
<strong>Ethereum smart contract integration</strong>, and <strong>Web3 wallet connectivity</strong>.
Unlike traditional task managers, this system stores tasks immutably on the blockchain, ensuring
data integrity, transparency, and user ownership.
</p>
<p>
The application allows users to connect a crypto wallet, interact with a deployed smart contract,
create and manage tasks, and view task states directly from the blockchain. The system is production-ready,
deployable on Vercel, and aligned with modern Web3 architecture standards.
</p>

<hr />

<h2>📑 Table of Contents</h2>
<ul>
  <li>🧩 Project Overview</li>
  <li>🎯 Objectives & Goals</li>
  <li>✅ Acceptance Criteria</li>
  <li>💻 Prerequisites</li>
  <li>⚙️ Installation & Setup</li>
  <li>🔗 API Documentation</li>
  <li>🖥️ UI / Frontend</li>
  <li>🔢 Status Codes</li>
  <li>🚀 Features</li>
  <li>🧱 Tech Stack & Architecture</li>
  <li>🛠️ Workflow & Implementation</li>
  <li>🧪 Testing & Validation</li>
  <li>🔍 Validation Summary</li>
  <li>🧰 Verification Tools</li>
  <li>🧯 Troubleshooting & Debugging</li>
  <li>🔒 Security & Secrets</li>
  <li>☁️ Deployment (Vercel)</li>
  <li>⚡ Quick-Start Cheat Sheet</li>
  <li>🧾 Usage Notes</li>
  <li>🧠 Performance & Optimization</li>
  <li>🌟 Enhancements & Features</li>
  <li>🧩 Maintenance & Future Work</li>
  <li>🏆 Key Achievements</li>
  <li>🧮 High-Level Architecture</li>
  <li>🗂️ Project Structure</li>
  <li>🧭 How to Demonstrate Live</li>
  <li>💡 Summary, Closure & Compliance</li>
</ul>

<hr />

<h2>🧩 Project Overview</h2>
<p>
The project implements a decentralized task management system where each task is recorded
on the blockchain via a smart contract. The frontend communicates with the blockchain using
contract ABI definitions and wallet-based authentication.
</p>

Key characteristics:
<ul>
  <li>Client-side rendered Web3 DApp</li>
  <li>Wallet-based authentication (MetaMask)</li>
  <li>Immutable task storage</li>
  <li>No centralized backend database</li>
</ul>

<hr />

<h2>🎯 Objectives & Goals</h2>
<ul>
  <li>Demonstrate practical blockchain integration in a frontend app</li>
  <li>Ensure user data ownership and transparency</li>
  <li>Eliminate centralized storage dependencies</li>
  <li>Build a deployable, scalable Web3 UI</li>
</ul>

<hr />

<h2>✅ Acceptance Criteria</h2>
<table>
  <tr>
    <th>Criteria</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Wallet Connection</td>
    <td>User must connect wallet before interacting</td>
  </tr>
  <tr>
    <td>Task Creation</td>
    <td>Tasks must be written to blockchain</td>
  </tr>
  <tr>
    <td>Task Visibility</td>
    <td>Tasks persist across sessions</td>
  </tr>
  <tr>
    <td>Network Validation</td>
    <td>Wrong network warning must appear</td>
  </tr>
</table>

<hr />

<h2>💻 Prerequisites</h2>
<ul>
  <li>Node.js (v16+)</li>
  <li>NPM or Yarn</li>
  <li>MetaMask Wallet</li>
  <li>Ethereum Test Network</li>
</ul>

<hr />

<h2>⚙️ Installation & Setup</h2>
<ol>
  <li>Clone repository</li>
  <li>Install dependencies</li>
  <li>Configure blockchain contract address</li>
  <li>Start development server</li>
</ol>

<hr />

<h2>🔗 API Documentation</h2>
<p>
This application does not rely on traditional REST or GraphQL APIs. Instead, it uses a
<strong>Blockchain-as-an-API model</strong>, where Ethereum smart contracts act as the authoritative
backend. All reads and writes are executed through Web3 providers using contract ABI definitions.
</p>

<h3>Interaction Model</h3>
<table>
  <tr>
    <th>Layer</th>
    <th>Responsibility</th>
    <th>Details</th>
  </tr>
  <tr>
    <td>Frontend (Next.js)</td>
    <td>UI & User Actions</td>
    <td>Collects input, triggers blockchain calls</td>
  </tr>
  <tr>
    <td>Web3 Provider</td>
    <td>Transport</td>
    <td>Bridges UI and Ethereum network</td>
  </tr>
  <tr>
    <td>Smart Contract</td>
    <td>Business Logic</td>
    <td>Stores, retrieves, validates tasks</td>
  </tr>
</table>

<h3>Smart Contract Methods (Logical API)</h3>
<table>
  <tr>
    <th>Method</th>
    <th>Type</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>createTask</td>
    <td>Transaction</td>
    <td>Writes a new task to the blockchain</td>
  </tr>
  <tr>
    <td>getTasks</td>
    <td>Read-only</td>
    <td>Fetches all tasks for a wallet</td>
  </tr>
  <tr>
    <td>toggleTaskStatus</td>
    <td>Transaction</td>
    <td>Marks a task as completed/incomplete</td>
  </tr>
</table>
<hr />

<h2>🖥️ UI / Frontend</h2>
<p><strong>Pages:</strong></p>
<ul>
  <li><strong>index.js</strong> – Main dashboard</li>
  <li><strong>_app.js</strong> – Global layout and providers</li>
</ul>

<p><strong>Components:</strong></p>
<ul>
  <li>Navbar – Application header</li>
  <li>ConnectWalletButton – Wallet integration</li>
  <li>TodoList – Task container</li>
  <li>Task – Individual task renderer</li>
  <li>WrongNetworkMessage – Network guard</li>
</ul>

<p><strong>Styling:</strong></p>
<ul>
  <li>Tailwind CSS</li>
  <li>Global and module-scoped styles</li>
</ul>

<hr />

<h2>🔢 Status Codes</h2>
<table>
  <tr>
    <th>Status</th>
    <th>Meaning</th>
  </tr>
  <tr>
    <td>200</td>
    <td>Successful blockchain interaction</td>
  </tr>
  <tr>
    <td>400</td>
    <td>User rejected wallet request</td>
  </tr>
  <tr>
    <td>403</td>
    <td>Wrong blockchain network</td>
  </tr>
</table>

<hr />

<h2>🚀 Features</h2>
<ul>
  <li><strong>Fully Decentralized Storage:</strong> Tasks are persisted on-chain, eliminating centralized databases.</li>
  <li><strong>Wallet-Based Identity:</strong> User identity is derived directly from Ethereum wallet addresses.</li>
  <li><strong>Immutable Task History:</strong> Once written, tasks cannot be altered maliciously.</li>
  <li><strong>Network Validation:</strong> Detects incorrect blockchain networks and prevents unsafe interactions.</li>
  <li><strong>Transaction Lifecycle Awareness:</strong> UI reflects pending, confirmed, and failed states.</li>
  <li><strong>Zero Backend Servers:</strong> Entire system operates without traditional servers.</li>
  <li><strong>Production-Ready Frontend:</strong> Optimized, modular, and deployable at scale.</li>
</ul>

<hr />

<h2>🧱 Tech Stack & Architecture</h2>

<h3>Technology Stack</h3>
<table>
  <tr>
    <th>Layer</th>
    <th>Technology</th>
    <th>Purpose</th>
  </tr>
  <tr>
    <td>Frontend</td>
    <td>Next.js, React</td>
    <td>UI rendering and routing</td>
  </tr>
  <tr>
    <td>Styling</td>
    <td>Tailwind CSS</td>
    <td>Utility-first responsive styling</td>
  </tr>
  <tr>
    <td>Blockchain</td>
    <td>Ethereum</td>
    <td>Decentralized state storage</td>
  </tr>
  <tr>
    <td>Web3 Layer</td>
    <td>Ethers.js</td>
    <td>Smart contract communication</td>
  </tr>
  <tr>
    <td>Deployment</td>
    <td>Vercel</td>
    <td>Global edge hosting</td>
  </tr>
</table>

<h3>ASCII Component Architecture</h3>
<pre>
┌─────────────┐
│   User UI   │
│  (Browser)  │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ Next.js App │
│ React Layer │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ Ethers.js   │
│ Web3 Layer  │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ Smart       │
│ Contract    │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│ Ethereum    │
│ Blockchain  │
└─────────────┘
</pre>

<hr />

<h2>🛠️ Workflow & Implementation</h2>
<ol>
  <li>User opens the web application.</li>
  <li>Frontend initializes Web3 provider detection.</li>
  <li>User connects wallet (MetaMask).</li>
  <li>Network ID is validated against supported chains.</li>
  <li>Smart contract instance is created using ABI and address.</li>
  <li>Existing tasks are fetched via read-only blockchain calls.</li>
  <li>User submits a new task.</li>
  <li>Transaction request is sent to wallet.</li>
  <li>User signs transaction.</li>
  <li>Transaction is mined and confirmed.</li>
  <li>UI re-syncs state from blockchain.</li>
</ol>

<hr />

<h2>🧪 Testing & Validation</h2>
<table>
  <tr>
    <th>ID</th>
    <th>Area</th>
    <th>Action</th>
    <th>Expected Result</th>
    <th>Purpose</th>
  </tr>
  <tr>
    <td>TV-01</td>
    <td>Wallet</td>
    <td>Connect Wallet</td>
    <td>Wallet address displayed</td>
    <td>Auth verification</td>
  </tr>
  <tr>
    <td>TV-02</td>
    <td>Blockchain</td>
    <td>Create Task</td>
    <td>Task appears on reload</td>
    <td>Persistence check</td>
  </tr>
  <tr>
    <td>TV-03</td>
    <td>Network</td>
    <td>Wrong Chain</td>
    <td>Error message shown</td>
    <td>Safety validation</td>
  </tr>
</table>

<hr />

<h2>🔍 Validation Summary</h2>
<p>
All critical flows were validated against real blockchain interactions. No centralized
failure points were observed. State consistency was verified across reloads and sessions.
</p>

<hr />

<h2>🧰 Verification Testing Tools & Command Examples</h2>
<ul>
  <li>MetaMask Activity Logs</li>
  <li>Ethereum Block Explorers</li>
  <li>Browser Developer Console</li>
  <li>React DevTools</li>
</ul>

<hr />

<h2>🧯 Troubleshooting & Debugging</h2>
<table>
  <tr>
    <th>Issue</th>
    <th>Cause</th>
    <th>Resolution</th>
  </tr>
  <tr>
    <td>Wallet not detected</td>
    <td>Extension disabled</td>
    <td>Enable MetaMask</td>
  </tr>
  <tr>
    <td>Transaction stuck</td>
    <td>Low gas</td>
    <td>Increase gas fee</td>
  </tr>
  <tr>
    <td>Wrong network</td>
    <td>Incorrect chain</td>
    <td>Switch to supported network</td>
  </tr>
</table>

<hr />

<h2>🔒 Security & Secrets</h2>
<ul>
  <li>No private keys stored</li>
  <li>Wallet signs transactions client-side</li>
  <li>Environment variables handled securely</li>
</ul>

<hr />

<h2>☁️ Deployment </h2>
<ol>
  <li>Push repository to GitHub</li>
  <li>Import project into Vercel</li>
  <li>Configure environment variables</li>
  <li>Build and deploy</li>
  <li>Verify wallet and contract interactions</li>
</ol>
<hr />

<h2>⚡ Quick-Start Cheat Sheet</h2>
<ul>
  <li>Install dependencies</li>
  <li>Run development server</li>
  <li>Connect wallet</li>
  <li>Create tasks</li>
</ul>

<hr />

<h2>🧾 Usage Notes</h2>
<p>
Users should note that blockchain writes are permanent and incur gas fees.
This application is recommended for test networks during demonstrations.
</p>

<hr />
<h2>🧠 Performance & Optimization</h2>
<ul>
  <li>Minimized blockchain reads</li>
  <li>Client-side state caching</li>
  <li>Component-level re-render control</li>
</ul>

<hr />

<h2>🌟 Enhancements & Features</h2>
<ul>
  <li>Task categories</li>
  <li>Multi-chain support</li>
  <li>Layer-2 integration</li>
</ul>

<hr />

<h2>🧩 Maintenance & Future Work</h2>
<ul>
  <li>Upgradeable smart contracts</li>
  <li>Gas usage optimization</li>
  <li>Improved UX flows</li>
</ul>

<hr />

<h2>🏆 Key Achievements</h2>
<ul>
  <li>Zero-backend decentralized architecture</li>
  <li>Production-ready Web3 frontend</li>
  <li>Blockchain-persistent data model</li>
</ul>

<hr />

<h2>🧮 High-Level Architecture</h2>
<pre>
User
 │
 ▼
Web Browser
 │
 ▼
Next.js UI
 │
 ▼
Wallet Provider
 │
 ▼
Smart Contract Interface
 │
 ▼
Ethereum Network
</pre>

<hr />

<h2>🗂️ Project Structure</h2>
<pre>
TO_DoList_Blockchain-main/
 ├── components/
 │   ├── ConnectWalletButton.js
 │   ├── Navbar.js
 │   ├── Task.js
 │   ├── TodoList.js
 │   └── WrongNetworkMessage.js
 ├── pages/
 │   ├── _app.js
 │   ├── index.js
 │   └── api/hello.js
 ├── styles/
 │   ├── globals.css
 │   └── Home.module.css
 ├── utils/
 │   └── TaskContract.json
 ├── config.js
 ├── next.config.js
 ├── tailwind.config.js
 ├── package.json
</pre>

<hr />

<h2>🧭 How to Demonstrate Live</h2>
<ol>
  <li>Launch application</li>
  <li>Connect MetaMask</li>
  <li>Create a task</li>
  <li>Refresh page to show persistence</li>
</ol>

<hr />

<h2>💡 Summary, Closure & Compliance</h2>
<p>
This project demonstrates enterprise-grade decentralized application design using modern
Web3 standards. It complies with open-source norms, avoids centralized data handling, and
follows secure wallet-based interaction patterns suitable for professional and commercial use.
</p>

</body>
</html>

