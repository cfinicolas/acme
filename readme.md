# @cfinicolas/acme

> A dummy package for testing and experimentation.

---

## 📦 Installation

Install the package:

```bash
npm install @cfinicolas/acme
```

---

## 🚀 Usage

Import and use the package:

```ts
import { sayHello } from "@cfinicolas/acme";

const greeting = sayHello("John");

console.log(greeting); // Hello John!
```

---

## 📦 Releases & Publishing

This package uses [Changesets](https://github.com/changesets/changesets) for versioning and publishing.

1. Create a Changeset:

   ```bash
   npm run changeset
   ```

   Follow the prompts to describe your changes.

2. Apply the version bump and rebuild the package:

   ```bash
   npm run version
   ```

   This will:

   - Bump the version in `package.json`
   - Update `CHANGELOG.md`
   - Rebuild the package

3. Publish the package:

   Make sure you're authenticate with the Business NPM Registry. If not, please follow this [guide](#-authenticate-with-the-business-npm-registry). Otherwise continue with:

   ```bash
   npm run publish
   ```

4. Verify your package has been published at:

   `https://npm.business.com/`

5. You may now use your package in your projects!

## 🔐 Authenticate with the Business NPM Registry:

1. Log in:

   ```bash
   npm login --registry=https://npm.business.com
   ```

   Enter your **username**, **password**, and **email** when prompted.

2. Verify login:
   ```bash
   npm whoami --registry=https://npm.business.com
   ```
   If successful, it will return your npm username. Otherwise, repeat the login step.
