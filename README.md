# **Carpool App**

<div align="center">
 <img src="./readme-imgs/mongo.png" alt="MongoDB" title="MongoDB" style="background: ; height: 2rem; padding: 0.3rem; border-radius: 0.3rem;"/>
 <img src="./readme-imgs/express.png" alt="Express JS" title="Express JS" style="background: ; height: 2rem; padding: 0.3rem; border-radius: 0.3rem;"/>
 <img src="./readme-imgs/react.png" alt="React Native" title="React Native" style="background: ; height: 2rem; padding: 0.3rem; border-radius: 0.3rem;"/>
 <img src="./readme-imgs/node.png" alt="Node.js" title="Node.js" style="height: 2rem; background: ; padding: 0.3rem; border-radius: 0.3rem;"/>
</div>

---

## 1. Problem

It is not easy for **students** to find other **students** to carpool. They must rely on groups or forum posts to find a suitable carpool that will take them to their destination safely.

<!-- Over the years it has become even harder to find a carpool with the increasing number of social platforms and the challenges that come with each platform. -->

Students are also becoming increasingly worried about their **safety** when join or hosting a carpool to the point where they use other methods besides social platforms. This makes it difficult for students to find a carpool as there is no **centralized** and **safe** board for posting and joining carpools

## 2. Solution

The app is meant to be a **safe** and **easy-to-use** service where students organize and join carpool rides with ease and peace of mind.

Takes less than 5 mins to start using:

> 1. Create an account using you university email<sup>[1]</sup>
> 2. Verify using your university email
> 3. Add a name and picture<sup>[2]</sup>
> 4. Start carpooling 😊

[1]: Available at [select](supportedUnis) Canadian university at launch. More added periodically.  
[2]: Image must follow [guidelines](guidelineLink)

[guidelinelink]: https://link.here/to/guidelines
[supportedunis]: https://link.here/to/supported/unis

## Progress

- [ ] Create user model
- [ ] Setup user auth
- [ ] Add university email validation
- [ ] Add email verification
  - generate random alpha-numeric string of length 5
  - save string and email in db with expiration time (5mins)
  - email js to send verification code
  - change user status to verified upon entering the string for their account
  - allow user to resend a new code every 5 mins
- [ ] create a ride
  - origin university
  - departure location (should be close to university)
  - time of departure
  - ride destination
  - number of passengers
  - price/passenger (est. gas price per person in car should be included in price)
- [ ] join a ride