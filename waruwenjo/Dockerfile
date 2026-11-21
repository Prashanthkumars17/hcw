# WaruWenJo wrapper frontend (NGINX serving prebuilt browser bundle).
#
# Built on GitHub-hosted ARM64 runners and published to GHCR.
# Copies the committed distribution bundle directly into nginx-unprivileged.

FROM docker.io/nginxinc/nginx-unprivileged:1.28-bookworm AS waruwenjo
COPY dist/waruwenjo/browser/ /usr/share/nginx/html/
COPY nginx.conf.template /etc/nginx/templates/default.conf.template
