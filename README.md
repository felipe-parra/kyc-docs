# KYC Docs - Sumsub

## Web SDK Settings

You will configure this properties to your project:
| Property | Example |Type |
| ----------- | --- |----------- |
| Domain | http://localhost:8081 |String or [String] |
| Secret Key (JWT) | eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9... | String |
| Success Redirect URL| https://exmapledomain.com/success | String |

---

## App Token

| Property        | Example                                       | Type               |
| --------------- | --------------------------------------------- | ------------------ |
| Name            | See All                                       | String             |
| Whitelisted IPs | http://localhost:8080, http://www.example.com | String             |
| Permisions      | See Costs, See Client Lists                   | Multiple Selection |

### List of permissions:

Multiple selections

- Application Notes
- Can Moderate
- Change Personal Data
- Manage Users
- Manage settings
- Manage Checks
- Manage KYT Settings
- Manage KYT Transactions
- Manage AML Cases
- Manage Client Lists
- Manage KYT Settings
- Moderation Buttons
- See AML Cases
- See Costs
- See Client Lists
- See Checks
- See KYT Rules
- See KYT Transactions
- See Personal Data
- See Stats

---

## Webhooks

Configuration requirements:
| Property | Example | Type |
| --------------- | --------------------------------------------- | ------ |
| Name | All Applicant Created | String |
| Receiver | HTTP Address | String |
| Target | https://exmple.com/webhook | String |
| Headers | `{"Key":"Value", "Value":"Value"}` | Object |
| Applicant Type | `(empty, for all types), Person or Company` | String |
| Types | `Applicaant create, Applicant pending` | String |
| Secret Key | eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9... | String |
| Try to resend failed webhooks several | True | Boolean |
| Active | True | Boolean |

### Receiver Options

    - HTTP address (Selected)
    - Slack
    - Telegram
    - Email

### Types

- Applicant created
- Applicant pending
- Applicant requires investigation
- Applicant reviewed
- Applicant action pending
- Applicant action reviewed
- Applicant action required investigation
- Applicant's personal info has been changed
- Applicant has been deleted
- Applicant has been reset
- Applicant level has been changed workflow completed

---

## API Integration Phases

This is the API Flow
[Docs](https://developers.sumsub.com/api-flow/#introduction)

<img src="https://developers.sumsub.com/images/api-flow-new.png" width="100%" height="200px"/>
