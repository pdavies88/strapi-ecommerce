# Strapi React E-Commerce App

## Built with:

- Create React App
- Material UI
- Formik
- Yup form validation
- React responsive carousel
- Redux toolkit
- Strapi
- Stripe

## Instructions:

- Inside the project root run `npx create-strapi-app@latest server`
- This will overwrite the data in your server folder with a new Strapi project so an admin can be set up to load in the project data.

## Example Admin:

- test@gmail.com
- TEST123abc

## Strapi Project Data Entry Instructions:

[https://youtu.be/EBCdyQ_HFMo?t=244&si=curkZZiTT6qKHkj8](https://youtu.be/EBCdyQ_HFMo?t=244&si=curkZZiTT6qKHkj8)

## Allow Access to the Strapi REST API

In the Strapi dashboard go to: `Settings -> Users & Permissions Plugin -> Roles -> Public`, then click on the edit icon and select the dropdown caret for `Item` and `Order` set toggle on the `Select All` checkbox

## Client Folder

In a new terminal run `npm i ` to install and then run `npm run start` to start the front end.

## Stripe Integration

- Inside the new server folder run `npm i stripe` for the Stripe integration
- In the server folder .env add in your Stripe Secret Key
- In the client folder create a .env file and add in REACT_APP_STRIPE_PUBLIC_KEY='CHANGETHISTOYOURSTRIPEPUBLICKEY'
- In the `server/src/api/order/controllers/order.js` adjust the file back to the state it was in prior to the creation of the new Strapi project. This files has specific code to allow for the Stripe integration to push data into Strapi.
