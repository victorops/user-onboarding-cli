# User Onboarding CLI Tool
A python script to transform csv/json/arguments into json and posts to create VictorOps accounts in bulk.

## Usage
```sh
# Manually add one user
./onboard_victorops_user create -apiId asd -apiKey asd -username foo -email foo@bar.gov -firstName foo -lastName bar -phone 1111111111 -teams team1,team2,team3

# Upload CSV
./onboard_victorops_user csv -f accounts-example.csv -apiId abc -apiKey 123

# Upload JSON
./onboard_victorops_user json -f accounts-example.json -apiId abc -apiKey 123
```

## Roles
In VictorOps, the following roles are supported when adding members
* Team
    * team_admin
    * member
* Organization
    * admin
    * team_admin
    * member

## Formats
Examples of the expected Json and CSV format are in the `accounts-example` files in this repo.

Since the fields of orgAdmin and teams are optional, the fields can be left blank in the CSV or json file.
