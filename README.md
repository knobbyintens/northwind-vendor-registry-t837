# Northwind Analytics — Vendor Due-Diligence Registry

This repository is the authoritative register of third-party vendor
due-diligence reviews maintained by Compliance Operations.

## Layout

- `vendors/<slug>.md` — one record per vendor. Each record starts with a YAML
  front matter block.

## Front matter fields

- `vendor` — legal vendor name
- `slug` — stable identifier, matches the file name
- `service_category` — business service provided
- `risk_tier` — inherent risk rating
- `review_status` — current due-diligence status (`pending_review`,
  `cleared`, `conditional`, `rejected`)
- `renewal_owner` — internal owner of the renewal
- `contract_id` — master contract reference
- Optional fields are added only when a review outcome makes them meaningful:
  `cleared_on`, `playbook_url`

## Change policy

Only Compliance Operations updates records in this repository. Remediation
playbooks live in their own repositories and are never modified from here.
