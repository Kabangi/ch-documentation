---
title: API Reference

language_tabs:
  - Request examples

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the ConnectHealth API! You can use our API to access ConnectHealth API endpoints.

This document is a simple guide to application developers to enable easy and convenient development of both mobile and web based applications based on the the connectHealth Api . connectHealth api has been developed with the sole function of providing a robust backend processing of data in alignment with the core concept of the application.

ConnectHealth web services typically follow the REST model for web services. Accessing a REST web service, therefore is merely a matter of making a standard HTTP request to a defined resource. Except where otherwise specified, all of the web services described in this document are accessed by an HTTP GET request. HTTP POST requests are reserved for methods that change and create data on the server, e.g. updating or creating a user's profile. Each request consists of a URI, and a list of parameters. The URI consists of a hostname and base path, a method name, and an optional format specifier. The parameters are appended to the URI on the query string.

You can view the response examples in the dark area to the right.

# Authentication

ConnectHealth implements 0auth2.0 hence to access the API you need to first request an access token using your "client_id" and "client_secret". You can register a new ConnectHealth Client Id and client Secret keys by contact us `support@connecthealth.io`.

ConnectHealth expects for the access_token to be included in all API requests to the server. Either in a header or as a query string 'access_token='

`Authorization: access_token`
## Generating access token


# Users

## Register a new user
## Login a user
## Account Verification
## Resending Verification Code
## Password Reset
## Changing Password
## Updating User