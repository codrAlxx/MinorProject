![bd](https://user-images.githubusercontent.com/57208352/149821063-97bfb91c-3d83-4804-9a85-7b1c76ea1167.png)
# BechDo
Do you think you made a mistake by buying some goods in your freshman year that you no longer need? Do you feel the urge to clear up that clutter and make room for something more useful? Are you up for selling/renting it to your juniors so that they don't end up making the same mistake and could save a few bucks?

Well then we've got your back! Presenting **BechDo**,

✨List your product on the app so that potential buyers from your college, i.e. your juniors can contact you via the inbuilt chat functionality and seal the deal. You can even keep a track of your active products and mark them as unavailable or permanently delete them if they have been sold.

✨The ones looking to buy some stuff can simply go through the various products offered, filter them based on type(For sale or Rent), college, category and/or price, add some of them to their wishlist and obviously contact the seller.

So what are you guys waiting for! **BechDo pe BechDo** ya _Khareed Lo_ 🙃


## Tech Stack

[![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/) [![Adobe XD](https://img.shields.io/badge/Adobe%20XD-FF61F6?style=for-the-badge&logo=Adobe%20XD&logoColor=white)](https://www.adobe.com/products/xd.html?sdid=12B9F15S&mv=Search&ef_id=CjwKCAjwwqaGBhBKEiwAMk-FtLdh_6WSOFgrFUSXMn7OV-3yYdf47-XcDa2PbqiybAFRYmLx7eRYsRoCkDcQAvD_BwE:G:s&s_kwcid=AL!3085!3!526748867264!b!!g!!experience%20design%20adobe!1641846445!65452677271) [![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com/) [![Firebase](https://img.shields.io/badge/firebase-ffca28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/) [![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?&style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/) 

## Features✨

- `Authentication` : This is implemented using Firebase Auth. A first-time user needs to sign up upon opening the app. On doing the same, the user will receive a verification mail. The link in the mail will verify the user after which they can sign in. If the mail is not sent due to any error, there's an option for the user to request for it again at an interval of 30 seconds. The user upon forgetting the password can use an option to reset their password, through which they will receive a mail, which will direct them to change the same. 

- `Create and Edit Profile` : Users need to fill out a profile section mentioning their name, date of birth, college name and year, profile picture is optional. The college name has to be selected from a drop-down list. In case, user's college is not present in the list then they will have to <a href="mailto:bechdoofficial@gmail.com" >contact us<a> to get it updated on our server. College name and date of birth cannot be changed once entered. 
  
- `Sell/Rent Products` : While listing a product, users need to provide a short description, title, category and images (atmost 7). Images are compressed while uploading to 25 % of their quality, still smaller image sizes are preferable.
  
- `Track/Remove products` : The sellers can track the products posted by them in the Active Products section. They can also mark them as unavailable temporarily (after which they will be visible in the Sold Products section) or remove them permanently.
  
- `Search Products/Add Filters` : Users can make use of title based search for Products and can also filter them based on type(for sale/rent/both), category, college and price.
	
- `Favourites` : Users can mark the products as favourites but this is limited to 10 products (due to Firestore's restriction on whereIn query on arrays, which has been employed to fetch products using an array of favouriteProductIds of user, stored online to provide a multi-device experience).
  
- `Messages` : Buyers and sellers can chat with each other to negotiate price and discuss the sale. The Chat functionality has been implemented using Firebase Realtime Database. Users also get push notifications for any new messages (not real-time but updated every 15 minutes using Jetpack Work Manager).
  
- `Help` :  Users can check out this FAQs section in the app to clear out their queries.  


## Setting up the project and Installation

BechDo requires [Android studio](https://developer.android.com/studio) to run.

Install the dependencies to get started.

fork the project
```sh
Using the fork option just below your profile image
```
clone the project in your own device
```sh 
git clone 'https link'
```
make a new branch
```sh
git checkout -b 'name_of_your_new_branch' 
```
open project in Android studio and do the needful changes

<p float="left">
<img src="https://user-images.githubusercontent.com/56028723/168736245-10acdf35-90d9-40ed-9b72-83c54f28de24.jpg" width="300" height="700">	
<img src="https://user-images.githubusercontent.com/56028723/168736258-180be7d2-a437-4f2f-9d9a-7891d250183b.jpg" width="300" height="700">
</p>
	
	
![1](https://user-images.githubusercontent.com/56028723/168736245-10acdf35-90d9-40ed-9b72-83c54f28de24.jpg)
![2](https://user-images.githubusercontent.com/56028723/168736258-180be7d2-a437-4f2f-9d9a-7891d250183b.jpg)
![3](https://user-images.githubusercontent.com/56028723/168736262-90c30700-d371-4a0b-acbc-f36a26568633.jpg)
![4](https://user-images.githubusercontent.com/56028723/168736267-77e06c6e-dab2-4cde-b234-cae10733811d.jpg)
![5](https://user-images.githubusercontent.com/56028723/168736272-2c0c3051-8043-492c-8d7d-4ca5e1515ab6.jpg)
![6](https://user-images.githubusercontent.com/56028723/168736275-96fd1c88-be90-4103-8563-fb8e7b466ca7.jpg)
![7](https://user-images.githubusercontent.com/56028723/168736278-ff03925b-3a41-467f-aea9-d47063b4266d.jpg)
![8](https://user-images.githubusercontent.com/56028723/168736279-26e3dd6c-67bf-4ff6-8bff-0f68736978eb.jpg)
![9](https://user-images.githubusercontent.com/56028723/168736283-7452ca7d-11af-4775-bf70-61a929401d4d.jpg)
![10](https://user-images.githubusercontent.com/56028723/168736286-9fe4e198-cc81-4d3b-bb22-fe053413bb8f.jpg)
![11](https://user-images.githubusercontent.com/56028723/168736290-873788c8-b3a2-4b1b-b174-8f7aac1eaa27.jpg)
![12](https://user-images.githubusercontent.com/56028723/168736293-84c208b1-ac15-485a-8c72-9e57f2d4ef11.jpg)


