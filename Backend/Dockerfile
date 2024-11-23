FROM public.ecr.aws/lambda/nodejs:20 AS build

WORKDIR /app

COPY package*.json ./


RUN npm install

COPY . .

RUN npm run build

RUN npm prune --production

FROM public.ecr.aws/lambda/nodejs:20

WORKDIR ${LAMBDA_TASK_ROOT}

COPY --from=build /app/dist ${LAMBDA_TASK_ROOT}
COPY --from=build /app/node_modules ${LAMBDA_TASK_ROOT}/node_modules

COPY --from=build /app/package*.json ${LAMBDA_TASK_ROOT}

ENV NODE_ENV=production

CMD ["index.handler"]
