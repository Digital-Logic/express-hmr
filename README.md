# User Authentication, ACL, Express template

## What it provides
* User authorization, authentication, and access control.
* Social media login support and account integration
* Socket.IO is used to synchronizes application state between multiply sessions.
* JWT token are stored in cookies.
* Bcrypt encryption on user passwords
* Email validate, password reset using jwt tokens.
* ~~Express with HMR support through webpack.~~
* Server automatically restarts when changes are detected using nodemon through webpack
* MongoDB, Mongoose.
* Testing with Mocha, Chai in watch mode.
* Logging with winston and morgan.
* Global error handling.
* Pug template generation / bundling through webpack.

### Task List
- [ ] Jwt secret key rotation.
- [ ] API endpoint throttling.

### Available commands
```javascript
npm run start // Start the development server with nodemon (no longer with hmr)
npm run build // Create a production build, (/build)
npm run test  // Run tests through Mocha / Chai (with watch mode enabled)
npm run clean // Remove build files
```

### Env Variables
Common env variables are injected into the built bundle, unless overrides are provided.
All other are expected to be injected on runtime.

Development envs are injected through the .env file.
.env.defaults: is provided with some common defaults, override these settings with your own in a .env, and .env.testing file.

.env.testing file to set specific settings to use during testing.