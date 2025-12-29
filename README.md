# Project Repository

This is the initial README file for the project.

## Container Path Note

The frontend container root is:
- techlearn-lms-253116-269824/lms_frontend

If any tooling or orchestrators reference:
- techlearn-lms-253116/lms_frontend

They must be updated to the correct path including the `-269824` suffix.

An init override has been added at `.init/.init-run-tool` to ensure commands use the correct working directory:
- WORKDIR=lms_frontend
- START_CMD="CI=true npm start"

## Environment Variables

The frontend expects environment variables prefixed with `REACT_APP_`. Available keys include:
- REACT_APP_SUPABASE_URL
- REACT_APP_SUPABASE_KEY
- REACT_APP_SITE_URL
- REACT_APP_API_BASE
- REACT_APP_API_BASE_URL
- REACT_APP_BACKEND_URL
- REACT_APP_FRONTEND_URL
- REACT_APP_WS_URL
- REACT_APP_NODE_ENV
- REACT_APP_NEXT_TELEMETRY_DISABLED
- REACT_APP_ENABLE_SOURCE_MAPS
- REACT_APP_PORT
- REACT_APP_TRUST_PROXY
- REACT_APP_LOG_LEVEL
- REACT_APP_HEALTHCHECK_PATH
- REACT_APP_FEATURE_FLAGS
- REACT_APP_EXPERIMENTS_ENABLED

