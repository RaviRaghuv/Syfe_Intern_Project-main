FROM openresty/openresty:1.21.4.1-0-alpine

# Fallback nginx.conf inside image (will be overridden by ConfigMap in Kubernetes)
COPY nginx.conf /usr/local/openresty/nginx/conf/nginx.conf

EXPOSE 80

# IMPORTANT: do NOT override CMD/ENTRYPOINT.
# Use the default from the base image, which correctly starts OpenResty.