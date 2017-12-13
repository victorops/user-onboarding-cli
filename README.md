# User Onboarding CLI Tool
A python script to transform csv/json/arguments into json and posts to create VictorOps accounts in bulk.

## Usage
```sh
# Manually add one user
./onboard_victorops_user create -apiId asd -apiKey asd -username foo -email foo@bar.gov -firstName foo -lastName bar -phone 1111111111 -role admin -teams team1:admin,team2:member,team3:member

# Upload CSV
./onboard_victorops_user csv -f accounts-example.csv -apiId abc -apiKey 123

# Upload JSON
./onboard_victorops_user json -f accounts-example.json -apiId abc -apiKey 123
```

## Formats
Examples of the expected Json and CSV format are in the `accounts-example` files in this repo.
