# Transfer-In
User can deposit or transfer gold and tokenize it.

## How to transfer or deposit
1. Register a Gold cache account and complete verification
2. Create a deposit request and get Order Id
3. Deposit or transfer the physical gold at selected partner vault
4. Partner vault receives, verifies and parcelizes the gold
5. CGT equivalent to amount of gold are send to depositor's registered Ethereum address

## User Flow Diagram
![Transfer In - Flow Diagram](https://user-images.githubusercontent.com/44263375/118361101-73afd080-b5a7-11eb-9448-7c16deefccf2.png)


## User Stories
Epic 01       : Deposit and Tokenize Physical gold

User Story 01 : As a potential depositor, I want to deposit physical gold, so that CGT equivalent to amount of gold is deposited to registered Ethereum address.

User Story 02 : As an existing Gold Bullion customer, I want to transfer physical gold to Cache, so that CGT equivalent to amount of gold is deposited to registered Ethereum address.

### User Story 01
As a potential depositor, I want to deposit physical gold, so that CGT equivalent to amount of gold is deposited to registered Ethereum address

 1. A registered customer creates a deposit request in CACHE
 2. Customer receives an email with Order Id and Other details [Order status - Pending]
 3. CACHE admin also gets an email at this point with order details
 4. A heads-up email with Order details is send to the partner vault selected by the customer
 5. Customer deposits the gold at selected partner vault either by shipping or dropping it with Order Id details marked on it
 6. At this point, CACHE admin acknowledges and approves the deposit request. He can also reject the order at this point, if he finds any discrepancies[Order Status-Confirmed/ Rejected]
 7. Once admin approves, Vault Provider verifies the deposited gold and if approved, VO parcelizes it. If it doesn't match the description in the order, order status becomes rejected
 8. Once gold is parcelized, Token Governor starts minting CGT equivalent to gold deposited by customer
 9. CACHE admin verifies deposit and user info, mark as completed
 10. Sends equivalent amount of CGT to customer's Ethereum address along with email notification.[Order status - Completed]

### User Story 02
As an existing Gold Bullion customer, I want to transfer physical gold to Cache, so that CGT equivalent to amount of gold is deposited to registered Ethereum address

 1. A registered customer creates a deposit request in CACHE
 2. Customer receives an email with Order Id and Other details [Order status - Pending]
 3. CACHE admin also gets an email at this point with order details
 4. A heads-up email with Order details is send to the partner vault selected by the customer
 5. Customer wants to move pre-existing Gold in Gold Bullion to Cache, for this customer requests Silver Bullion to withdraw the bar with a message that it has to be gramchainized
 6. Customer has to visit Silver Bullion site, select the gold and withdraw it
 7. Once withdrawal is completed by customer, Silver Bullion communicates with Cache internally by sending an email to Cache
 8. Silver Bullion has to mark the Order Id on the package for easy tracking
 9. At this point, CACHE admin acknowledges and approves the deposit request. CA can also reject the order at this point, if he finds any discrepancies[Order Status-Confirmed/ Rejected]
 10. Once admin approves, Vault Provider verifies the deposited gold and if approved, VO parcelizes.If it doesn't match the description in the order, order status becomes rejected
 11. Once gold is parcelized, Token Governor starts minting CGT equivalent to gold deposited by customer
 12. CACHE admin verifies deposit and user info, mark as completed
 13. Sends equivalent amount of CGT to customer's Ethereum address along with email notification [Order status - Completed]

## Features 
- Transfer Gold
  - User can transfer existing gold to CACHE by placing requests on CACHE and Silver Bullion sites
  - Gold has to be internally transferred to CACHE and has to approved by CACHE Admin and Vault Provider
  - User receives equivalent CGT to the physical gold transferred to CACHE
 
- Deposit Gold
  - User can deposit gold in CACHE by placing a request on CACHE site
  - Gold has to be deposited in the selected Partner Vault and has to approved by CACHE Admin and Vault Provider
  - User receives equivalent CGT to the physical gold deposited in CACHE

## Future Features
- User gets an option to select Transfer or Deposit Gold in Transfer In page
- Order confirmation mail - make changes in content
- Email notification on CGT Transfer

## Dependencies


## What the page looks like now

![Transfer In_Screenshot](https://user-images.githubusercontent.com/44263375/118362180-094d5f00-b5ac-11eb-99ef-9aa0a11d81f7.JPG)



 
