**Client Project Brief**


Scenario Overview
Client: James Smith, freelance web designer

Project: Portfolio Website Deployment

Project Description:
James Smith has designed a modern, responsive single-page portfolio website using Next.js. He needs this website hosted on a robust, scalable, and cost-effective platform with global availability and fast loading times.

Your Role:
As cloud engineers, you will deploy James's Next.js portfolio website on AWS using Infrastructure as Code (IaC) principles with Terraform.

**Requirements; The website must be:**
>Highly Available: Accessible worldwide with minimal downtime

>Scalable: Able to handle increasing traffic without performance degradation

>Cost-Effective: Optimized hosting costs without unnecessary expenses

>Fast Loading: Quick loading times for all visitors globally

**Project Objectives; By completing this project, you will:**

>Deploy a Next.js website on AWS

>Implement Infrastructure as Code using Terraform

>Configure global content delivery with AWS CloudFront

>Apply security and performance best practices

>Host all project files and code on GitHub

**Understanding Next.js**

Next.js is an open-source React framework maintained by Vercel that enhances the development experience for building web applications.

**Key Benefits**

>Server-Side Rendering (SSR): Generates pages on the server for each request

>Static Site Generation (SSG): Pre-renders pages at build time

>API Routes: Built-in API routing system for serverless functions

>File-Based Routing: Simplified navigation through file structure

>Built-In CSS and Sass Support: Easy styling implementation

>Automatic Code Splitting: Loads only necessary JavaScript for current page

**Common Use Cases**

>Static Websites: Blogs, landing pages, and portfolio sites

>E-Commerce Sites: Fast-loading product pages optimized for SEO

>Corporate Websites: Scalable sites for handling significant traffic

>Web Applications: From simple dashboards to complex web apps

>Blogs and Content Sites: Easy-to-maintain, SEO-friendly content platforms

**Step 1: Prepare the Next.js Application**

**1.1 Create a GitHub Repository**

>Go to GitHub and create a new repository named terraform-portfolio-project

>Initialize the repository with a README file

>Clone the repository to your local machine: 

**1.2 Clone the Next.js Portfolio Starter Kit**

**Clone the Portfolio Starter Kit:**

>npx create-next-app@latest nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/main/basics/learn-starter"

>Navigate to the project directory and start the development server:

>Access your Next.js application at http://localhost:3000/

**Create Configuration File**

>In the root of your project folder, create a new file called next.config.js

>Paste the following code into the file:

![Screenshot 2025-05-31 at 1 18 19 PM](https://github.com/user-attachments/assets/47437839-d2ba-4f27-9fe9-642b6a619681)

**Build Your Project**

>After setting up the configuration, run the build command:>

![Screenshot 2025-05-31 at 1 19 37 PM](https://github.com/user-attachments/assets/6a36bb4a-8d4a-45cd-8954-6b0d81fd3519)

This will generate a static export of your Next.js application in the out directory, which can be deployed to any static hosting service.


![Screenshot 2025-05-31 at 1 20 08 PM](https://github.com/user-attachments/assets/3ccd86d3-e6a1-43f6-8c68-277a04204ba9)


 

**Step 1: Initialize Git and Push to GitHub**

![Screenshot 2025-05-31 at 1 20 39 PM](https://github.com/user-attachments/assets/c82bbcdd-2ee2-4570-a4e0-912e1729a0cc)


**Step 2: Create and Share a Loom Video**

>Record Your Loom Video

>-Create a video explaining the Next.js code structure

>-Cover key files and folders (pages, components, public)

>Add Video to README

>-Update the README.md file to include your Loom video link

**Push README Changes**

![Screenshot 2025-05-31 at 1 22 42 PM](https://github.com/user-attachments/assets/d48f920c-cc97-4391-a2b8-217649a9d2d8)

**Step 3: Set Up Terraform Configuration**

**Create Project Directory**

![Screenshot 2025-05-31 at 1 23 39 PM](https://github.com/user-attachments/assets/47742e39-e325-4123-93ef-bedd3819d3fd)

**Create Terraform Files**

>a. State File with S3 + DynamoDB

>b. Main.tf with AWS Provider Block

>c. S3 Bucket Resource

![Screenshot 2025-05-31 at 1 24 21 PM](https://github.com/user-attachments/assets/b660da2e-d0f5-4013-9241-248917bd3a31)

>d. S3 Bucket Policy Resource

![Screenshot 2025-05-31 at 1 25 02 PM](https://github.com/user-attachments/assets/466370f9-93d2-48ea-a36d-45a686d87e69)

>e. CloudFront Distribution

![Screenshot 2025-05-31 at 1 25 55 PM](https://github.com/user-attachments/assets/1a030cb5-761e-4b40-b262-58d08a634dde)

>f. outputs.tf File

![Screenshot 2025-05-31 at 1 26 43 PM](https://github.com/user-attachments/assets/2365b028-8e6d-4699-9538-0ff115b87291)

**Initialize and Apply Terraform**

![Screenshot 2025-05-31 at 1 27 09 PM](https://github.com/user-attachments/assets/94d7e009-6b70-43e9-80fc-b6c2e3fafb38)

**Step 4: Upload the Next.js Static Site to S3**

![Screenshot 2025-05-31 at 1 27 35 PM](https://github.com/user-attachments/assets/18e34aa3-3b3e-45cd-8a25-8c7e5ba162fc)

>-Note: Make sure you're using the correct path to your Next.js build output folder and the correct S3 bucket name.

**Step 5: Access the Deployed Website**

>1. Get the CloudFront URL

![Screenshot 2025-05-31 at 1 28 20 PM](https://github.com/user-attachments/assets/27288327-2800-4228-9def-d95f16f48744)

>2. Access Your Website Open the CloudFront URL in your web browser to view your deployed Next.js portfolio site.
