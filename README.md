This is the Readme for the passport mobile app.  It is built in React Native.

### Branch Structure

Our app's development process revolves around three main branches, each serving a specific purpose in the lifecycle of the app. This approach ensures smooth transitions from development to production, adhering to best practices in software development.

- **Main Branch**: This is the live app branch. It mirrors what's currently live in production. All updates that pass through the staging process and are deemed ready for live deployment will be merged into this branch.

- **Staging Branch**: Our staging branch is a pre-production environment. It's where our app undergoes thorough testing. This branch hosts the TestFlight and Google Beta versions of the app. Only after successful testing and quality assurance here will updates be considered for merging into the main branch.

- **Development Branch**: This is the primary development branch. All ongoing development work, including new features and bug fixes, will be committed here. It serves as a base for all development activities. Developers should branch off from here to create feature branches.

### Workflow Overview

1. **Feature Development**:
   - Developers create new branches off the `development` branch for each feature or bug fix. These branches are named according to the feature or fix they're intended for (e.g., `feature/user-authentication`, `fix/login-bug`).
   - Once the work is completed and locally tested, developers will open a pull request (PR) against the `development` branch.

2. **Code Review and Merge to Development**:
   - Team members review the PRs for code quality, functionality, and adherence to project guidelines.
   - After approval, the feature or fix is merged into the `development` branch. This merge signifies that the code is ready for broader testing beyond the scope of the developer's local environment.

3. **Staging for Testing**:
   - Periodically, the team will merge the `development` branch into `staging` to prepare for a release. This merge initiates a cycle of testing in the app's staging environment.
   - The app in the staging branch undergoes rigorous testing through TestFlight and Google Beta. Feedback and bug reports are addressed during this stage.

4. **Production Release**:
   - Upon successful testing and quality assurance in the staging branch, the changes are deemed ready for production.
   - The `staging` branch is then merged into the `main` branch, updating the live application with the new features or fixes.
