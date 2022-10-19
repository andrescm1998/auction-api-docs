# AUCTION API DOCUMENTATION
This is the documentation for the Auction API that you can find in this repo.

**Contents**
- [Getting started](#1-getting-started)
- [Auctions](#2-auctions)

## 1. Getting started

## 2. Auctions
`GET https://auction-api.com/auctions`
This request returns all active auctions
**Example:**
```
[{
  "itemID": 0,
  "itemName": "Lamp",
  "initialPrice": 200,
  "currentPrice": 650,
  "description": "A rare 1870s lamp used in an unsolved murder",
  "numberOfBids": 5,
  "highestBidder": "John Smith"
},{
  "itemID": 1,
  "itemName": "Sword",
  "initialPrice": 1000,
  "currentPrice": 1900,
  "description": "A sword forged in Japan and used by the emperor ",
  "numberOfBids": 12,
  "highestBidder": "Benjamin Franklin"
}]
```

| Field | Type  | Description |
| ------|-------|-------------|
| itemID | integer | A unique ID for each item in the auction|
| itemName | string | The name of the item |
| initialPrice  | integer | Price of the item at the start of the auction |
| currentPrice  | integer | Current price of the item after the most recent bid |
| description  | string | Short description of the item |
| numberOfBids  | integer | Number of bids |
| highestBidder  | string | Name of person with current bid |

Possible errors:

| Error code | Description   |
| ------|-------|
| 404 | Content not found|
