# [Cloud Resume Challenge](https://acloudguru.com/blog/engineering/cloudguruchallenge-your-resume-in-azure)

# On AWS : https://jineshkumar.com
My AWS Resume is deployed on S3 Bucket > High awailibility achieved using AWS CloudFront distribution which does the https redirects and Route53 hosted zone


# On Azure : https://www.jineshkumar.ml  
Azure CDN Profile URL : [jineshkumarCDNendpoint.azureedge.net](https://jineshkumarcdnendpoint.azureedge.net/)  
Storage Account Static Website URL : https://jineshkumar.z13.web.core.windows.net/

# CI/CD using [Github Actions](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-static-site-github-actions)
CI/CD solution by Github works out perfect for my resume. With every commit or change in the Resume, Workflow automatically trigger merge of the updated file to Azure Storeage Blob "$web" (Azure Static Website Location) reflects on CDN (Content Delivery Network) endpoint and updates as well and reflects on Custom Domain with SSL (HTTPS) enabled.

This article helped simplied the Github Action Part
https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-static-site-github-actions
