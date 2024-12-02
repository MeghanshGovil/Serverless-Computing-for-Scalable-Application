# Serverless Corona Admin Dashboard

## Project Overview

This project transforms the Corona Admin free admin template into a fully serverless web application leveraging AWS cloud services. By reimagining the original Bootstrap 5 admin dashboard, we've created a scalable, high-performance solution that eliminates server management overhead.

## Original Template Credits

* **Template**: Corona Admin Free Bootstrap 5 Admin Template
* **Original Developers**: BootstrapDash
* **Key Technologies**:
  - Bootstrap 5
  - Material Design Icons
  - jQuery
  - Chart.js

## Serverless Architecture

### Project Architecture

Our serverless implementation uses the following AWS services:

* **Frontend Hosting**: Amazon S3
* **Content Delivery**: Amazon CloudFront
* **Backend Compute**: AWS Lambda
* **Database**: Amazon DynamoDB
* **Authentication**: Amazon Cognito (optional)

### Key Architectural Benefits

- **Zero Server Management**: Completely serverless infrastructure
- **Automatic Scaling**: Handles traffic spikes effortlessly
- **Cost-Efficient**: Pay only for actual usage
- **High Availability**: Distributed across multiple AWS regions

## Features

### Original Corona Admin Features
- Responsive Design
- Clean, Elegant UI
- Comprehensive Admin Dashboard Components
- Chart Integrations
- Modern Browser Support

### Serverless Enhancements
- Automatic Scaling
- Global Low-Latency Delivery
- Secure, Managed Infrastructure
- Simplified Deployment
- Reduced Operational Overhead

## Prerequisites

- AWS Account
- Node.js (v14+ recommended)
- AWS CLI
- Serverless Framework (optional but recommended)

## Installation & Deployment

### Local Development

1. Clone the repository
   ```bash
   git clone https://github.com/[your-username]/corona-admin-serverless.git
   cd corona-admin-serverless
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Configure AWS Credentials
   ```bash
   aws configure
   ```

### Serverless Deployment

```bash
# Deploy entire serverless stack
serverless deploy --stage production

# Or use AWS SAM
sam build
sam deploy --guided
```

## Project Structure

```
corona-admin-serverless/
│
├── frontend/               # S3 Hosted Static Files
│   ├── index.html
│   ├── assets/
│   └── js/
│
├── lambda/                 # AWS Lambda Functions
│   ├── crud-operations/
│   └── authentication/
│
├── infrastructure/         # CloudFormation/SAM Templates
│   └── serverless.yml
│
└── README.md
```

## Security Considerations

- Implemented AWS Cognito for authentication
- Used AWS IAM Roles for granular access control
- Enabled CloudFront HTTPS by default
- Integrated AWS WAF for additional protection

## Cost Optimization

- Utilized Lambda's pay-per-execution model
- Implemented DynamoDB auto-scaling
- Leveraged CloudFront caching strategies

## Browser Compatibility

Fully compatible with:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Contributing

Contributions are welcome! Please read our contributing guidelines before submitting pull requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- Original template by BootstrapDash
- AWS Serverless Application Model (SAM)
- Open-source community

---

**Note**: This is a community project and is not officially associated with BootstrapDash or AWS.
