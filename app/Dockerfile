FROM node:12.12

ENV APP_ROOT /src

# Set Timezone
ENV LANG C.UTF-8
ENV TZ Asia/Tokyo

RUN mkdir ${APP_ROOT}
WORKDIR ${APP_ROOT}
COPY . ${APP_ROOT}

RUN npm ci
RUN npm run build

ENV HOST 0.0.0.0
