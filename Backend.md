**Table of Contents**

* [README](https://github.com/alokm/defi-wallet/blob/main/README.md)
* [Problem Statement](https://github.com/alokm/defi-wallet/blob/main/problem-statement.md)
* [User Facing Improvements](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#user-facing-product-improvements)
* [Backend Improvements](https://github.com/alokm/defi-wallet/blob/main/Backend.md#backend-product-operations) - You are here

# Backend Product Operations Improvements

This page covers a series of recommendations for backend improvements designed to provide the right infrastructure to enable defi-wallet to build a product that allows users to be successfull.

**Table of Contents**
* [User Persona Model](https://github.com/alokm/defi-wallet/blob/main/Backend.md#user-persona-model)
* [Instrument the App](https://github.com/alokm/defi-wallet/blob/main/Backend.md#instrument-the-app)
* [Product Operations Dashboard](https://github.com/alokm/defi-wallet/blob/main/Backend.md#product-operations-dashboard---productops) 

## User Persona Model

The user persona model is defined in three dimensions with two states each based on the user's: **ability**, **experience**, and **size of wallet**

* Two personas by **ability** - where **ability** is a measure of a user's skill or knowledge about the capabilities of the defi-wallet app
  - **Casual Users** - lightweight users who store and stack crypto with the occasional swap or staking activity (>50% of users are casual)
  - **Power Users** - hardcore users with complex multi-chain needs and active trader user cases involving frequent swap or staking activity (top 10-20% of users are power users)
* Two personas by **experience** - where **experience** is a measure of the users time with defi-wallet in calendar time and/or session time
  - **Noobs** - new users to defi-wallet who have yet to become stuck on the product
  - **Veterans** - experienced active users on defi-wallet who make up our most loyal users
* Two personas by **size of wallet** - where **size of wallet** is a measure of average assets under management in terms of portfolio value
  - **Honey Badgers** - small wallet balance 
  - **Whales** - huge wallet balance 

## Instrument the App
- Install Product Analytics Stack
	- Install [Segment.com](https://segment.com/) - User Data Collection platform
		- On website
		- On Chrome extension
		- On iOS 
		- On Andriod
	- Install [Amplitude.com](https://amplitude.com/) - User activity and engagement analytics
	- Install [FullStory.com](https://www.fullstory.com/) - User behavior insights and analytics
- Configure Product Analytics Stack
	- Wire up dashboards to track user personas by **ability**, **experience**, and **size of wallet**
	- Setup Amplitude.com to run standard user engagement reports by cohort and user segment
	   - Wire up actions corresponding to each product page and feature entry point
	   - Wire up features end-to-end across app and cross platform
	- Setup FullStory.com to run per user behavior insights and analytics to understand user journeys, particularly across device
	- Build an Engagement funnel from activation to multiple steps of a user's engagement journey as they discover the apps full capabilitiies
	

## Product Operations Dashboard - ProductOps

Build a ProductOps dashboard that measures **Activity**, **Engagement** and **Satisfaction** by cohort on an ongoing basis. Where cohort is a basket of users who activated in the same time period (weekly or monthly). By measuring cohorts against each other over time, we can identify the impact of new feature enhancements and other strategies for improving product engagement by release date. 

**ProductOps Dashboard** - Starter Pack

* Optimize for **activity, engagement and satisfaction**
  * **activity:** measures active users and core activity metrics across features and actions by platform (mobile, web, chrome app, etc.)
    * daily, weekly, monthly active users 
  * **engagement**  measures depth of engagement across features and actions. Designed to help us understand operational trends in cohorts and segments over time.
    * usage in sessions, sessions/week and session length
    * engagement in feature actions or goals completed 	
  * **satisfaction** measures how happy are users?
    * One question in-app survey to a random subset of users on a weekly basis. Modified CSAT or NPS score - stick to one question. Use a 7-point scale or higher resolution.
    * [optional] Second question. Open-ended. "How can we make it better?" 	
    * Apply some ML on this feedback to do clustering and feature request management from this treasure trove of data. There are lots of 3rd party tools that do this. I’m no expert but I believe Intercom does this well.
  * **New User Funnel:** Build Acquisition > Activation > Onboarding funnel for new users in their first 60 days
  * **Power User Funnel:** Build Noob > Power User funnel to understand how a new user becomes a Power user


* Questions to ask about **Onboarding** and **Usage** metrics
 
  * *Onboarding* - from signup to first transaction
	- How long does it take for a new user to go from signup to first deposit? 
	- How many steps?
	- How many sessions?
	- How many days?
	- How many support tickets?
	- How many users tried and tried but then gave up and failed silently (say after 30 days of inaction)?

  * *Usage* - how does the user behave in-app
	- what features or pages are most used by frequency, sessions, total session time, session time per week etc
	- Core Feature Area usage - Depth of Usage
		- Feature Area A - Wallet home
		- Feature Area B - Atomic Swap
		- Feature Area C - Multi-chain usage
		- ..

## Next Steps

* Explore [User Facing Improvements](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#user-facing-product-improvements)
