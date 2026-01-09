# Next.js on cPanel Shared Hosting

![Next.js](https://img.shields.io/badge/Next.js-Production-black)
![Node.js](https://img.shields.io/badge/Node.js-20%2B-green)
![cPanel](https://img.shields.io/badge/cPanel-Shared%20Hosting-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

This repository provides a simple and practical setup to deploy a Next.js application on cPanel shared hosting. It is intended for environments where VPS access, Docker or advanced server control is not available.

The setup uses cPanel Node.js Application Manager with a custom server.js and a minimal next.config.js to serve a production build of a Next.js app.

## Repository Tags

nextjs, cpanel, shared-hosting, nodejs, deployment, serverjs, next-config, production

## Features

- Works on cPanel shared hosting
- Uses Node.js Application Manager
- Custom server.js for production mode
- No VPS or container setup required
- Lightweight and easy to maintain

## Requirements

- cPanel hosting with Node.js enabled
- Node.js version 20 or higher
- Access to cPanel File Manager or Git

## Project Structure

- server.js  
  Custom Node.js server to start and serve the Next.js app.

- next.config.js  
  Next.js configuration adjusted for shared hosting.

- package.json  
  Scripts required to build and start the app.

## Deployment Steps

1. Upload your Next.js project to your cPanel account.
2. Open Node.js Application Manager in cPanel.
3. Create a new Node.js application.
4. Set the application root to your project folder.
5. Set the startup file to server.js.
6. Select the required Node.js version.
7. Click Run NPM Install.
8. Build the project by running:
   npm run build
9. Start the application from cPanel.

## package.json Script Example

```"scripts": {
  "build": "next build",
  "start": "NODE_ENV=production node server.js"
}```

## Use Cases

- Hosting Next.js apps on shared hosting
- Deploying client websites on cPanel
- Running small production projects without VPS

## Limitations

- Development mode is not supported
- Hot reload is not available
- Performance depends on hosting limits

## License

This project is licensed under the MIT License.
