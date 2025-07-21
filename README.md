# Global Node.js Libraries

This repository contains shared Node.js dependencies used across all my projects.

## 📦 **Included Dependencies**

- **Express.js** (v5.1.0) - Web framework
- **MySQL** (v2.18.1) - Database driver

## 🚀 **Installation**

### **As Git Submodule:**
```bash
git submodule add https://github.com/YOUR_USERNAME/global_libs.git libs
cd libs
pnpm install
```

### **As NPM Package:**
```bash
npm install git+https://github.com/YOUR_USERNAME/global_libs.git
```

### **Direct Clone:**
```bash
git clone https://github.com/YOUR_USERNAME/global_libs.git libs
cd libs
pnpm install
```

## 💡 **Usage in Projects**

```javascript
// In your project, reference the libs folder
const express = require('../libs/node_modules/express');
const mysql = require('../libs/node_modules/mysql');

const app = express();
const db = mysql.createConnection({ /* config */ });
```

## 🔧 **Maintenance**

```bash
# Update dependencies
pnpm update

# Add new dependency
pnpm add package-name

# List installed packages
pnpm list
```

## 📁 **Structure**

```
libs/
├── package.json      # Dependencies configuration
├── pnpm-lock.yaml   # Lock file for reproducible installs
├── node_modules/    # Installed packages
└── README.md        # This file
```

## 🎯 **Purpose**

- **Centralized Dependencies** - One place for all Node.js packages
- **Version Consistency** - Same versions across all projects
- **Easy Updates** - Update once, use everywhere
- **Reduced Redundancy** - No duplicate node_modules folders

---

**License:** MIT  
**Package Manager:** PNPM v10.13.1  
**Node.js:** >=14.0.0
