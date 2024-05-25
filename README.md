# Whale Docker

This is the Docker Compose configuration for the ordering system for BAID's Whale Cafe.

## Get Started

The Docker Compose configuration is intended to be run in production. For development, please check [BAIDWebDev](https://github.com/BAIDWebDev)/[**whale-backend**](https://github.com/BAIDWebDev/whale-backend) and [BAIDWebDev](https://github.com/BAIDWebDev)/[**whale-frontend**](https://github.com/BAIDWebDev/whale-frontend).

* Clone this repository.
* Run `git submodule update --init --recursive`.
* Move `.env.example` to `.env` and add your database credentials, JWT secret key, public hosting base URL, and authorization secrets accordingly.
* In the `frontend` directory, copy `.env.example` to `.env`. You should not change the contents of `.env` within the `frontend` directory.
* Run `docker-compose up -d`.
* You're ready to start! Create an account at `/nc/`, and add a data source with hostname `db`, database name `whale`, along with your credentials to use the dashboard.

## Contribution

To contribute, simply open a pull request.

## License

```
    Whale is BAID's Whale Cafe's ordering system.
    Copyright (C) 2024  BAID Web Dev Team

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.
```

