**Table of Contents**
* [Problem Statement](https://github.com/alokm/defi-wallet#problem-statement)
* [User Facing Improvements](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#user-facing-product-improvements)
* [Backend Improvements](https://github.com/alokm/defi-wallet/blob/main/Backend.md#backend-product-operations)
* [ProductOperationsDashboard](https://github.com/alokm/defi-wallet/blob/main/ProductOpsDash.md#productopsdash)

This page covers a series of recommendations for backend improvements designed to provide the right infrastructure to enable defi-wallet to build a product that allows users to be successfull.

# Backend Product Operations 
**Table of Contents**
* [User Persona Model](https://github.com/alokm/defi-wallet/blob/main/Backend.md#user-persona-model)
* [Instrument the App](https://github.com/alokm/defi-wallet/blob/main/Backend.md#instrument-the-app)
* [Product Operations Dashboard - ProductOps](https://github.com/alokm/defi-wallet/blob/main/Backend.md#product-operations-dashboard---productops) 
* [Marketing Operations Dashboard - MarketOps](https://github.com/alokm/defi-wallet/blob/main/Backend.md#marketing-operations-dashboard---marketops)			

## Backend Product Operations Improvements

### User Persona Model

The user persona model is defined in three dimensions with two states each based on the user's: **ability**, **experience**, and **size of wallet**

* Two personas by **ability** - where **ability** is a measure of a user's skill or knowledge about the capabilities of the defi-wallet app
  - **Casual Users** - lightweight users who store and stack crypto with the occasional swap or staking activity (>50% of users are casual)
  - **Power Users** - hardcore users with complex multi-chain needs and active trader user cases involving frequent swap or staking activity (top 10-20% of users are power users)
* Two personas by **experience** - where **experience** is a measure of the users time with defi-wallet in calendar time and/or session time
  - **Noobs** new users to defi-wallet who have yet to become stuck on the product
  - **Veterans** experienced active users on defi-wallet who make up our most loyal users
* Two personas by **size of wallet** - where **size of wallet** is a measure of average assets under management in terms of portfolio value
  - **honey badger** - small wallet balance 
  - **whale** - huge wallet balance 

### Instrument the App
- Install Product Analytics Stack
	- Install [Segment.com](https://segment.com/) - User Data Collection platform
		- On website
		- On Chrome extension
		- On iOS 
		- On Andriod
	- Install [Amplitude.com](https://amplitude.com/) - User activity and engagement analytics
	- Install [FullStory.com](https://www.fullstory.com/) - User behavior insights and analytics
- Configure Product Analytics Stack
	- Wire up dashboards to track *median users* by skill and *MID* users by account age
	- Wire up dashboards to track two user segments: *casual users* and *power users* by cohort
	- Wire up dashboards to track two user maturity levels: *noobs* vs *EXP* users corresponding to new users vs experienced users.
	- Setup Amplitude.com to run standard user engagement reports by cohort and user segment
		- Wire up actions corresponding to each product page and feature entry point
		- Wire up features end-to-end across app and cross platform
	- Setup FullStory.com to run per user behavior insights and analytics reports 

### Product Operations Dashboard - ProductOps 
* Optimize for **activity, engagement and satisfaction**
  * **activity:** measures active users and core activity metrics across features and actions by platform (mobile, web, chrome app, etc.)
    * daily, weekly, monthly active users 
  * **engagement**  measures depth of engagement across features and actions. Designed to help us understand operational trends in cohorts and segments over time.
    * usage in sessions, sessions/week and session length
    * engagement in feature actions or goals completed 	
  * **satisfaction** measures how happy are users?
    * One questions in-app survey to a random subset of users on a weekly basis. Modified CSAT or NPS score - stick to one question. Use a 7-point scale or higher resolution.
    * [optional] Second question. Open-ended. "How can we make it better?" 	
    * Apply some ML on this feedback to do clustering and feature request management from this treasure trove of data. There are lots of 3rd party tools that do this. I’m no expert but I believe Intercom does this well.
  * **New User Funnel:** Build Acquisition > Activation > Onboarding funnel for new users in their first 60 days
  * **Power User Funnel:** Build Noob > Power User funnel to understand how a new user becomes a Power user


*Acquisition* - signups per week
	- Growth Startup Stack per Segment.com co-founder
		- User Data Platform (User Data Collection) 
			- Segment.com
		- User Analytics (Insight): 
			- Amplitude, 
			- Google BigQuery and Mode Analytics, 
			- Snowflake w/ any BI tool like Tableau or Power BI
		- Customer Interactions (CRM)
			- Intercom 
		- Customer Experience Insightd
			- FullStory
		- Customer Messaging
			- Customer.io
		- Growth
			- Google Ads
			- Facebook Ads
- *Onboarding* - from signup to first transaction
	- How long does it take for a new user to go from signup to first deposit? 
	- How many steps?
	- How many sessions?
	- How many days?
	- How many support tickets?
	- How many users tried and tried but then gave up and failed silently (say after 30 days of inaction)?
- *Usage* - how does the user behave in-app
	- what features or pages are most used by frequency, sessions, total session time, session time per week etc
	- Core Feature Area usage - Depth of Usage
		- Feature Area A - Wallet home
		- Feature Area B - Atomic Swap
		- Feature Area C - Multi-chain usage
		- ..
- *Satisfaction* - how happy are users?
	- One question in-app survey to a random subset of users on a weekly basis. Work with Marketing and Leadership to choose the question but model on CSAT or NPS - stick with it over time. Use a 7 point scale or higher resolution.
	- [Optional] Second question. Open-ended. “How can we make it better?” 
		- Apply some ML on this feedback to do clustering and feature request management from this treasure trove of data. There are lots of 3rd party tools that do this. I’m no expert but I believe Intercom does this well.
	
### Marketing Operations Dashboard - MarketOps 
- Report by marketing channel to better understand our best channels for attracting our most active and loyal users over time.
	- Where do our best users come from?
	- What makes our best users unique?
	- How do we attract more of our best users?
