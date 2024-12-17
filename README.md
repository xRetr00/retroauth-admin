# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

# RetroAuth Admin Panel

A modern web interface for managing RetroAuth licenses.

## Deployment to GitHub Pages

1. Create a new GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/retroauth-admin.git
   git push -u origin main
   ```

2. Enable GitHub Pages:
   - Go to your repository settings
   - Navigate to "Pages" section
   - Select "main" branch as source
   - Select "/(root)" as folder
   - Click "Save"

3. Update API URL:
   - Open `index.html`
   - Find the `apiUrl` variable
   - Replace with your InfinityFree domain:
     ```javascript
     apiUrl: 'https://your-subdomain.infinityfree.com/api/v1'
     ```

4. Push changes:
   ```bash
   git add .
   git commit -m "Update API URL"
   git push
   ```

Your admin panel will be available at: `https://YOUR_USERNAME.github.io/retroauth-admin`

## Features

- Create new license keys
- Set license duration and level
- Revoke existing licenses
- Modern dark theme UI
- Responsive design

## Security Notes

- Ensure CORS is properly configured on your backend
- Consider adding authentication to the admin panel
- Use HTTPS for all API calls
- Regularly monitor access logs

## Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/retroauth-admin.git
   cd retroauth-admin
   ```

2. Open `index.html` in your browser or use a local server:
   ```bash
   python -m http.server 8000
   ```

3. Access at `http://localhost:8000`
