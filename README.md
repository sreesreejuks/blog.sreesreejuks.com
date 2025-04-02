# Personal Blog

A personal blog built with Jekyll and deployed on Cloudflare Pages.

## Overview

This repository contains the static files for my personal blog hosted at [blog.sreesreejuks.com](https://blog.sreesreejuks.com). The blog is built using Jekyll and the static files are served through Cloudflare Pages.

## Technology Stack

- Jekyll - Static Site Generator
- Cloudflare Pages - Hosting and Deployment
- GitHub - Version Control and Source Code Management

## Local Development

To run the blog locally using Docker:

1. Run Nginx container with the static files:
   ```bash
   docker run -d -p 8080:80 -v $(pwd):/usr/share/nginx/html nginx
   ```
2. Access the blog at `http://localhost:8080`

## Deployment

The blog is automatically deployed to Cloudflare Pages when changes are pushed to the main branch. The deployment process:

1. Jekyll builds the static site in the `_site` directory
2. The built files are moved to a separate folder
3. The static files are pushed to the repository
4. Cloudflare Pages automatically deploys the updated content

## License

All rights reserved. 