# Project 4

## Build your own portfolio

A website where you can register and login, add money in cash and buy different stock form different portofolios that we recommend you to buy

## Wireframes
![1](https://git.generalassemb.ly/juanmardikian/project_4/blob/master/Screen%20Shot%202020-03-05%20at%2011.04.41%20AM.png)
![2](https://git.generalassemb.ly/juanmardikian/project_4/blob/master/Screen%20Shot%202020-03-05%20at%2011.09.05%20AM.png)
![3](https://git.generalassemb.ly/juanmardikian/project_4/blob/master/Screen%20Shot%202020-03-05%20at%2011.30.07%20AM.png)

## MVP
​
- Creating a home page to sign in, or log in if you have sign in previously
- Creating a database with the user has many portfolios and the portfolio has many stocks
- Creating a user page where the user can chose between portfolios an stocks
- Backend with full CRUD in ruby
- Shared components, like header and footer and probably portfolios and stocks
​

## Post-MVP
​
- Add money to your portfolio
- Buy stocks and add it to your portfolio and compared in time to the market
- Sell stocks, taking them from your portfolio and adding it to your money
- Auth with Facebook/Google
​

## ERD Diagram
​
![ERD](https://git.generalassemb.ly/juanmardikian/project_4/blob/master/Screen%20Shot%202020-03-05%20at%2011.57.07%20AM.png)
​


## Endpoints
getUsers - returns users
	* GET /users. return all of the users
  * GET /users/:id
  * GET /users/:id/portfolios
  * GET /users/:id/portfolios/:id
  * PUT /users/:id/portfolios/:id/stock/:id
  
  * createUser, updateUser, deleteUser - create, update or delete user information
	* POST /users/:id
	* PUT users/:id
	* DELETE users/:id
  
  Sample JSON from GET `/users`
​
users[0].portfolios[0].stocks[0].name = 'apple'

			[
			    {
			        "id": 1
				“name” : “mardikian”,
                                “email” : “juan@mardikian.es”,
			        “password” : “laMadre”,
			  
			        “portfolios : [{
						{
							"id":1
							name: 'tech'
							stocks:[{
								id: 1
								name: apple,
								price: 200
								},
								{
								name: "microsoft",
								"price": 200
								}]
						},
								
						{
							id:2
							name: 'pharma'
							stocks:[{
								id: 1
								name: pfizer,
								price: 200
								},
								{
								name: proctel,
								price: 200
								}]
						}
						
						]
						
						
				}
			  ]	
			
				

## React Component Hierarchy
​
​
​![Component Hierachy](https://git.generalassemb.ly/juanmardikian/project_4/blob/master/Screen%20Shot%202020-03-05%20at%202.11.24%20PM.png)
​

## Components
​
Breakdown the initial logic of the component pseudocode
​
## ​Routes

| Components | Description                                                                                                              | Type       | State                      |
|------------|--------------------------------------------------------------------------------------------------------------------------|------------|----------------------------|
| App        | This component will render the Header, Footer and Routes.                                                                | Functional | User Sign up an login|
| Login      | This component allows a user to authenticate themselves, to allow the user to access to the portfolios | Functional | Username, Password         | 
| Sign In       | This component will render the Header, Footer and the sign in form.                                                                | Functional | User Sign up an login|
| Header      | This component will render the Header                                                                | Functional | Not Applicable|
| Footer     | This component will rsocial media Icons      | Functional | Not Applicable|
| Portfolio     | This component will render the different porffolios of the user    | Functional | API Data|
| Stocks    | This component will render the different stocks   | Functional | API Data|
| Money    | This component will add the money the user can spen in stocks  | Functional | Not applicable|
| user     | This component will some personal data, and the portfolio the user has    | Functional | API Data|

## Priority Matris
​
![Matrix](https://git.generalassemb.ly/juanmardikian/project_4/blob/master/Screen%20Shot%202020-03-05%20at%202.47.32%20PM.png)
​
