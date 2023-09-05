# Udagram Pipeline

## GitHub
- Developers team has done developing and testing stage, then pushed codes to GitHub with the CircleCI integration.
- When codes are pushed to GitHub, it activates the CircleCI platform.

## CircleCI
- CircleCI will read the `config.yml` file which instructs the platform on what is the actions.
- `config.yml` file is using scripts from `package.json` file.
- The scripts split into 2 main tasks (Front-end and Back-end configuration).

### Scripts
These scripts are from `package.json` file:
- `frontend:install` - To install Front-end dependencies.
- `frontend:build` - To build Front-end template (Angular).
- `frontend:lint` - To lint the Front-end codes.
- `frontend:test` - To test the Front-end codes.
- `frontend:deploy` - To deploy built Front-end to S3 using deploy script.
- `api:install` - To install Back-end dependencies.
- `api:build` - To build/compile Back-end codes.
- `api:deploy` - To deploy built Back-end codes to EB using deploy script.