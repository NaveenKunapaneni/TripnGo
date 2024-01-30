# # CSCI 5709 Grp-18

The project is built upon the backdrop of the increasing demand for a streamlined and user-friendly solution for booking travel packages. Traditional methods of booking trips often lack transparency and comprehensive information, leading to difficulties for users in selecting suitable options within their desired budget and preferences. To bridge this gap, our project endeavours to tackle these challenges through the development of a resilient web-based platform that delivers a seamless and user-friendly experience. Harnessing the capabilities of cutting-edge technology, our objective is to establish a centralized hub empowering users to effortlessly search, compare, and book personalized travel packages that align precisely with their unique requirements.

- _Deployment URL_: <https://incandescent-flan-2c4d6d.netlify.app/>
- _Backend URL_: <https://web-project-backend-erns.onrender.com>

## Authors

1. Abhishek Bhatt
2. Naveen Kunapaneni
3. Parshva Shah
4. Rahul Saliya
5. Siddhesh Salve
6. Sindhu Bhimavarapu

## Testing

For testing this project, We have tested the web app on various devices and browsers. The web app is tested on the following devices and browsers:

1. Google Chrome on Windows 10, 11
2. Microsoft Edge on Windows 10, 11
3. Mozilla Firefox on Windows 10, 11
4. Google Chrome on Android
5. Brave Browser on Android
6. Samsung Internet on Android
7. Safari on iOS
8. Safari on Mac OS
9. Google Chrome on Mac OS
10. Brave Browser on Mac OS

The individual contributions for developing the backend of our application is mentioned below. Each member has done significant amount of work to complete their fully functional feature:

## 1. User Management[16]

For testing the APIs, users can access the signup & login page by clicking on the signup/login button in the navigation bar. Through this page, users can signup and login while planning to book their desired travel packages.

The user dashboard serves as the gateway for users to interact with the signup and login page for registering their account. The seamless flow from the user dashboard to the sign-up & login page ensures a straightforward and user-friendly experience for users when accessing the registration process. If the user forgets the password user can always select on forgot password button on the login page.

![Alt text](https://res.cloudinary.com/datzhsgw6/image/upload/v1690316780/Screenshot_2023-07-25_134039_kjdqai.png)

After the user registers their account through sign up page, they will be redirected to the profile page:

![Profile page](https://res.cloudinary.com/datzhsgw6/image/upload/v1690319912/Trip%27nGo/Screenshot_2023-07-25_181814_ccgenz.png)

Parshva created Login backend API to fetch the user email and password from frontend. Once the user enters the details and clicks on the Login button, my backend will validate the values with database and if details are correct, it redirects the user to dashboard page. For invalid email it will showcase a message 'User does not exist! Please enter correct email or Signup'. If password is incorrect it will show 'invalid password'. The test case for Login APi is shared in above data and below images.

![Login Page](https://res.cloudinary.com/datzhsgw6/image/upload/v1690317000/Trip%27nGo/Screenshot_2023-07-25_135809_fjawiy.png)

After the user is logged in successfully, they will be redirected to the home page of the website.

![Home Page](https://res.cloudinary.com/datzhsgw6/image/upload/v1690317453/Trip%27nGo/Screenshot_2023-07-25_173641_yif7cu.png)

If the user forgets the password and clicks on it then they will get redirected to '/forgotpassword' page which will ask for their email. For that Parshva has created backend API '/validate-email' which checks for the valid emailid and if it is correct the user will receive the OTP.

![Forgot Password Email](https://res.cloudinary.com/datzhsgw6/image/upload/v1690317258/Trip%27nGo/Screenshot_2023-07-25_150958_k5hlv0.png)

As shown in the below image user enters a valid OTP of 6 digits and then clicks on submit, it redirects them to the 'Resetpassword' page.

![Forgot Password OTP](https://res.cloudinary.com/datzhsgw6/image/upload/v1690317746/Trip%27nGo/Screenshot_2023-07-25_151241_hxyyav.png)

After the user enters the new password and confirms it, the user is navigated back to the Login page so that they can re-enter the email & new password and confirm the login with it.

![Reset Password page](https://res.cloudinary.com/datzhsgw6/image/upload/v1690317955/Trip%27nGo/Screenshot_2023-07-25_151643_vth4mx.png)

Parshva has created admin side login page '/admin' which is used explicitely for the admins to handle the contact-us messages recieved and enter new promo codes from admin side see below image . If the user tries to enter their email id and password on this page they will receive this message 'User is not authorized as an admin'.

![Admin Login page](https://res.cloudinary.com/datzhsgw6/image/upload/v1690317893/Trip%27nGo/Screenshot_2023-07-25_152249_jnmfzj.png)

If the correct credentials are used for Admin login then it will redirect the admin to the 'contact-list' page where a list of contact-us messages are shown.

![Admin side contact-list page](https://res.cloudinary.com/datzhsgw6/image/upload/v1690317856/Trip%27nGo/Screenshot_2023-07-25_173921_l5ljmi.png)

## 2. Profile Management[17]

To test the payment APIs, users can initiate the process by login to the website then the user is dircted to dashboard. when the user clicks on the profile icon the user is redirected to profile page and the user details will be populated in the user profile page.

![Login](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404290/web/eibm5xkx0cxvt5c3ymoq.jpg)

![Click On profile Icon ](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404289/web/vlgqypk9jpftdq1bwk5p.jpg)

![Profile Page](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404288/web/ole66b5ajrlgj4x4fpup.jpg)


To test the payment APIs, users can initiate the process by clicking on the update profile button. Then a modal with the users existing details is displayed. now the user can update the details in the modal and click on save changes. The user will be able to see the updated details on the page as well as the details will be updated in the backend.

![click on edit profile](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404288/web/hu5xyyhrc4t8haubeizy.jpg)

![Updated age](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404288/web/nlapd7yqlmbuisik9cwn.jpg)

![After clicking save changes](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404288/web/a37vhmfljlqncdrmkd5b.jpg)


To test the payment APIs, users can initiate the process by clicking on the update profile image button. Then a modal with the users will be allowed to select an image from the device to upload. The user will click on save changes. The user will be able to see the updated image on the page as well as the image will be updated in the backend.

![Edit profile Image](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404288/web/ltmruskly0nvqi3icyhp.jpg)

![Select Image](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404289/web/abmyidz57ndp3mjenqeu.jpg)

![save changes](https://res.cloudinary.com/djaxleu2q/image/upload/v1690404288/web/awiju8vfdgjibcytllpx.jpg)

## 3. Dashboard & Notifications[18]

- Dashboard

This is the landing page for the project, while creating Rahul created the main theme of the website and the navigation bar. He also created the footer and the spacer component. He also created the trip item component which is used in the dashboard and the wishlist page.
![Alt text](https://res.cloudinary.com/dj2ovidaj/image/upload/v1690387403/screencapture-incandescent-flan-2c4d6d-netlify-app-2023-07-26-12_59_26_jkihev.png)

- Notifications

Rahul has also created the notifications popup which is used to display the notifications and the API for the notifications.
![Alt text](https://res.cloudinary.com/dj2ovidaj/image/upload/v1690387398/Snipaste_2023-07-26_13-01-28_kxg4bz.png)

## 4. Contact-Us & Payment Gateway[19]

![Alt text Img 1](https://res.cloudinary.com/dujnfk24p/image/upload/v1690305604/dly3lguqv06ak1mokam6.png)

After the user submits their response through the contact-us page, they will receive the following message:

![Alt text](https://res.cloudinary.com/dujnfk24p/image/upload/v1690305604/ajlbs6puptcvxb25njwn.png)

As an admin, when you log in and navigate to the contact-list page, you will have access to view the feedbacks submitted by users. The contact-list page will display the feedbacks in a well-organized and easy-to-read format, providing you with relevant details about each entry.

![Alt text](https://res.cloudinary.com/dujnfk24p/image/upload/v1690305604/jgrgazh2razx5m5gbqqb.png)

By clicking on delete button admin can delete the given feedback by users.


![Alt text](https://res.cloudinary.com/dujnfk24p/image/upload/v1690305604/fwvwweadcnpegfchfptw.png)

After the user submits their response, they will be redirected to the Stripe payment gateway.

![Alt text](https://res.cloudinary.com/dujnfk24p/image/upload/v1690305603/cd3teghwoobijpy5ru7y.png)

After the user fills up the required details and completes the payment, the gateway will utilize a webhook to send a notification to the actual website. This notification will contain a success or failure message and will navigate the user to either the dashboard or the payment page, based on the received response.


## 5. Wishlist Feature[20]

![Postman Testing](https://res.cloudinary.com/daqjl702r/image/upload/v1690388159/Web-5709/jl6qrgc0x9pe4aq0mpz4.png)

![Wishlisting an Item](https://res.cloudinary.com/daqjl702r/image/upload/v1690388160/Web-5709/xq8r15xvy2cncypbu6es.png)

![wishlist](https://res.cloudinary.com/daqjl702r/image/upload/v1690388159/Web-5709/qjiwzh3jymbp7ikbdkyl.png)

## 6. Travel package list, Search & Filter[21]          

- Main page of all packages availabe: 
![Alt text](https://res.cloudinary.com/dv0rdcdpa/image/upload/v1690410006/packageslistingpage_vu6bse.png)

- Sample output when user searches for a particular trip type
![Alt text](https://res.cloudinary.com/dv0rdcdpa/image/upload/v1690410006/SearchforTrip_rpyl9y.png)

- Sample output when user filters by location
![Alt text](https://res.cloudinary.com/dv0rdcdpa/image/upload/v1690410006/filterbyLocation_mjxon4.png)

- Sample output when user filters by price 
![Alt text](https://res.cloudinary.com/dv0rdcdpa/image/upload/v1690410006/filterbyPrice_vhruxk.png)

- Filter options available to apply
![Alt text](https://res.cloudinary.com/dv0rdcdpa/image/upload/v1690410006/filterOptions_xexhtx.png)

## Deployment

1. We have created basic backend using [Node.js](https://nodejs.org/en/) and [Express.js](https://expressjs.com/).
2. We have used [Socket.io](https://socket.io/) for realtime notifications.
3. We have used [Stripe](https://stripe.com/en-ca) for payment services.
4. We have used [MongoDB](https://www.mongodb.com/) as the database.
5. We have created APIs for the frontend to consume.
6. We have created API calls in the frontend using axios to consume the backend APIs.
7. We have tested the application locally.
8. We have deployed the backend on [Render.com](https://render.com/) and frontend on [Netlify](https://app.netlify.com/).
9. We have tested the APIs on the deployed version.

## Built With

- [React](https://react.dev) - The web framework used
- [Netlify](https://app.netlify.com/) - Hosting platform used
- [Node.js](https://nodejs.org/en/) - Backend framework used
- [Express.js](https://expressjs.com/) - Backend framework used
- [MongoDB](https://www.mongodb.com/) - Database used
- [Render.com](https://render.com/) - Hosting platform used
- [Socket.io](https://socket.io/) - Used for realtime notifications
- [Postman](https://www.postman.com/) - Used for testing APIs
- [Stripe](https://stripe.com/en-ca) - Used for payment services

## Acknowledgments

[1]. “React Icons,” Github.io, 2023. <https://react-icons.github.io/react-icons/> [accessed June 10, 2023].

‌[2]. “React-Bootstrap,” Github.io, 2023. <https://react-bootstrap.github.io/components/cards/> [accessed June 10, 2023].

[3]. “React-Bootstrap,” Github.io, 2023. <https://react-bootstrap.github.io/layout/grid/> [accessed June 10, 2023].

[4]. Chinwike M., “Create a responsive navbar with React and CSS - LogRocket Blog,” LogRocket Blog, Apr. 2022. <https://blog.logrocket.com/create-responsive-navbar-react-css/> [accessed June 10, 2023].

[5]. D. oscar, “How to make a dropdown notification list with and React?,” Stack Overflow, Jul. 07, 2022. <https://stackoverflow.com/questions/72905276/how-to-make-a-dropdown-notification-list-with-and-react> [accessed May 11, 2023].

[6]. Harita R., “The Most Complete Guide for React Navigation,” CopyCat Blog, Dec. 09, 2021. <https://www.copycat.dev/blog/react-js-navigation/> [accessed May 12, 2023].

[7]. M. Otto, “Flex,” Getbootstrap.com, 2023. <https://getbootstrap.com/docs/4.0/utilities/flex/> [accessed June 12, 2023].

[8] “React Stripe.Js reference,” Stripe.com. [Online]. Available: https://stripe.com/docs/stripe-js/react. [Accessed: 26-Jul-2023].

[9]. Geshan Manandhar, “Geshan’s Blog,” Geshan’s Blog, Jan. 09, 2022 [Online]. Available: https://geshan.com.np/blog/2022/01/nodejs-uuid/ [Accessed: Jul. 16, 2023].

[10]. “Deploy a Node Express App | Render,” Deploy a Node Express App | Render, 2023[Online]. Available: https://render.com/docs/deploy-node-express-app [Accessed Jul. 16, 2023].

[11]. “Express.js And MongoDB REST API Tutorial,” MongoDB, 2023[Online]. Available: https://www.mongodb.com/languages/express-mongodb-rest-api-tutorial [Accessed: Jul. 16, 2023].

[12]. “ObjectID() — MongoDB Node.JS Driver 1.4.9 documentation,” Github.io, 2013 [Online].Available: https://mongodb.github.io/node-mongodb-native/api-bson-generated/objectid.html [Accessed: Jul. 17, 2023].

[13] “Tutorial - 7” Brightspace. [Online]. Available: https://dal.brightspace.com/d2l/le/content/274269/viewContent/3608669/View. [Accessed: 19-July-2023].

[14] F. Kelhini, “How to make HTTP requests with Axios,” LogRocket Blog, 26-Jan-2021. [Online]. Available: https://blog.logrocket.com/how-to-make-http-requests-like-a-pro-with-axios/. [Accessed: 25-Jul-2023].

[15] A. Bilal, “How to use the Fetch API with async/await,” Rapid API Guides. [Online]. Available: https://rapidapi.com/guides/fetch-api-async-await. [Accessed: 25-Jul-2023].

[16] Parshva Shah, “CSCI 5709 Assignment 3.” Dalhousie University, [Online document], 2023. [Accessed 26-Jul-2023]

[17] Siddhesh Salve, “CSCI 5709 Assignment 3.” Dalhousie University, [Online document], 2023. [Accessed 26-Jul-2023]

[18] Rahul Saliya, “CSCI 5709 Assignment 3.” Dalhousie University, [Online document], 2023. [Accessed 26-Jul-2023]

[19] Abhishek Bhatt, “CSCI 5709 Assignment 3.” Dalhousie University, [Online document], 2023. [Accessed 26-Jul-2023]

[20] Naveen Kunapaneni, “CSCI 5709 Assignment 3.” Dalhousie University, [Online document], 2023. [Accessed 26-Jul-2023]

[21] Sindhu Bhimavarapu, “CSCI 5709 Assignment 3.” Dalhousie University, [Online document], 2023. [Accessed 26-Jul-2023]
