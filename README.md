### Development Workflow

1. **Link the package locally**

   In the `packages/react-pdf` directory, run:
   ```
   yarn link
   yarn link --link-namespace "jeremy-react-pdf"
   ```

2. **Link the package in the sample app**

   In the `sample/next-app` directory, run:
   ```
   yarn link "jeremy-react-pdf"
   ```

3. **Run the sample app**

   In the `sample/next-app` directory, run:
   ```
   npm run dev
   ```

4. **Rebuild after changes**

   Every time you make a change to the package, rebuild it in `packages/react-pdf`:
   ```
   npm run build
   ```

---

### Publishing Workflow

1. **Login to NPM**

   In the `packages/react-pdf` directory, run:
   ```
   npm login
   ```

2. **Build the package**

   ```
   npm run build
   ```

3. **Publish the package**

   In the `packages/react-pdf` directory, run:
   ```
   npm publish --access public
   ```

   > **Note:** Update the version in `package.json` before publishing if needed.
