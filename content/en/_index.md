---
# title: "API Route Zero"
weight: 1
type: docs
---
# What
API Route Zero is an opinionated and pragmatic guide for building and operating REST APIs.

# Why
We're pretty good at building REST APIs these days, but what is still hard is picking a REST style to consistency apply across your APIs and a way to operate them in a practical way at scale. So that's how we'll break this up, style and operations.

# Cars as an example
We'll use cars as an example throughout this guide, mostly because we all understand what cars are, and there are lots of expanded examples to work with that most people understand. Specifically we'll use a car sales company coincidentally called API Route Zero.

# Style

## URL structure

### Subdomains
Use subdomains for to two things:
- Routing intra-network
- Separating your production and non-production environments

#### Routing
The first subdomain should be used in the event that you may have APIs you only want internally to a company network and APIs you wanted exposed outside the company to the Internet. A few examples:
- `api.prod.apiroutezero.com`
- `api-internal.prod.apiroutezero.com`

#### Environment separation
The second subdomain should be the environment. A few examples:
- `prod.apiroutezero.com`
- `dev.apiroutezero.com`

### Collection name
The first URI element should be reserved for the name of the collection. Always make the collection names plural. A few examples:
- `api.prod.apiroutezero.com/cars`
- `api.prod.apiroutezero.com/customers`

### Versioning
The second URI element should be reserved for the version of the collection. Conform to a pattern of `v` and then the major version number of the collection. A few examples:
- `api.prod.apiroutezero.com/cars/v1`
- `api.prod.apiroutezero.com/customers/v3`

## Type of collections
Anything you would ever want to do with a REST API can be classified into one of three collection types:
- *CRUD* - 

## CRUD

### Get a car

### Create a car

### Update a car

### Delete a car

### List all the cars

## Search

## Transactional

# Operations