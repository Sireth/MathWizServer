FROM sireth/math_wiz_front_prod:latest as build-stage


FROM nginx:1.27-alpine

COPY nginx.conf /etc/nginx/nginx.conf

COPY --from=build-stage /math_wiz_front/dist /math_wiz_front/html
