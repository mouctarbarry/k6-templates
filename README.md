# k6-templates

This repository provides a boilerplate for performance testing using k6. k6 is an open-source load testing tool for testing the performance of APIs, microservices, and websites.

## Table of Contents

- [Introduction](#introduction)
- [How k6 Works](#how-k6-works)
- [Libraries](#libraries)
- [Handling Requests](#handling-requests)
- [Correlations](#correlations)
- [Interpreting Results](#interpreting-results)
- [Sending Results to Grafana](#sending-results-to-grafana)

## Introduction

k6 is a modern load testing tool that provides a simple and powerful scripting environment based on JavaScript. It is designed to be developer-friendly and integrates well with CI/CD pipelines.

## How k6 Works

k6 scripts are written in JavaScript and executed using the k6 runtime. The scripts define the behavior of virtual users (VUs) that simulate real user interactions with your application. k6 can generate a large number of VUs to simulate high load and measure the performance of your application under stress.

## Libraries

k6 provides several built-in libraries to facilitate load testing:

- `http`: For making HTTP requests.
- `k6`: Core k6 functionality, including test lifecycle functions.
- `k6/metrics`: For defining custom metrics.
- `k6/ws`: For WebSocket support.

## Handling Requests

To handle HTTP requests in k6, you can use the `http` module. Here is an example of making a GET request:
