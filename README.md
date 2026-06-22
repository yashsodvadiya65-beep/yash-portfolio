# Yash Sodvadiya Portfolio Website

This is a static portfolio website for Yash Sodvadiya, built using HTML, CSS, and JavaScript. It is designed for AWS static hosting with S3, CloudFront, ACM, Route 53, and GitHub Actions.

## Local preview

Open `index.html` in your browser.

## AWS hosting steps

1. Create an S3 bucket for the website.
2. Upload `index.html`, `styles.css`, `script.js`, and the `assets` folder.
3. Create a CloudFront distribution with the S3 bucket as the origin.
4. Request an HTTPS certificate in AWS Certificate Manager.
5. Add your custom domain in Route 53.
6. Connect GitHub Actions for automatic deployment.

## GitHub Actions setup

Add these repository secrets:

- `AWS_ACCESS_KEY_ID`
- `AWS_SECRET_ACCESS_KEY`
- `AWS_REGION`
- `S3_BUCKET`
- `CLOUDFRONT_DISTRIBUTION_ID`

Then push changes to the `main` branch.
