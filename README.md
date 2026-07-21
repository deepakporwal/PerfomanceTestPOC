# Performance Test POC

This repository contains a simple performance testing setup using k6 and Taurus.

## Project Structure

- k6/login-test.js: Sample k6 load test script
- taurus/taurus.yml: Taurus configuration that runs the k6 test

## Prerequisites

Make sure you have the following installed:

- k6
- Taurus (BZT)

## Running the Test

From the project root, run:

```bash
bzt taurus/taurus.yml
```

This will execute the k6 script defined in the Taurus configuration.

## What the Sample Test Does

The current test sends a request to https://test.k6.io and checks that the response status is 200.

## Customization

You can adjust the test behavior by editing:

- the k6 script in k6/login-test.js for request logic, thresholds, and load settings
- the Taurus config in taurus/taurus.yml for execution settings and reporting
