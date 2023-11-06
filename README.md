# Ethereum Job Portal Smart Contract

Welcome to the Ethereum Job Portal Smart Contract repository. This smart contract aims to connect unskilled and unorganized migrant workers with job providers while eliminating the exploitation by middlemen. It allows workers to create profiles, apply for jobs, and receive ratings from job providers.

## Overview

The Ethereum Job Portal Smart Contract is designed to facilitate the connection between job seekers (applicants) and job providers. It includes the following features:

- Applicants are registered by admin with their profiles, including details such as name, experience, skills, and more.
- Job providers can post new job listings with details like job title, description, salary, and experience requirements.
- Applicants can apply for jobs they are interested in.
- Job providers can hire applicants for their posted jobs.
- Job providers can provide ratings for applicants they've hired.

## Smart Contract Functions

### Adding Applicants
- `addApplicant(string name, uint experience, string[] skills, address applicantAddress)`: Allows the admin to add new applicants to the portal. Applicants provide their name, experience, skills, and Ethereum address.

### Getting Applicant Details
- `getApplicantDetails(uint256 applicantId)`: Retrieves detailed information about an applicant using their unique ID.

### Adding Jobs
- `addJob(string title, string description, uint experienceNeeded, uint256 salary) payable`: Enables job providers to post new job listings. Job providers pay 1 ether to list a job.

### Getting Job Details
- `getJobDetails(uint256 jobId)`: Retrieves detailed information about a job using its unique ID.

### Applying for Jobs
- `applyForJob(uint256 jobId)`: Allows applicants to apply for jobs they are interested in. It checks for applicant availability and prevents duplicate applications.

### Hiring Applicants
- `hireApplicant(uint jobId, uint applicantId)`: Permits job providers to hire applicants that have applied for specific job. It marks the applicant as "unavailable" as they get hired.

### Providing Ratings
- `provideRating(uint256 jobId, uint256 applicantId, uint256 rating)`: Lets job providers rate applicants they've hired. Ratings range from 1 to 5 and prevent double rating.

## Usage

To interact with this smart contract, you can deploy it to the Ethereum network using tools like Remix or Hardhat. Make sure to have Ethereum accounts with Ether for gas fees.

To compile and deploy the contract, follow these steps:

1. Clone this repository to your local machine.
2. Install a development environment for Ethereum (e.g., Remix, Truffle).
3. Deploy the contract to the Ethereum network.
4. Interact with the contract using its functions.

## Contributions

Contributions and improvements to this project are welcome. Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Create a pull request with a clear description of the changes.

## License

This Ethereum Job Portal Smart Contract is open-source and available under the MIT License. Feel free to use and modify it for your own projects.

## Disclaimer

This smart contract is provided for educational purposes and as a starting point for building decentralized applications. Please be aware of the potential risks and security considerations when deploying and using smart contracts on the Ethereum blockchain.

**Use this code responsibly and at your own risk.**

## Contact

If you have any questions or need assistance, feel free to contact [me](guri252001@gmail.com).

