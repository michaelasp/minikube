# TEST ONLY: minimal stand-in for the real kicbase image so the workflow runs in
# seconds instead of building kicbase for four platforms. debian-slim rather than
# busybox because the update job runs `dpkg -l` inside the built image.
ARG KICBASE_IMAGE="debian:trixie-20261005-slim"
FROM ${KICBASE_IMAGE}
ARG VERSION_JSON
ARG COMMIT_SHA
LABEL kicbase.test.version_json="${VERSION_JSON}" kicbase.test.commit_sha="${COMMIT_SHA}"
