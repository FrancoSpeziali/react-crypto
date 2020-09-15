# React Crypto

In this project you will be building a crypto currency calculator

You will be converting between USD, GBP, EUR and LTC, BTC, ETH

## What you will be doing

This project assumes you've already had experience with:

- React Basics
- create-react-app
- React Components
- Handling state in React
- Handling styles in React
- Using the Fetch API

🚨 If you are unclear about any of these technologies, please research them before proceeding 🚨

## Cryptocompare API

You can use the following URL syntax for your API fetch calls.

`https://min-api.cryptocompare.com/data/pricemulti?fsyms=&tsyms=&api_key=`

Where `fsyms` are the *from symbols*, i.e, the currency you are converting from.

And `tsyms` are the *to symbols*, i.e, the currency you are converting to.

And `api_key` is the key for the API

A few valid symbols:

`EUR` `GBP` `USD` `BTC` `LTC` `ETH`


#### Examples:

To get EUR into BTC
```
https://min-api.cryptocompare.com/data/pricemulti?fsyms=EUR&tsyms=BTC
```

To get BTC, ETH, LTC into USD, EUR, GBP
```
https://min-api.cryptocompare.com/data/pricemulti?fsyms=BTC,ETH,LTC&tsyms=USD,EUR,GBP
```

To get USD, EUR, GBP into BTC, ETH, LTC
```
https://min-api.cryptocompare.com/data/pricemulti?fsyms=USD,EUR,GBP&tsyms=BTC,ETH,LTC
```

> If you want to test the API, you can use a tools such as [Postman](https://www.postman.com/) or [Insomnia](https://insomnia.rest/)

## Expectations

✔ Build a design of your choice

✔ Separate your code into components

✔ You can use functional or class based components, or both

✔ Your calculator can convert between any of the available currencies from the API

## Assignments

Create a new project folder, using `create-react-app`

Use a folder name of your choice

[How to use create-react-app](https://reactjs.org/docs/create-a-new-react-app.html#create-react-app)

## Design your application

We all want to start write code straight away. Take some time to think about the code you will write, before you write it.

Take a look at the following image.

Before you start building your application, decide what your application will do. Make a rough design of the layout. The design does not need to include details such as fonts, colours or sizes, but should focus on how the parts are arranged and how the User Interface should work.

Then:

1. How would you break this design into smaller parts?

2. What React components could you create?

3. Can any of those components be re-used?

4. How many components will you need?

5. Which information will be part of the state?

## Build your application

### The top level component

- Begin by creating a top level component. This will be the calculator component. You may wish to re-use the `App.js` file which comes with `create-react-app`

### Things to consider

#### You only need to access the API once

There's no need to call the API multiple times - in fact some APIs will block you if you call them too many times!

I would recommend calling it once and storing the result.
1. Design your app (start with something small)

2. Determine what data you need from the API
(play around with the API)

Download and install - Postman (Mansour)
`sudo snap install insomnia` - Insomnia

3. Think about how you will structure your application in terms of components

- what hierarchies will there be
- smart and dumb components

4. Logic - how is it going to work? What will you keep in state?

- Call your API, get your data (store it in state)
- Input
- Output
- Maths

5. Styling
