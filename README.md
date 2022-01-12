# [Cloud Resume Challenge](https://acloudguru.com/blog/engineering/cloudguruchallenge-your-resume-in-azure)

# On AWS : https://jineshkumar.com
My AWS Deployed Resume is deployed on S3 Bucket > High availibility achieved using AWS CloudFront distribution which does the https redirects and Route53 hosted zone


# On Azure : https://www.jineshkumar.ml  
Azure CDN Profile URL : [jineshkumarCDNendpoint.azureedge.net](https://jineshkumarcdnendpoint.azureedge.net/)  
Storage Account Static Website URL : https://jineshkumar.z13.web.core.windows.net/

# CI/CD using [Github Actions](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-static-site-github-actions)

CI/CD solution by Github Actions works perfect for my resume. When I want to make any change in the Resume files, Github Action Workflow automatically trigger replace/add the updated file to Azure Storeage Blob "$web" (Azure Static Website Location) reflects on CDN (Content Delivery Network) endpoint and updates there as well thus reflects on Custom Domain with SSL (HTTPS) enabled. Checkout my DeployToAzureStaticWebSite.yaml

(Logic behind now a days WebApps is same. They require continuous Integration and new features deployments. Github Action is at the rescue) 

Just needed .yaml workflow file needs to be created in proper format (Resource below)
This article helped understanding the .yaml file and creation of the workflow. (Easy once you undertand the workflow)  
https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-static-site-github-actions
