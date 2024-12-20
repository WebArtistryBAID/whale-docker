# Whale Docker

This is the Docker Compose configuration for the ordering system for BAID's Whale Cafe.

## Get Started

The Docker Compose configuration is intended to be run in production. For development, please check [WebArtistryBAID](https://github.com/WebArtistryBAID)/[**whale-backend**](https://github.com/WebArtistryBAID/whale-backend) and [WebArtistryBAID](https://github.com/WebArtistryBAID)/[**whale-frontend**](https://github.com/WebArtistryBAID/whale-frontend).

* Clone this repository.
* Run `git submodule update --init --recursive`.
* Move `.env.example` to `.env` and add your database credentials, JWT secret key, public hosting base URL, and authorization secrets accordingly.
* In the `frontend` directory, copy `.env.example` to `.env`. Change `VITE_ONELOGIN_HOST` and `VITE_ONELOGIN_CLIENT_ID` accordingly, but leave other entries intact.
* Run `docker-compose up -d`.
* You're ready to start!

## Caveat

* Unfortunately, we had to hardcode `X-Forwarded-Proto` to be `https` because of a weird production environment setup. This may cause issues on your end.
* There is a bug in FastAPI's `StaticFile` that causes it to repeat the app's `root_path`. This issue is compensated for in the frontend.

## Contribution

To contribute, simply open a pull request.

## License

```
    Whale is BAID's Whale Cafe's ordering system.
    Copyright (C) 2024  Team WebArtistry

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

