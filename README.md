# cloud-vampire
# CloudVampire Interceptor // Full-Stack Cloud Optimization Engine

CloudVampire Interceptor is a high-utility, production-grade full-stack application engineered to isolate and eliminate **Zombie Infrastructure ("Vampire Servers")** across public cloud platforms. The system bridges a low-latency frontend tactical dashboard with an authenticated Node.js microservice backend to target and terminate idle cloud instances via the official enterprise AWS SDK.

## 💸 The \$150 Billion Cloud Resource Crisis
As engineering teams scale, they continuously spin up virtual servers, dev environments, and sandbox databases for feature verification. However, due to decentralized team operations, **up to 35% of all corporate cloud computing infrastructure sits completely idle** over weekends, holidays, and nights—processing zero user traffic while continuing to bill corporate credit cards. 

CloudVampire Interceptor solves this hidden operational bottleneck by continually parsing compute metrics, aggregating active budget leakage variables, and providing engineering managers with a single-click cloud API destruction mechanism.

## 🏗️ Full-Stack System Architecture

```text
[ Client Dashboard UI ]  <───(Secure HTTPS)───>  [ Node.js API Backend ]
  (HTML5/CSS3/Async JS)                             (Express / Cors Network Layer)
                                                               │
                                                 (Secure Environment Variables)
                                                               │
                                                               ▼
                                               [ AWS Data Center Cloud Infrastructure ]
                                                 ├── CloudWatch API (Reads Real Telemetry)
                                                 └── EC2 Service API (Live Termination)
```

## 💰 The Developer Cost Breakdown (Is it Free?)
**Yes.** Running, testing, and presenting this application is **100% free** under the standard **AWS New Account Free Tier** (valid for the first 12 months).

* **Compute (AWS EC2):** 750 free hours per month of a `t2.micro` or `t3.micro` Linux instance. (A full month only has 744 hours, making a single test node entirely free).
* **Monitoring (AWS CloudWatch):** 1,000,000 free metrics API requests per month. Our Node.js microservice stays safely within these thresholds.

*Note: AWS requires a credit/debit card during identity registration purely to verify user authenticity and prevent server room spam abuse. No charges are applied as long as you deploy Free Tier eligible infrastructure instances.*

## 🔑 IAM Security & Credential Configuration
To connect this codebase to a live AWS account, you must provision a programmatic developer user with strict, restricted permissions inside the **AWS IAM Console**:

1. Create a user named `CloudVampireDeveloper`.
2. Attach these two standard AWS enterprise permission policies directly:
   * `AmazonEC2FullAccess` (Grants the `server.js` script rights to list and destroy instances).
   * `CloudWatchReadOnlyAccess` (Grants the `server.js` script rights to poll live CPU averages).
3. Generate **Access Keys** for the user under the **Local Code** use-case. Securely download the `Access Key ID` and `Secret Access Key`.

## 📁 Repository Blueprint
```text
├── index.html       # Structural frontend control viewport layout
├── app.js           # Frontend data parsing & backend consumer logic
└── server.js        # Full-stack Node.js API & AWS SDK integration layer
```

## 🛠️ Local Ubuntu Deployment & Setup

### 1. Project Initialization & Dependencies
Initialize your software package workspace and pull down the enterprise production dependencies:
```bash
npm init -y
```
*Note: Ensure you open your generated `package.json` file and append `"type": "module"` directly below the `"name"` key to support modern ECMAScript imports.*

Install the production packages:
```bash
npm install express cors @aws-sdk/client-ec2 @aws-sdk/client-cloudwatch
```

### 2. Environment Security Injection
Inject your downloaded cloud access credentials straight into your local shell environment memory to authorize your Node.js server without hardcoding passwords into plain-text files:
```bash
export AWS_ACCESS_KEY_ID="your_actual_aws_access_key"
export AWS_SECRET_ACCESS_KEY="your_actual_aws_secret_key"
```

### 3. Launching the Full-Stack Pipeline
Boot your server core instance. It will initialize and bind itself to Port 3000:
```bash
node server.js
```

Launch a local static web server inside another terminal block to preview your interface:
```bash
python3 -m http.server 5500
```
Open your browser engine and navigate to `http://127.0.0.1:5500`.

## 🧪 Live Presentation Verification Protocol
1. Open your browser dashboard interface and click **Scan Real AWS Architecture**.
2. Watch your cluster boxes dynamically parse the background arrays. The backend will pull real-world metrics via **CloudWatch**, isolating idle infrastructure elements with real-time financial tracking indicators.
3. Click **Execute Cloud Terminations**.
4. Monitor your application terminal live: Your browser logs will capture the secure backend handshake, display the incoming verified AWS JSON lifecycle mutation from `running` to `terminating`, and wipe the operational cost leak to absolute zero.

## 🛡️ License
Distributed under the MIT Open Source License. Architectural efficiency built at the speed of thought.
# cloud-vampire
