# Create a site
hugo new site myblog

# Create new post
cd myblog
hugo new posts/`date +%Y-%m-%d_%H-%M-%S`.md

# Download theme
cd myblog
git init
git submodule add https://github.com/matsuyoshi30/harbor.git themes/harbor

# Build the site
rm -rf public
hugo -D

# Start server
hugo server
