# AWS Infrastructure Automation with Terraform

## Overview

This project demonstrates modular and reusable AWS infrastructure
provisioning using Terraform.

The project follows a separation-of-concerns architecture with:

- Environment-specific root modules
- Reusable Terraform modules
- AWS provider configuration
- Environment-specific variables
- Infrastructure as Code practices
- Secure state and credential management

## Architecture

```text
                    Terraform
                        |
              Environment Root Module
                        |
          +-------------+-------------+
          |             |             |
       Network       Compute       Database
        Module        Module         Module
          |             |             |
          +-------------+-------------+
                        |
                       AWS