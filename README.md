# AWS Static Website Deployment

A static HTML/CSS website deployed on AWS using Amazon S3 for storage and public web hosting — no servers provisioned or managed.

## Live Demo

http://aws-static-website-deployment.s3.ap-south-2.amazonaws.com/index.html

## Architecture

- **Amazon S3** — object storage and static website hosting
- **Bucket policy** — public read access granted via `s3:GetObject`
- **No compute** — fully serverless, zero servers to patch or scale

## Steps

1. Created an S3 bucket with public access unblocked
2. Uploaded `index.html` to the bucket root
3. Enabled static website hosting (index document: `index.html`)
4. Attached a public-read bucket policy
5. Verified the S3 website endpoint loads the site correctly

## Next Steps

- Add Amazon CloudFront in front of S3 for HTTPS and global CDN caching
- Optionally map a custom domain via Route 53

## Tech Stack

Amazon S3 · IAM Bucket Policy · HTML5 / CSS3

---

**Author:** Mohammed Ashif S
