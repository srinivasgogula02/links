# Static Website with Netlify CMS

This is a simple static website that displays a list of links managed through Netlify CMS.

## Deployment Instructions

### 1. Deploy to Netlify

1. Push this repository to GitHub
2. Log in to [Netlify](https://app.netlify.com)
3. Click "New site from Git"
4. Choose your repository
5. Configure build settings:
   - Build command: Leave empty (no build required)
   - Publish directory: `.` (root directory)
6. Click "Deploy site"

### 2. Enable Netlify Identity and Git Gateway

1. Go to your site settings in Netlify
2. Navigate to "Identity" and click "Enable Identity"
3. Under Identity settings:
   - Enable Git Gateway
   - Set registration preferences (Invite only recommended)
4. Invite yourself as a user:
   - Go to Identity tab
   - Click "Invite users"
   - Enter your email
5. Accept the invitation and set up your password

### 3. Custom Domain Setup

1. In Netlify, go to "Domain settings"
2. Click "Add custom domain"
3. Enter your domain name
4. Update your DNS records:
   - If using Netlify DNS:
     - Follow Netlify's instructions to point your domain nameservers to Netlify
   - If using another DNS provider:
     - Add a CNAME record pointing to your Netlify site URL
     - Example: `CNAME www.yourdomain.com yoursitename.netlify.app`

## Using the CMS

1. Access the CMS at `/admin` on your site
2. Log in with your Netlify Identity credentials
3. Edit the links list:
   - Add new links
   - Modify existing links
   - Remove links
4. Publish changes to update the site

## Local Development

1. Clone the repository
2. Serve the files using a local server
3. Access the site at `localhost` with your chosen port

Note: The CMS will only work on the deployed site with Netlify Identity configured.