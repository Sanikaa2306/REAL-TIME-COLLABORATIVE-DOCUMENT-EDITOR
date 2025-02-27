# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

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

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)


INTRODUCTION -
--------------------------------------------------------------------------------------------------------
In today's interconnected world, seamless collaboration on documents among multiple users is 
essential for productivity and efficiency. The Real-Time Collaborative Document Editor is a 
cutting-edge application designed to facilitate simultaneous editing of shared documents by 
multiple users in real time. This project harnesses the power of modern web technologies, 
including NestJS for the backend, WebSocket for real-time communication, and robust 
authentication mechanisms to ensure data security and user privacy


KEY-FEATURES ->
--------------------------------------------------------------------------------------------------------

  1. Real-Time Collaboration
  2. Document & users management
  3. Identification/mapping of websocket client with database user
  4. Authentication & Authorization
  5. Conflict Resolution
  6. Persistence
  7. Maintaining DTO’s (Data Transfer Object)
  8. Class-Validator & Class-Transformer

TECHNOLOGY STACK  ->
--------------------------------------------------------------------------------------------------------

  1. Frontend : ReactJS, state management(ContextAPI), TailwindCSS
  2. Backend : NestJS, WebSockets Gateway, Socket.io-client, Mongoose, Mongo-Atlas, JWT(JSON web token - HMAC with SHA-256), Typescript

PROJECT STRUCTURE ->
--------------------------------------------------------------------------------------------------------

Realtime-collaborative-doc-editor/
│
├── src/
│ ├── app.module.ts // Main module
│ ├── document/ // Document module
│ │ ├── document.controller.ts // Document controller
│ │ ├── document.service.ts // Document service
│ │ ├── document.entity.ts // Document entity (Mongoose)
│ │ └── document.module.ts // Document module definition
│ │
│ ├── auth/ // Authentication module
│ │ ├── auth.controller.ts // Auth controller (login, register)
│ │ ├── auth.service.ts // Auth service (JWT authentication)
│ │ └── auth.module.ts // Auth module definition
│ │ └── jwt.strategy.ts 
│ │ └── guards
│ │ ├── jwt-guards.auth.ts // JWT guard for authentication
│ │
│ ├── user/ // User module
│ │ ├── user.controller.ts // User controller
│ │ ├── user.service.ts // User service
│ │ ├── user.entity.ts // User entity (Mongoose)
│ │ └── user.module.ts // User module definition
│ ├── socket.gateway.ts // WebSocket gateway
│ │
│ └── main.ts // Entry point for the application
├── .env // Environment variables
└── package.json // Project dependencies and scripts


VIDEO-DEMO URL ->
--------------------------------------------------------------------------------------------------------


  1. Frontend :
      
       Part 1 - https://www.loom.com/share/ef97f7ba1e16435baf3506f7e2333ab8?sid=9ab4cb8c-39a9-48ea-9cde-c55c023b6e76

       Part 2 - https://www.loom.com/share/db0d9a09a1a64a1196e2fb717db1fea2?sid=82fe327b-9ff7-4d4b-88e8-871ac0c95c7b
     
  3. Backend :
                https://www.loom.com/share/d32ac1f69e454fbab57841eb05fe958a?sid=1b64a82b-9707-4481-908b-3f087d283069

PROJECT SNAPSHOTS ->
--------------------------------------------------------------------------------------------------------



![Screenshot (19)](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/4e9c93d3-9b8d-4170-8683-41b3c9cdf44d)


![Screenshot (21)](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/d8d46bcc-af22-40d3-964e-707766b51522)


![Screenshot (22)](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/37f102ba-e5d4-4083-8b7f-660db28e2cb9)


![Screenshot (26)](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/bec637a6-c544-4f26-877b-5cd6dc594647)


![Screenshot (28)](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/ee8a2558-3320-40be-9f96-b40d3f5e2c16)


![Screenshot (33)](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/b7bea3c8-584d-4247-924f-dbe96bc2bd24)


![Screenshot (35)](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/179da481-b196-410e-a4ce-d56cd1b43442)

