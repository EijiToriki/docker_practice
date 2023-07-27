FROM ubuntu:20.04 AS base
RUN apt update
CMD ["sh", "-c", "echo My name is $my_name"]

FROM base AS dev
ENV my_name=TEST

FROM base AS prd
ENV my_name=Bob

# docker image build --target dev .
# docker image build --target prd .