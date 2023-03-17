
# StripePaymentGatewayAPI 

Stripe is a very powerful online payment gateway and it is easy to integrate and implement Stripe to accept payments through an API.

## Prerequisites

- A Stripe Account.



## Installation

```bash
Install-Package Stripe.net
```
    
## SecretKey

To run this project, you will need to add the SecretKey to your appsettings.json file

`SecretKey`


## API Reference

#### Create a new customer

```http
  POST /api/customer/add
```

| Parameter | Type       |
| :-------- | :------- |
| `email` | `string` |
| `name` | `string` |
| `creditCard` | `object` |

#### Create Payment/Charge on Customer

```http
  POST /api/payment/add

```
| Parameter | Type       |
| :-------- | :------- |
| `customerId` | `string` |
| `receiptEmail` | `string` |
| `description` | `string` |
| `currency` | `string` |
| `creditCard` | `long` |


## Notes

When testing out the Stripe API you got three card numbers to test on. You can set expiration and CVC to what you prefer.

**4242424242424242 :** Successful Payments
**4000000000009995  :** Failed Payments
**4000002500003155 :** Required  Authentication 


# StripePaymentGatewayAPI 

Stripe is a very powerful online payment gateway and it is easy to integrate and implement Stripe to accept payments through an API.
