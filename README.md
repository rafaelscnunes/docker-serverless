This repository contains the code used in the talk _Leveraging Docker to Build Serverless Platforms_ by [Tercio de Melo](https://github.com/terciodemelo) to take place on October 1st [Docker Meetup at VTEX Rio de Janeiro](https://www.meetup.com/Docker-Rio-de-Janeiro/events/264791000/).

It doesn't aim to provide a production ready infrastructure, but rather experiment with Docker inner APIs to gain insight into container orchestration systems by implementing a serverless Python system.

# Repository Organization
Each stage of our experiment is be properly documented in this very `README.md` file, and each stage is accessible by a Git branch in the format `stage-{int}`. Each component of our system is contained in its own directory under the root directory, with a dedicated `README.md` documenting the component. Components are leveraged with Docker Compose.  

# Stage 1
```
.
├── docker-compose.yml
├── LICENSE
├── nginx
│  ├── Dockerfile
│  ├── nginx.conf
│  └── README.md
└── README.md
```

The goal of this stage is to provide a REST API to manage Docker containers; [check how it's done](nginx/README.md)