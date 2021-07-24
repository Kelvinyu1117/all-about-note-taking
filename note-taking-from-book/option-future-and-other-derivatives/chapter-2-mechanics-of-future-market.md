# Chapter 2 Summary
----
## Specification of future contracts
* Asset: Underlying asset represented by the contract
  
* Contract size: Amount of the asset has to be delivered at the expiry date under one unit of contract
  
* Delivery arrangement: Location where the delivery will be made

* Delivery months: The months for delivery

* Price quotes: The way for quoting the price defined by the exchanges (dollars/cents/...)

* Price limits: Usually refers to the daily price movement defined by the exchanges
  * Limit down: the price move down from the previous closing price by an amount = daily price limit
  * Limit up: the price move up from the previous closing price by an amount = daily price limit

* Position limits: maximum number of the contracts that the trader can hold defined by the exchanges, to avoid undue influence on the market
----
## The Argument for the convergence of future price -> spot price

Statement: The future price will be spot price of the asset when the time close to the expiry date

### Case 1 - Future Price > Spot Price
1. The trader can sell the contract and buy the underlying asset, then delivery it
2. Eventually, the price of the future will go **down** as more and more trader apply this strategy
   
### Case 2 - Future Price < Spot Price
1. The trader can buy the contract and sell the underlying asset
2. Eventually, the price of the future will go **up** as more and more trader apply this strategy
   
----
## Operations of Margin Account
Margin account is a brokerage account for the broker to lend the customer money to invest different financial product. The customer need to hold the **maintenance margin** in the margin account, that is the minimum balance required with respect to the total value of portfolio of the margin account. If the balance fall below the maintenance margin, the customer will receive a **margin call**, that require the customer to topup the margin account to fulfill the maintenance margin, this extra fund is called **variation margin**. If the investor doesn't provide this fund, the positions will be closed out to fulfill the requirement.

----
## Operations of OTC market
### Central Counterparties (CCP)
CCP acts as an clearing house between two parties in the OTC market
Suppose A and B agreed the trade, which will be sent to the CCP.
CCP takes on the credit risk of both A and B, that is the CCP gurantee to fulfill the requirements from both parties. Moreover:

* All member of CCP need to provide the initial margin to each transcation and also the variation margin if it is needed.

* If the market participant is not the member of CCP, it can arrange the trade through the CCP member, and the margin need to be provided
  
### Bilateral Clearing
Two parties need to provide collatral to each other, that's the margin required due to the daily valuation of the contract

----
## Types of orders
* Limit order: It specifics a particular price, which can be executed only at this price or better. Not gurantee to be executed

* Market order: It is a order to execute immediately at the best price in the market, it can always be executed

* Stop order: It is an order to buy or sell when the spot price reach a specific price. Usually it is used for stop loss/profit

* Stop limit order: It is the combination of stop order and limit order, when the spot price each the stop price, the order will be convert to limit order

* Market-if-touched order: It is similiar to limit order, but not gurantee the price to be exectuted. When the market price reach the price defined in this order, it will be convert to market order to get the best price in the market