# Whale Docker
For Beijing Academy's Whale Cafe internal ordering system, this is the Docker Compose configuration, bringing all the pieces together for a workable system.

## To run this copy

Before starting, you must have Docker, Docker Compose, and git installed.

1. Clone this repository.
2. Run `git submodule update --init --recursive`.
3. Move `.env.example` to `.env` and add your database and JWT token information.
4. Run `docker-compose up -d`.
5. You're ready to start! Create an account at `/nc/`, and add a data source with hostname `db`, database name `whale`, along with your credentials to use the dashboard.

