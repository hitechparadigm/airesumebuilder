# AI Resume Helper

airesumebuilder/
├── .github/
│   └── workflows/
│       └── deploy.yml               # GitHub Actions workflow for automated deployment
├── frontend/
│   ├── public/                      # Public assets for the frontend app (React or other framework)
│   ├── src/                         # Source code for the frontend app (React or other framework)
│   ├── package.json                 # NPM package file for managing frontend dependencies
│   ├── .env                         # Environment variables (e.g., API Gateway URL)
│   └── README.md                    # Documentation for the frontend app
├── infrastructure/
│   ├── parameters.yaml              # CloudFormation parameters for S3, Lambda, etc.
│   ├── infrastructure.yaml          # Main CloudFormation template for backend resources
│   └── s3_cloudfront_infrastructure.yaml # CloudFormation template for S3 and CloudFront setup
├── lambda_functions/
│   ├── process_job_description/
│   │   ├── index.py                 # Lambda code for processing job descriptions
│   │   └── requirements.txt         # Optional: Dependencies for this Lambda function
│   ├── generate_resume/
│   │   ├── index.py                 # Lambda code for generating the resume
│   │   └── requirements.txt         # Optional: Dependencies for this Lambda function
├── scripts/
│   └── package_and_upload.sh        # Script to package and upload Lambda functions to S3
└── README.md                        # Documentation for the overall project

