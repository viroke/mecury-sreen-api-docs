# mecury-sreen-api-docs

# Screen 6 - Dashboard

### (1) Total Balances
* Method: GET
* Endpoint: `api/transactions/dashboard_statistics`

```
// Sample Response
{
  "totalPlanSaved": 14000,
  "creditAvailable": 0,
  "overallBalance": 14251.7,
  "overViewStats": {
    "year": {
      "debit": 0,
      "credit": 14251.7
    },
    "month": {
      "debit": 0,
      "credit": 15.4
    },
    "week": {
      "debit": 0,
      "credit": 2.8
    },
    "today": {
      "debit": 0,
      "credit": 1.4
    }
  }
}
```

### (2) Saved Debit Cards
* Method: GET
* Endpoint: `api/users/debit_cards`

```
// Sample Response
{
  "data": [
    {
      "id": "59",
      "type": "user_debit_cards",
      "attributes": {
        "card_number": "7014",
        "expires_on": "09/21",
        "brand": "DIAMOND BANK PLC CREDIT CLASSIC DIAMOND",
        "bank_name": "Not Available",
        "card_type": "VISA",
        "user_info": {
          "id": 1298,
          "name": "John Doe",
          "email": "johndoe@gmail.com"
        },
        "created_at": "2020-03-05T15:07:52.475Z"
      }
    }
  ]
}
```

### (2) Transaction List
* Method: GET
* Endpoint: `api/plans/view_compound_transaction`

```
// Sample Response
{
  "data": [
    {
      "id": "6767",
      "type": "plan_transactions",
      "attributes": {
        "intended_amount": 1.4,
        "actual_amount": 1.4,
        "approval_required": false,
        "approved_by": null,
        "approved_on": null,
        "is_approved": false,
        "on_hold": false,
        "plan_type": "MERCURY_COOP",
        "transaction_title": "Interest Calculation for Dream My Kolo",
        "transaction_description": "MERCURY_COOP-interest-ID6141-EZOIiqHGGq",
        "transaction_status": "success",
        "transaction_type": "interest",
        "processed_with": "paystack",
        "user_info": {
          "id": 8,
          "name": "Patrick Harry",
          "email": "patrick@gmail.com"
        },
        "used_card_info": {
          "id": 0,
          "card_number": "System Credit",
          "expires_on": "01/01"
        },
        "plan_info": {
          "id": 44,
          "dream_title": "My Kolo Plans"
        },
        "created_at": "2020-08-11T00:00:59.743Z"
      }
    },
    ...
```
