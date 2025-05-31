# Node.js Express TypeScript Starter

A robust and production-ready Node.js backend starter template built with Express.js and TypeScript. This template provides a solid foundation for building scalable RESTful APIs with modern best practices and security features.

## 🚀 Features

- **TypeScript** - Written in TypeScript for better type safety and developer experience
- **Express.js** - Fast, unopinionated, minimalist web framework for Node.js
- **MongoDB** - MongoDB integration with Mongoose ODM
- **Security Features**
  - Rate limiting to prevent abuse
  - IP whitelisting/blacklisting
  - CORS enabled
  - Request size limits
- **Authentication** - JWT-based authentication system
- **Environment Configuration** - Dotenv for environment variable management
- **Development Tools**
  - Hot reloading with ts-node-dev
  - TypeScript compilation
  - Pre-commit hooks for code quality
  - Cross-env for environment variable management

## 📋 Prerequisites

- Node.js (v14 or higher)
- MongoDB
- Yarn or npm

## 🛠️ Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd node-express-ts-starter
```

2. Install dependencies:
```bash
yarn install
# or
npm install
```

3. Create a `.env` file in the root directory and add your environment variables:
```env
PORT=3000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

## 🚀 Usage

### Development
```bash
yarn dev
# or
npm run dev
```

### Production
```bash
yarn build
yarn start
# or
npm run build
npm start
```

### Type Checking
```bash
yarn ts.check
# or
npm run ts.check
```

## 📁 Project Structure

```
├── config/         # Configuration files
├── middleware/     # Custom middleware
├── model/         # Database models
├── routes/        # API routes
├── utils/         # Utility functions
├── index.ts       # Application entry point
├── tsconfig.json  # TypeScript configuration
└── package.json   # Project dependencies
```

## 🔒 Security Features

- **Rate Limiting**: Implements rate limiting to prevent abuse (100 requests per 15 minutes per IP)
- **IP Filtering**: Supports IP whitelisting and blacklisting
- **Request Size Limits**: Limits request body size to 50MB
- **CORS**: Cross-Origin Resource Sharing enabled
- **Environment Variables**: Secure configuration management

## 🛠️ Available Scripts

- `dev`: Start development server with hot reload
- `start`: Start production server
- `build`: Build TypeScript files
- `ts.check`: Run TypeScript type checking
- `add-build`: Add built files to git

## 📦 Dependencies

### Main Dependencies
- express: Web framework
- mongoose: MongoDB ODM
- jsonwebtoken: JWT authentication
- bcryptjs: Password hashing
- cors: Cross-Origin Resource Sharing
- dotenv: Environment variable management
- express-rate-limit: Rate limiting
- express-validator: Request validation

### Development Dependencies
- typescript: TypeScript support
- ts-node: TypeScript execution
- ts-node-dev: Development server with hot reload
- @types/*: TypeScript type definitions

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- Your Name - Initial work

## 🙏 Acknowledgments

- Express.js team for the amazing framework
- TypeScript team for the type system
- MongoDB team for the database
